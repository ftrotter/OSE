OSE
=======

The NOD Open Source Eventually License.

<a href='https://github.com/ftrotter/OSE/blob/master/OSELicense.asciidoc'>Click here to read the license!</a>

An Open Source Eventually License allows a creator to license copyrights (etc) to a user that will become Open Source on a particular date. This is good for the user, because they end up getting good Open Source stuff, and they eventually have the freedom to change how the stuff works! This is good for the creator because they can ensure that they can pay the bills. This works especially well for data, software or other projects which have to be updated regularly!

Background
------

There have been a history of "<a href='http://freecode.com/articles/ransom-software-for-fun-and-profit'>Ransom</a>" style licenses in the Open Source community. Most notably the considerable work done by Zooko O'Whielacronx around the <a href='http://lists.debian.org/debian-legal/2009/02/msg00047.html'>Transitive Grace Period Public License</a>. He put forward the value proposition really well in a presentation. http://lists.debian.org/debian-legal/2009/02/msg00047.html   Recently, Not Only Development (NOD) has been releasing data sets under an Open Source Eventually style license.

We first used the Open Source Eventually concept in our <a href='http://docgraph.org'>DocGraph</a> Crowdfund effort.

A few months after that, Monty Widenius (of <a href='https://mariadb.org/'>MariaDB</a> fame) started calling this concept "Business Source".

* Monty <a href='http://www.zdnet.com/open-source-its-true-cost-and-where-its-going-awry-by-monty-widenius-7000016024/'>interviewed on the concept with zdnet</a>
* He wrote a blog post <a href='http://monty-says.blogspot.com/2013/06/business-source-software-license-with.html'>about the benifits of Business Source</a>.
* Linus Nyman and Monty wrote <a href='http://timreview.ca/article/691'> a more formal description of the concept in TIM</a>.

My Itch
------
I (Fred Trotter) have had fairly extensive experience working with and evaluating Open Source Free/Libre licenses and I know a couple of ways that you can get "burned" by vanity licenses that are poorly written, mangled into proprietary licenses or otherwise abused. One of the problems with vanity licenses is that it is impossible to programmatically ensure license compliance.

Many community members have been burned by vanity licenses. Rather than have hundreds of slightly different ways to do "Open Source on a timer", I would prefer to have a formal, reliable license that is trusted community wide for delaying Open Source releases for fun and profit!!!

In order to enable programatic compliance efforts, license files must be text-identical, and if you have a different date embedded in each licence file then you have to write code to ensure that the files have identical licensing requirements. The approach that we are taking here ensures that each file can be evaluated programmatically, with simple checksums most of the time. Only the date file should have changing data and then only the date itself should change.

Features
------

### Peer Review

This will be a peer reviewed license. Please follow <a href='http://twitter.com/fredtrotter'>Fred Trotter</a> if you would like to be notified when peer review begins.

* We will be using <a href='http://www.co-ment.com/'>co-ment</a>, which is the grandchild of the software that was used to gather comments during the GPL v3 licensing writing process.
* This should ensure that lots of lawyers (and not just ours) are comfortable with the text as a balance between user and creator interests.
* It is not possible to have a formal peer evaluation of a license that can be modified on a per-licensee basis.
   * This means that the core license file cannot change, which means...
   * No changeable dates in the core file, dates in a seperate file called CONVERSIONDATE.txt
   * No changeable terms in the core file, any custom proprietary terms are found in STARTINGLICENSE.txt
   * This lets us ensure that the core licenses is word-for-word identical very easily (programatically even)

### Not Reinventing

There are well-established mechanisms for communicating licensing within our community(s). This license extends current best practices established by the FOSS community.

   * We have used the files LICENSE.txt, README.txt and COPYRIGHT.txt as the default mechanism for communicating project licensing
   * This project merely extends that practice with several new files
   * We use Asciidoc to write the file itself, to be compliant with meta-legal programming efforts
   * We are trying to work with meta-programming efforts like Common Accord http://commonaccord.org

### How NOD OSE protects creators

The Licensor is protected by fairly restritive terms for project use, before the conversion to the Open Source license has occured
   * The user cannot share the Thing outside the company that purchased the OSE license
   * The user cannot offer a download of the Thing
   * The user cannot offer a service around the Thing
   * It is limited to internal use by the end user only
   * Sometimes, a Licensor might want to sell additional privileges for more money. In that case, there is a file called STARTINGLICENSE.txt where extra privileges or support warranties etc etc can be defined

### How NOD OSE protects end-users

Generally, end-users of licenses need to be protected against Licensors who do no understand the rules of mass-licensing (i.e. peer review of licenses produces trustable known-good options for both creators and consumers)
   * It forces Licensors to describe exactly what FOSS license is being used and when it takes effect.
   * It is not a "promise that an Open Source release will occur" the OSE conversion is automatic and cannot be taken back by the Licensor.
   * Strict terms ensure that Licensors cannot change how the license works and still call it the "NOD Open Source Eventually License"
   * If a Licensor fails to define the conversion date, then the conversion date is automatically two years from download date
   * If a Licensor picks an unreasonable time in the future, then the conversion date is automatically set two years from the download date
   * (we are not sure about what an unreasonably long time is... for now it is also set to two years...)
   * If a Licensor fails to choose a license, then the end user can pick between the Creative Commons Share-Alike 2.0 and the AGPL.
   * The Licensor cannot use a vanity license and call it Open Source. They must choose one from the approved list from the FSF, OSI or Creative Commons.

### Not focuses on just software
We have tried to account for the different ways that hardware, software, bioware and art can be used, licensed and shared.


### Script friendly

By pulling dates and privileges into seperate files from the core license, we intended for this license to be script-friendly.

Lets say you want to seperately sell the privileges of A. Offering a service to the web with your code. B. Allow resellers to resell the pre-Open Source codebase or C. Allow your customers to market their use of your software. You can auto-generate the EXTRASTUFF.txt file to fit with your specific needs.

Alternatively, you might want to give different dates to every downloader. To do this, simply have a script write the the date in the CONVERSTIONDATE.txt file.

