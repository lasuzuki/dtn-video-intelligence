# Using GCP Video Intelligence over the Interplanetary Internet :rocket:
This project has been developed by Dr Lara Suzuki :woman_technologist: [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/larasuzuki.svg?style=social&label=Follow%20%40larasuzuki)](https://twitter.com/larasuzuki) and supervised by Vint Cerf :technologist: [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/vgcerf.svg?style=social&label=Follow%20%40vgcerf)](https://twitter.com/vgcerf), both at Google Inc.

[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/lasuzuki/StrapDown.js/graphs/commit-activity)
[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
![Profile views](https://gpvc.arturio.dev/lasuzuki)
[![GitHub contributors](https://img.shields.io/github/contributors/Naereen/StrapDown.js.svg)](https://GitHub.com/lasuzuki/StrapDown.js/graphs/contributors/)
[![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)
[![saythanks](https://img.shields.io/badge/say-thanks-ff69b4.svg)](https://saythanks.io/to/lasuzuki)

[![ForTheBadge built-with-science](http://ForTheBadge.com/images/badges/built-with-science.svg)](https://GitHub.com/lasuzuki/)

In this tutorial I will demonstrate how to connect use GCP Video Intelligence over the Interplanetary Internet. 

# Setting up the Interplanetary Internet

Please follow tutorial [Multicasting over the Interplanetary Internet](https://github.com/lasuzuki/dtn-multicasting) to set up your nodes. 

Once the hosts are configured you can run the command to get ionstart running:

```
$ ./execute
```

# Google Cloud Video Intelligence

Cloud Video Intelligence API allows you to process frames of videos with a simple API call  from anywhere. With GCP Video Intelligence you can:

1. Quickly understand video content by encapsulating powerful machine learning models in an easy to use REST API. 

2. Accurately annotate videos stored in Google Cloud Storage with video and frame-level (1 fps) contextual information. 

3. Make sense of large amount of video files in a very short amount of time.

4. Utilise the technology via an easy to use REST API to analyze videos stored anywhere, or integrate with your image storage on Google Cloud Storage. 

# Executing Google Cloud Video Intelligence

In the Interplanetary host you choose to run the excecution of the Video Intelligence API, install the library:

```
$ pip install --upgrade google-cloud-videointelligence
```

To use the Video Intelligence API you must be Authenticated. To do that, please follow the instructions in this [GCP Tutorial](https://cloud.google.com/docs/authentication/getting-started). After you've created your service account, Provide authentication credentials to your application code by setting the environment variable GOOGLE_APPLICATION_CREDENTIALS.

```
$ export GOOGLE_APPLICATION_CREDENTIALS="/home/user/Downloads/my-key.json"
```

On the host that will run the Video Intelligence, execute: 

```python
python3 video_processing.py
```
