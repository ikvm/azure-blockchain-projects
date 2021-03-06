# Stratis Blockchain Node on Ubuntu VM

This template delivers the Stratis network to your VM in about 15 minutes (PPA install).  Everything you need to get started using the Stratis blockchain from the command line is included. 
You may select to build from source or install from the community provided Personal Package Archive (PPA).Once installed, 'stratisd' will begin syncing the public blockchain. 
You may then connect via SSH to the VM and launch 'stratisd' to interface with the Stratis blockchain.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-quickstart-templates%2Fmaster%2Fstratis-on-ubuntu%2Fazuredeploy.json" target="_blank"><img src="http://azuredeploy.net/deploybutton.png"/></a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-quickstart-templates%2Fmaster%2Fstratis-on-ubuntu%2Fazuredeploy.json" target="_blank"><img src="http://armviz.io/visualizebutton.png"/></a>

# What is Stratis?

Stratis is a flexible and powerful Blockchain Development Platform designed for the needs of real-world financial services businesses and other organisations that want to access the benefits of Blockchain technologies without the overheads inherent in running their own network infrastructure. Stratis offers a turnkey solution that enables developers and businesses to develop, test and deploy blockchain-based applications quickly and easily, and without the costs and security concerns that would otherwise arise from an in-house implementation.

Stratis - STRAT<br />

Ticker: STRAT<br />
Consensus: POW & POS (Hybrid)<br />

Block Time: 60 Seconds<br />
Block Reward: 1 STRAT<br />

Full POS from Block 12500<br />

For more information, as well as an immediately useable, binary version of
the Stratis client sofware, see http://stratisplatform.com/.


# Template Parameters

When you click the Deploy to Azure icon above, you need to specify the following template parameters:

* `adminUsername`: This is the account for connecting to your Stratis host.
* `adminPassword`: This is your password for the host.  Azure requires passwords to have One upper case, one lower case, a special character, and a number.
* `dnsLabelPrefix`: This is used as both the VM name and DNS name of your public IP address.  Please ensure an unique name.
* `installMethod`: This tells Azure how to install the software.  The default is using the community provided PPA.  You may choose to install from source, but be advised this method takes substantially longer to complete.
* `vmSize`: This is the size of the VM to use.  Recommendations: Use the A series for PPA installs, and D series for installations from source.

# Getting Started Tutorial

* Click the `Deploy to Azure` icon above
* Complete the template parameters, choose your resource group, accept the terms and click Create
* Wait about 15 minutes for the VM to spin up and install the software
* Connect to the VM via SSH using the DNS name assigned to your Public IP
* If you wish to relaunch stratisd `sudo stratisd`
* Stratis will run automatically on restart

# Licensing

Stratis is released under the terms of the MIT license. See `COPYING` for more information or see http://opensource.org/licenses/MIT.
