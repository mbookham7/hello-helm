Hello helm
==========

hello-helm is an example of helm charts repo used for training and/or testing. 

## How It Works

I set up GitHub Pages to point to the `gh-pages` branch. From there, I can
create and publish docs like this:

```console
$ helm create mychart
$ helm package mychart
$ helm repo index --url https://rawmind0.github.io/hello-helm/.
$ git checkout gh-pages
$ git add mychart-0.1.0.tgz
$ git commit -m "Added mychart-0.1.0 chart"
$ git push origin gh-pages
```

From there, I can do a `helm repo add hello-helm
https://rawmind0.github.io/hello-helm/.`

## License
Copyright (c) 2014-2018 [Rancher Labs, Inc.](http://rancher.com)

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

[http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
