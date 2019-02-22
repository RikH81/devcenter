---
title: Migrating from Travis CI to Bitrise

menu:
  migrating:
    weight: 1

---

So you're looking for a Travis CI alternative for your mobile applications? You came to the right place! Let's dive right in:

## Before we get started

Make sure you have a Bitrise account with a connected repository. Can't migrate from Travis CI to Bitrise without one of those. Find more details in the [guide on getting started with Bitrise](https://devcenter.bitrise.io/getting-started/index/).

{% include message_box.html type="info" title="Migrating an open source project?" content="If you're migrating an open source project from Travis to Bitrise, make sure to configure it as a [Public App](https://devcenter.bitrise.io/getting-started/adding-a-new-app/public-apps/) to get **free access** to unlimited builds, unlimited teammembers and a dedicated concurrency for your app."%}

## The Basics
In Bitrise, the series of actions taken 

## Configuration
Both Travis CI and Bitrise use a YML configuration file to store your workflows. In case of Travis, this will be a `.travis.yml` file in the root of your repository, while for Bitrise it will be the `bitrise.yml` file. The guiding principle of the two is very similar, but be sure to check out the [Basics of bitrise.yml](https://devcenter.bitrise.io/bitrise-cli/basics-of-bitrise-yml/) for more information.

When you connected a repository, Bitrise will actually scan your project and -  in most cases - configures the entire project for you. If it's unable to, you can set up the project manually. Read more on that in our documentation on [setting up configuration](https://devcenter.bitrise.io/getting-started/adding-a-new-app/setting-up-configuration/).

## Workflow triggers
One your project configuration is done, you're able to register a webhook in your repository. If you choose to do so, any code change in that repository will trigger your primary workflow by default. You can also skip this step during app creation to get back to this later.

There is more information on webhooks and the different ways in which to trigger workflows in our [webhooks section](https://devcenter.bitrise.io/webhooks).


## Setting variables


## Artifacts


## Advanced Bitrise
