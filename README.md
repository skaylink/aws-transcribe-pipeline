# Amazon Transcribe-Translate Pipeline

This is a small project that was initiated for the AWS Workshop on 9.2.2023, where most presentations were in German and we wanted a transcription and translation to English for people who don't speak German.

For this, Amazon Transcribe was used and hooked up to Amazon Translate. It basically consists of 2 sets of example code glued together.

The code used for the components can be found here:

- AWS Transcribe: https://github.com/awslabs/amazon-transcribe-streaming-sdk/blob/develop/examples/simple_mic.py 
- AWS Translate: https://docs.aws.amazon.com/translate/latest/dg/examples-python.html

## Usage

Simply run the script `translate-transcribe.py` via command line. It will start a loop where it listens to microphone inputs and sends them to AWS. The translated transcriptions are printed to the terminal.

You have to have your AWS credentials set up of course.

## Take-aways

The transcription and translation worked, but wasn't very good. Improvement ideas:

- use a custom vocabulary for transcription
- let the script translate only finished sentences
- use a different translation service, e.g. DeepL
- use a microphone without noise cancelling / a room with better acoustics
- build a nice GUI
  
