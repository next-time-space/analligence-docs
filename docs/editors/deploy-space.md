---
title: "Deploy Space"
---

# Deployment Space

One last step to get our script out side world. Deployment space allows multiple way of doing that. First step will be creating deploy configuration. If you're using Sandbox console, for POC it's better to go with **Analligence Sandbox CDN**

## Deploy Script to Analligence Sandbox CDN

(1) Navigate to **Deploy Space**

(2) Click on **Deploy Config** button.

(3) Side bar shows up with configurations options. Click on **Create Deploy Config**

(4) Provide configuration name

(5) For Type select **Analligence Sandbox CDN**

(6) Copy the URL showing in the config side bar and save it for future purpose.

(7) Basic URL structure will be like `https://analligence.nexttimespace.com/cdn/{organization}/{workspace}/{configName}/craft.js`

## Deploy script to JFrog Artifacts

(1) If you are using npm repository used by [JFrog](https://jfrog.com/artifactory/) best option will be configuring JFrog parameters and build will be published to your repository.

(2) Navigate to **Deploy Space**

(3) Click on **Deploy Config** button.

(4) Side bar shows up with configurations options. Click on **Create Deploy Config**

(5) Provide Config name. Type JFrog Artifact.

(6) Provide required configurations and save.

<img alt="Analligence Deploy - JFrog" style="max-height: 20rem; padding: 1rem 5rem;" src="/docs/imgs/analligence_deploy_jfrog.png">

(7) Now select the version you want to publish to JFrog. Click on **Deploy** icon

(8) Select the configuration you created and click **Deploy**

<img alt="Analligence Deploy - Target" style="max-height: 20rem; padding: 1rem 5rem;" src="/docs/imgs/analligence_deploy_target.png">

(9) Post success deploy message, if you check artifactory repo, new build should be published.

<img alt="Analligence Deploy - Target" style="max-height: 20rem; padding: 1rem 5rem;" src="/docs/imgs/analligence_deployed_jfrog_deployed.png">

## Deploy to Analligence CDN

When you run Analligence in your environment, we have [cdn-service](https://github.com/next-time-space/cdn-service) which helps to have all Analligence script. It's not just for Analligence but also provide all CDN facility and it's open source. Follow [here](/docs/setup/analligencecdn) for more information.

(1) Navigate to **Deploy Space**

(2) Click on **Deploy Config** button.

(3) Side bar shows up with configurations options. Click on **Create Deploy Config**

(4) Provide configuration name

(5) For Type select **Analligence CDN**

(6) For CDN Host:Port provide all host where CDN is deployed.

(7) For alias Check [Analligence CDN](/docs/setup/analligencecdn)

(8) For Content Path provide the URI where the script will be resolved.

(9) For all SSL configurations check [Analligence CDN](/docs/setup/analligencecdn)

## Deploy using shell script

This option is not available in sandbox environment. This deploy option allows to access the script file and move them to anywhere you want using shell script.

## Next step

Next step would be including craft script in your application. Utilize URL or repository to include Analligence craft script into your application web page. And metrics will be started to flow to Analligence. Please do not use our sandbox environment for production traffic as it's a small server serving multiple organization. Check out [Trends Space](/docs/editors/trends-space) for more information about how to check anality representation.