# Write Code to Satisfy Tests

*Basics:* Write Code to Satisfy Tests - explore building code, when the code you build is wrapped with (existing) tests.

*About:* Writing code is accessible, and helped by a framework of tests, but (syntax aside) it's not trivial.

*Source:* Hands-on Lab

*Output:* More, and changed, code in a file on a remote server. ?debrief TDD insights?

## Requirements

Per participant / sharing group:

* Remote environment (built from Ansible playbook to have a web server, Jasmine to run tests, Blockly to build JavaScript, IceCoder to change files, and pre-built `main.js` and `testMain.js`).
* Web-connected device, ideally that can be easily used for typing.

For Facilitator

* Digital Ocean account
* Ansible locally
* Ansible playbook
* Configuration files for environment details, tokens etc. in `./vars`
* Time to set up

## Logistics

Set up the environments an hour before with `ansible-playbook makeDroplets.yml`. You may need to run the playbook twice.

Destroy the environments with `ansible-playbook destroyDroplets.yml` afterwards

Example playbooks, ./vars etc. on [GitHub](https://github.com/workroomprds/WriteCodeToSatisfyTestsAnsible "GitHub - workroomprds/WriteCodeToSatisfyTestsAnsible: Ansible playbooks for &quot;Write Code to Satisfy Tests&quot; exercise").

On first entry to IceCoder, the app will ask for a password. This is a /new/ password, and must be recalled to re-enter later. TEACH YOUR GROUP.

IceCoder may have an off-by-one probem with icons and filenames, so folders aren't as obvious as one might hope.

Each env has a web page that links to all the others. That web page has links to run the jasmine tests and to edit the code with IceCoder. 

That web apge has a "blockly" editor, which builds JavaScript for people who haven't coded, or haven't coded in JavaScript. The advantage is that it makes syntactically-correct JavaScript. Participants will need to paste that code into `main.js`, within the function {}. Add the variable "inbound" and show a logic block.	Note that blockly doesn't have a "return" block on its own – you could set up a blockly function called "main" with an input "inbound", or set up an output variable and change main to return(output).

## Process

Group inexperienced with experienced – but let everyone have their own environment, so that everyone can have their own code and tests.

Take 10 minutes to walk *all* participants through:

* getting to a general page (with an IP address in the browser)
* moving from that general page to their "own" page.
* read the page.
* running Jasmine tests (read the dead ones) (keep it in a tab) (stop random order)
* opening IceCoder, setting a password, browsing to files
* reading testMain.js, and changing it to enable or add a test
* seeing a failed test by rerunning jasmine (show "spec list" vs "failures")
* reading `main.js` and editing to change or add code
* maybe, here, demo a test.


Exercise starts here!

Everyone chooses a test, enables it, strugles (keep track of what you've learned) or doesn't. Repeat.

Try to spot a likely refactoring (ie fn. to choose units, to choose and do truncation and rounding, to cope with non-numeric input) and introduce that refactoring while keeping tests passing. 

Potentially expose another function and test that. 

Look at how the exploration env lets you experiemnt to build judgement and to reveal unexpected behaviour – and how it works as an attractor when building tests is less attractive. Mention approval tests.

Wrap-up with insights / things to remember. Ask for comments from less-experienced people first.

It'll probably take 20 minutes to get "over the hump", and at least 10 more to get refactoring. With 10 mins a the end for insights, this can take you close to an hour, some of which will be uncomfortable. Be sure that you and participants are up for this.

## Versions


## Website text / abstract

In this exercise, you'll write code to satisfy some pre-existing tests.

Each person here has their own server in the cloud. Do work together, but use your own server.

Each server has a web page to give you routes to testing (Jasmine for automation, something trivial for exploration) editing (IceCoder) and visual coding (Blockly) if you want to try it.

You're writing code – a file called `main.js` with a function `main` in it that transforms a variable `inbound` into something else, and returns it. Your pre-written tests express some things about the transformation. 

Your job is to write code to do the transformation, editing a file (on the server) to add and change code, and another file (on the server) to enable (and write) tests. 

Some of this coding will be trivial, some will be confusing. Please work through the confusion, and wok with each other. Experienced coders are encouraged to pair with inexperienced participants, but should not write the code on their server.

In our guided tour, we'll

* get your browser to your own page on your own server
* run Jasmine tests and read the dead ones
* get into our coding environment (setting a password on the way) and browsing to files
* read testMain.js, recognising the conenction with Jasmine, and change it to enable or add a test
* rerun jasmine to seeing the new (probably failed) test
* read `main.js` and edit it to change or add code

Then you'll pick a test to enable, and write code to make it pass.

We'll review what you've done, do more, maybe refactor.

At the end, we'll share what we've done and our reactions to it.

