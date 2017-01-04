# Overview

This is a example Alexa skill to retrieve voicemail count from RingCentral.

To use this sample, you will need 2 accounts:

1. Amazon Developer Account: https://developer.amazon.com/
2. AWS Account: https://aws.amazon.com/

This guide has the following sections:

1. Create Alexa Skill
2. Create Lambda Function

## The Alexa Skill

### Create the skill

1. Access your Amazon developer account at https://developer.amazon.com/alexa
1. Click on `Alexa` > `Alexa Skills Kit` > `Get Started`
1. On the "Building Alexa Skills with the Alexa Skills Kit" page, click `Add a New Skill`

### Skill Information Page

1. Add a `Name`
1. Add a `Invocation Name`
1. Click `Next`

### Interaction Model Page

1. Build an intent Schema

```js
{
  "intents": [
    {
      "intent": "RingCentralGetNewVoicemailCountIntent"
    },
    {
      "intent": "RingCentralGetLatestNewVoicemailIntent"
    },
    {
      "intent": "RingCentralGetOldestNewVoicemailIntent"
    },
    {
      "intent": "AMAZON.HelpIntent"
    },
    {
      "intent": "AMAZON.StopIntent"
    },
    {
      "intent": "AMAZON.CancelIntent"
    }
  ]
}
```

2. Provide some Sample Utterances

```
RingCentralGetNewVoicemailCountIntent for voicemails
RingCentralGetNewVoicemailCountIntent for my voicemails
RingCentralGetNewVoicemailCountIntent give me voicemails
RingCentralGetLatestNewVoicemailIntent for latest new voicemail
RingCentralGetLatestNewVoicemailIntent give me latest voicemail
RingCentralGetOldestNewVoicemailIntent for oldest new voicemail
RingCentralGetOldestNewVoicemailIntent give me oldest voicemail
```

3. Click `Next`

## Create AWS Lambda function

AWS Lambda

## Notes

The following information is on playback of Audio on AWS:

* [AWS SSML Reference](https://developer.amazon.com/public/solutions/alexa/alexa-skills-kit/docs/speech-synthesis-markup-language-ssml-reference)
* [Alexa Audio File Thread](https://forums.developer.amazon.com/questions/5915/error-playing-audio-file-from-s3-in-alexa-skill.html)
