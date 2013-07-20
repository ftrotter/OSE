OSE
===

The NOD Open Source Eventually License. 

<a href='https://github.com/ftrotter/OSE/blob/master/OSELicense.md'>Click here to read the license!</a>

There have been a history of "Ransom" style licenses in the Open Source community. Recently, Not Only Development (NOD) has been releasing data sets under an Open Source Eventually style license.

We first used the Open Source Eventually concept in our <a href='http://docgraph.org'>DocGraph</a> Crowdfund effort.

A few months after that, Monty Widenius (of <a href='https://mariadb.org/'>MariaDB</a> fame) started calling this concept "Business Source". 

* Monty <a href='http://www.zdnet.com/open-source-its-true-cost-and-where-its-going-awry-by-monty-widenius-7000016024/'>interviewed on the concept with zdnet</a>
* He wrote a blog post <a href='http://monty-says.blogspot.com/2013/06/business-source-software-license-with.html'>about the benifits of Business Source</a>.
* Linus Nyman and Monty wrote <a href='http://timreview.ca/article/691'> a more formal description of the concept in TIM</a>. 
 
I (Fred Trotter) have had fairly extensive experience working with and evaluating Open Source Free/Libre licenses and I know a couple of ways that you can get "burned" by vanity licenses that are poorly written, mangled into proprietary licenses or otherwise abused. The article from Monty essentially recommends a "vanity license" in that it suggest that this licensing strategy be undertaken in a one-off manner. Rather than do that, I would prefer to have a formal, reliable license that is trusted community wide for delaying Open Source releases for fun and profit!!!

Here are the features of the NOD Open Soruce Eventually License:

* This will be a peer reviewed license. Please follow <a href='http://twitter.com/fredtrotter'>Fred Trotter</a> if you would like to be notified when peer review begins.
* We will be using <a href='http://www.co-ment.com/'>co-ment</a>, which is the grandchild of the software that was used to gather comments during the GPL v3 licensing writing process.
* It is not possible to have a formal peer evaluation of a license that can be modified on a per-licensee basis. 
   * This means that the core license file cannot change, which means
   * No changeable dates in the core file, dates in a seperate file called CONVERSIONDATE.txt
   * No changeable terms in the core file, any extra, less restrictive terms are found in EXTRASTUFF.txt
   * This lets us ensure that the core licenses is word-for-word identical very easily (programatically even)
* This liceense extends current best practices established in the FOSS community
   * We have used the files LICENSE.txt, README.txt and COPYRIGHT.txt as the default mechanism for communicating project licensing
   * This project merely extends that practice with several new files
* The Licensor is protected by fairly restritive terms for project use, before the conversion to the Open Source license has occured
   * The user cannot share the Thing outside the company that purchased the OSE license
   * The user cannot offer a download of the Thing
   * The user cannot offer a service around the Thing
   * It is limited to internal use by the end user only
   * Sometimes, a Licensor might want to sell additional privileges for more money. In that case, there is a file called EXTRASTUFF.txt where extra privileges or support warranties etc etc can be defined
* Generally, end-users of licenses need to be protected against Licensors who do no understand the rules of mass-licensing (i.e. peer review of licenses produces trustable known-good options for both creators and consumers)
   * Strict terms ensure that Licensors cannot change how the license works and still call it the "NOD Open Source Eventually License"
   * If a Licensor fails to define the conversion date, then the conversion date is automatically two years from download date
   * If a Licensor picks an unreasonable time in the future, then the conversion date is automatically set two years from the download date
   * (we are not sure about what an unreasonably long time is... for now it is also set to two years...)
   * If a Licensor fails to choose a license, then the end user can pick between the Creative Commons Share-Alike 2.0 and the AGPL.
   * The Licensor cannot use a vanity license and call it Open Source. They must choose one from the approved list from the FSF, OSI or Creative Commons.
   


