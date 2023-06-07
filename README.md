# ReFramework Cross Platform Implementation

A Crossp-platform version of UiPath's ReFramework project template

This implementation will loop continously waiting for queue items to be processed. In order to set it up correctly, make sure you set the "stop after" parameter in the queue trigger in Orchetsrator. For example, if you are running this on a serverless robot, I suggest to stop it after 10 minutes. This way, when the 15 minutes limit hits, the job won't be killed.

Once you build a new project in UiPath Studio starting from this template, please make sure to change the queue name in the "Wait Queue Item" activity.
