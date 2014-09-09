# PNWScala

This is the code for the PNWScala website. It's just raw code, at the moment. We should probably use a static site generator at some point. One day....

Currently, to preview, just use `python -m SimpleHTTPServer` from within the `src/site` directory. The site is hosted on S3 and there is a redirect at the root level to send visitors from `/` to `/2014/index.html`, but you'll need to just manually go to [http://localhost:8000/2014/index.html](http://localhost:8000/2014/index.html).

To upload the site, use `s3cmd sync --delete src/site/ s3://pnwscala.org` (assuming you have the right access key and secret).

## Notes:

For whatever it's worth, the design for the 2014 website is based on the template here (which I paid for, of course -- it's worth every cent)! --> [http://wrapbootstrap.com/preview/WB02332JB](http://wrapbootstrap.com/preview/WB02332JB)
