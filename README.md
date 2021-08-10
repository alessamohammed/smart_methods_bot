# TTS & STT Project

## Getting started

## Credentials


You'll need to sign up for the `Watson STT service`_. As of Sept 2018,
IBM Cloud accounts get 100 minutes / month free.

In order to connect to the Watson streaming server you need an API Key, and to
specify which region your speech to text service was provisioned in (there are
different gateways per region). You can find these on your IBM Cloud console
for the service you have added.

### Pre-requisites and Local Development
Developers using this project should have python3 and pip installed on their local machines.
Api's and Url's are stored as secret env files

#### installation
run ```pip install -r requirements.txt``` All required packages are included in the requirements file.





### Expected Output

To run the application run the following commands:
```
python transcribe.py -t ['required seconds']
```
replace ['required seconds'] with number of seconds

Once you run transcribe.py with a timeout value (-t) you'll get both
incremental output as data comes back, as well as a final stitching of
things together. The output will look something like this.

::

   ./transcribe.py -t 5
   * recording             
اهلا
اهلا
اهلا
اهلا
* done recording
     مرحبا، كيف يمكنني مساعدتك؟
Transcription is far from perfect. and the bot will replay in text and audio.
