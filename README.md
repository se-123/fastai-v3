# Starter for deploying [fast.ai](https://www.fast.ai) models on [Render](https://render.com)

This repo can be used as a starting point to deploy [fast.ai](https://github.com/fastai/fastai) models on Render.

The sample app described here is up at https://fastai-v3.onrender.com. Test it out with bear images!

You can test your changes locally by installing Docker and using the following command:

```
docker build -t fastai-v3 . && docker run --rm -it -p 5000:5000 fastai-v3
```

The guide for production deployment to Render is at https://course.fast.ai/deployment_render.html.

Please use [Render's fast.ai forum thread](https://forums.fast.ai/t/deployment-platform-render/33953) for questions and support.

_______________________

__dropbox__

mein export.pkl auf dropbox legen und download link erzeugen (link generator auf fast.ai/deployment_render) <br>
https://www.dropbox.com/s/sdh7c62d11v1seb/export.pkl?dl=0 - link direkt aus dropbox <br>
https://www.dropbox.com/s/sdh7c62d11v1seb/export.pkl?dl=1 - download link über https://syncwithtech.blogspot.com/p/direct-download-link-generator.html

__render / github__

classes anpassen <br>
unter app/server.py download link von dropbox eintragen <br>
classes anpassen

in line 64 return JSONresponse({'result': str(predicition)}) <br>
probieren abhängig von der prediction noch mehr anzuzeigen <br>
a) Übersetzung <br>
b) Link <br>
gibt es eine praktische Art "SVERWEIS" zu machen?

app_view/index.html

Überschrift der Website anpassen, Bild reinladen

__Vorlage__ <br>
https://github.com/science4performance/fastai-v3
