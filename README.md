# WindowsServerClientLab


<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Feldanielo%2FWindowsServerClientLab%2Fmaster%2FWindowsServerClientLab%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>

<p>
This Template creates a Windows 7 Client and a Windows Server 2008 Test Lab 
</p>

The parameter "labCount" indicates how often the template should be deployed, making it easy to deploy it for multiple lab users. All resources will be deployed in the same Resource Group and will be tagged by a tailing index starting at 0, indicating its iteration.</br>
e.g: </br>
VirtualNetwork_0 </br>
client-pip_0 </br>
clientnic_0 </br>
client-0 </br>
represents a single deployment and belong to one user. 
It is recommended not to use any digits for the parameters during deployment as filtering resources by number/user won't be possible. 

<p>
Each VM has an DNS name consisting of the paramater "dnsNameForPublicIP" and the name and number of the VM. You can rdp into the machines using this uri</br>
eg: lab-client-0.northeurope.cloudapp.azure.net 
</p>