# wordy

wordy is a chat bot built on the [Hubot][hubot] framework. It was
initially generated by [generator-hubot][generator-hubot].

[hubot]: http://hubot.github.com
[generator-hubot]: https://github.com/github/generator-hubot

### Running wordy

#### Setup
Set environment vars by filling out a `.env` in this dir. contents:
    export HUBOT_BUILDBOT_URL_NO_TRAILING_SLASH="https://buildbot.YOUR_SITE.com"
    export HUBOT_OAUTHPROXY_VAL="XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX" <- cookie from browser

Set the `oauthproxy` var with the oauth_proxy cookie value in the hubot's redis
brain by calling `hubot buildbot oauth <VAR>`.

#### Running
Run tests with
    $ ./run-tests.sh

You can start wordy locally by running:
    $ bin/hubot

You'll see some start up output and a prompt:

    [Sat Feb 28 2015 12:38:27 GMT+0000 (GMT)] INFO Using default redis on localhost:6379
    wordy>

Then you can interact with wordy by typing `wordy help`.

    wordy> wordy help
    wordy animate me <query> - The same thing as `image me`, except adds [snip]
    wordy help - Displays all of the help commands that wordy knows about.
    ...