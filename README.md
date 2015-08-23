# Catapult
Use Google's Edge Cache CDN for a highly distributed network with SPDY support.

# Usage
Built to work entirely on the [Google App Engine](https://cloud.google.com/appengine/docs), Catapult is an app that proxies your data via App Engine's front end cache. Google's Front End Cache uses a high performance CDN that [spans the globe](https://peering.google.com/about/delivery_ecosystem.html) and supports a range of features that make it more attractive than other alternatives like Cloudfront for certain use cases. 

One very specific use case where an SPDY/HTTP2 CDN beats other alternatives is the serving of a large number of small files - that's precisely the case that Cataput was written for. For other uses, Cloudfront may be more economical - Cloudfront offers [pricing that decreases with usage](https://aws.amazon.com/cloudfront/pricing/) while Google App Engine offers [a constant rate](https://cloud.google.com/appengine/pricing) for outbound data.

