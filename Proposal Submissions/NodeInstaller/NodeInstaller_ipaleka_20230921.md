# Token Quantity
50,000,000

# Abstract
This proposal refers to the development, testing, and one year of administration of the open-source GUI and CLI installer for Voi participation nodes (testnet and mainnet). Users will be able to provide IPs and corresponding administrative users' credentials for any number of network computers, preinstalled with almost any of the contemporary OS distributions. The installer will idempotently install all the software for all the computers and register the nodes for participation in consensus if the address(es) mnemonics are provided.

# Team
Ivica Paleka, ASA Stats (https://www.asastats.com) founder and core developer. This proposal extends the work from two published open-source projects: https://github.com/ipaleka/algorand-provisioning and https://github.com/ipaleka/arrangeit.

This proposal is created as Ivica Paleka's solo endeavor to get familiar with the ecosystem's internal processes, as well as with the team and community.

# Problem Description
One of the highlights from Chris's guest appearance on ReCoop's YouTube channel has been the fact that crypto isn't easy for everyone. And Voi wants to change that fact.

Why would running a Node be anything different?

If you are able to enter your credit card number, expiration, and security code, then also you are able to click how much you are ready to spend on your brand new VPS (virtual private server) and which OS you want to run on it.  Yep, you may even choose where you want it to be physically, like Singapore or Finland.

The provider will send you credentials afterward and you're ready to go.

An ordinary/average person will give up after playing with their server for a couple of hours or a day. The others, who succeed in powering up some long-term processes, and brag about that are not among our target groups. Our target groups are the first group and the experts.

Those groups of people need to run the Voi Participation Node Installer standalone executable (no software installation would be required) and fill out the required fields (IP and credentials of the user with the administrative privileges on related VPS).

Optionally, they will be able to add the mnemonics for the address they want to participate in consensus. If such an address has enough Voi to pay the fee, the node will be registered online.

# Solution Approach
If the address connected with a network computer lacks Voi for paying the fee, or if the user chooses to create a completely new address for the job, then the mnemonics will be presented back to the user to write it down, together with the public address they will need to top up with Voi. In both cases, after the user tops up the address, the following run of the software will register the related node as a participation node.

Users can pick as many network computers as they want, and all of them will be installed and registered online in parallel. The whole process is idempotent, meaning that nothing will change with the system or the software if a user runs the software again with the filled-out required fields.

They will be able to add and remove the nodes. In case of removal, the node will first go offline and the software will uninstall completely without a trace.

The installer software will be able to install a node without providing an IP, and that will imply that they want to install a Node locally in the computer where they have started the installer.

For the advanced users, a configuration file can be created and the installer will pull the data from it.

It is expected that the proposer and the Foundation agree upon security measures that should take place in the software. The content is probably out of scope in this phase.

# Expected Impact & Outcomes for the Voi Community 
All the Node installation issues Voi users are facing will be redirected and resolved in the installer GitHub. If there exists a problem with some Node version installation on some OS, then that problem has to be analyzed and fixed for the installer purposes in the installer code/repository. Sometimes the bug will be redirected as an issue further to the Node package builders, sometimes a new version of the code will take place or only a hard-coded bypass will be added for the OS and/or node version, but it is expected that in most cases a simple link to self-explanatory installer code part will be enough for the reporter to get a grasp on their problem.

After a while, a Voi Node install should become a process stress-wise and expertise-wise comparable to a new address creation.

In case of some emergency or testing requirements, and by developing some quite rudimentary additional code using providers' API, in a couple of minutes, the Foundation will be able to power up a few hundred nodes (or a few thousand). After a few hours or a few days, they can be destroyed with a very small total cost.

# Technical Approach
There are two aspects of the installer software. The first consists of gathering information and installation tweaks for the major OSes. In that phase the Node installation will be tested probably on Debian testing, Ubuntu LTS 22.04, CentOS Linux, Oracle Linux, openSUSE Leap, Alpine, Mac OS Ventura, and Microsoft Windows 11.

In parallel, the GUI and CLI installer software will be developed using Python and Tkinter. Tkinter, obviously, aesthetically isn't a state-of-the-art GUI toolkit, but it is being shipped with Python and it has an almost consistent look across various OSes - that makes it the preferable choice for this phase. Once the project matures, the community is of course free to port the installer software to some more attractive toolkit, but that's out of the scope of this proposal.

The engine that runs the Node software deployment and installation is Ansible.

# Define Success
Success would be a successful installation of the Voi Node software conducted by the installer on 95% of the OSes listed on the front page of https://distrowatch.com/, as well as on the last two versions of Mac OS and Microsoft Windows.

A kind of non-measurable success would be that the installer GitHub repository becomes the main issue tracker for Voi Node installation problems.

# Concerns
Is Voi *the next thing* in the crypto world or not? That represents the main concern for this installer. Of course, Voi can reach the next thing status completely based on its community enthusiasm and in that case installer like this one won't be needed.

Some people can contemplate that the installer can be a too powerful tool in the hands of bad actors. The answer is: bring them rather sooner than later!

# Prerequisite
New hardware for the development should probably be purchased in order to test such software without frustration.

# Project Longevity 
The software will be developed and administrated by the proposer during the first year. No matter of actual success of the project, it is expected that the maintenance continues afterwards.

# Project Length
It is expected that MVP will be prepared for the beta testers after around two months. The first stable release should come a few months later.

In any case, it is expected that the official release will be ready when Voi launches the Mainnet.

# Additional Information
As mentioned in the Team section, this project is, among other reasons,  proposed so Ivica Paleka gets familiar with the ecosystem's internal processes, as well as with the team and community.

The main reason for the need for such a familiarization is to pave the way for https://www.voistats.com where the Voi and ASA Stats communities meet.
