# C--linux-echobot

## Notes 
* Preview in VSCode with command (Ctrl+K V).
* Use clipboard manager 

## Setup 
Use the [link](https://docs.microsoft.com/en-us/azure/bot-service/bot-service-quickstart-create-bot?view=azure-bot-service-4.0&tabs=csharp%2Cvs) to do all the installation you will need both the sdk for 3.1 and 6.0

Below code will help in setting up on ubuntu

<code><pre>
sudo dpkg -i packages-microsoft-prod.deb 
sudo apt update 
sudo apt install apt-transport-https 
sudo apt install dotnet-sdk-3.1 
dotnet --version
sudo apt install dotnet-sdk-6.0
dotnet --version
dotnet new -i Microsoft.Bot.Framework.CSharp.EchoBot
dotnet new -i Microsoft.Bot.Framework.CSharp.CoreBot
dotnet new -i Microsoft.Bot.Framework.CSharp.EmptyBot
</pre>
</code>

Also do not forget to install ngrok and bot emulator<br>
<pre>
ngrok config add-authtoken #your-authtoken#
</pre>

# Two methods to create bots

## Azure Bot Setup
* Follow this [link](https://docs.microsoft.com/en-us/azure/bot-service/abs-quickstart?view=azure-bot-service-4.0&tabs=multitenant) to create azure resource and link the app to Azure bot
* Will eventually have an application and one Azure bot service created 

## Via bot framework and Developer portal
* Do all activities via the UI Developer portal only 
* Eventually Only one application should be created 
* You can do all activities from the Developer Portal

Known issues to be aware of : 
* App settings should always be multitennant 
* Do not use [perview](https://techcommunity.microsoft.com/t5/teams-developer/quot-manifest-parsing-has-failed-quot-in-developer-portal/m-p/3104733/page/3) in developer portal 

## Next steps 
* Deployment for .Net Framework Rest API's [here](https://www.c-sharpcorner.com/article/hosting-asp-net-web-api-rest-service-on-iis-10/)
* More on Deploying on server core with framework [here](https://www.youtube.com/watch?v=iu9ei66_KLo)

## Tools 
* Installed versions [here](https://learn.microsoft.com/en-us/dotnet/framework/migration-guide/how-to-determine-which-versions-are-installed)
* Installation of framework [here](https://bobcares.com/blog/install-net-framework-4-8-on-windows-server-2016/)
* Webserver on IIS [here](https://cloud.google.com/compute/docs/tutorials/basic-webserver-iis)
* Good search [here](https://www.google.com/search?q=powershell+enable+iis+features+windowser+server+gcp&sxsrf=ALiCzsaP54QU9iPRz3i8VFbP5MGTjQBETw%3A1665934951876&ei=ZyZMY_uRNce3z7sPmtWf4Aw&ved=0ahUKEwi74Zmoi-X6AhXH23MBHZrqB8wQ4dUDCA4&uact=5&oq=powershell+enable+iis+features+windowser+server+gcp&gs_lcp=Cgdnd3Mtd2l6EAMyBwghEKABEAo6CggAEEcQ1gQQsAM6DQgAEOQCENYEELADGAE6CgghEBYQHhAKEB1KBAhNGAFKBAhBGABKBAhGGAFQhgFY9wxg3w9oAXAAeACAAbgBiAGDBZIBAzAuNJgBAKABAcgBDcABAdoBBggBEAEYCQ&sclient=gws-wiz)

