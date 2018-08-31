## Scrapy

Un marco de código abierto y de colaboración para extraer los datos que necesita de los sitios web.
De una manera rápida, simple, pero extensible.  
**Instalación**  
` pip install scrapy `

**Ejemplo básico**  
~~~
$ cat > myspider.py <<EOF
import scrapy

class BlogSpider(scrapy.Spider):
    name = 'blogspider'
    start_urls = ['https://blog.scrapinghub.com']

    def parse(self, response):
        for title in response.css('.post-header>h2'):
            yield {'title': title.css('a ::text').extract_first()}

        for next_page in response.css('div.prev-post > a'):
            yield response.follow(next_page, self.parse)
EOF
 scrapy runspider myspider.py 
~~~