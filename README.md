<img class="logo" alt="DNS flag day logo" src="/images/IPv4_Flag.svg">

<!--
<div class="translations">
<nav>
	<a href="/cs"><img alt="Česky" src="/flags/cs.svg"/></a>
	<a href="/"><img alt="English" src="/flags/en.svg"/></a>
	<a href="/es"><img alt="Español" src="/flags/es.svg"/></a>
        <a href="/pt-br"><img alt="Português Brasileiro" src="/flags/pt-br.svg"/></a>
</nav> 
</div> CONTRIBUTE TRANSLATIONS ;) -->
<div class="social">
<nav>
	<a href="https://twitter.com/ipv4flagday"><img alt="@ipv4flagday" src="/images/Twitter_Social_Icon_Rounded_Square_Color.svg"></a> 
</nav>
</div>

What is happening?
==================
The current <a href="https://wikipedia.org/wiki/IPv4">IPv4</a> is unnecessarily slow and suffers from inability to deploy new features. To remediate these problems, <a href="#supporters">software vendors</a> and also big <a href="#supporters">content and access ISPs</a> are going to remove IPv4 backwards compatibility in favor of <a href="https://wikipedia.org/wiki/IPv4">IPv6</a> on February 1st, 2030.

This change affects only sites which operate software which doesn't support IPv6. Are you affected?

Site owners
=============
Please check if your site is affected:
<div id="domain-checker">
	<form action="https://dns.google.com/resolve" method="GET" target="_blank">
		<fieldset>
			<legend>Test your site</legend>
			<label for="name">Domain name (without www):
				<input type="text" name="name" id="name" required title="Please enter a domain name to test IPv6 connectivity.">
			</label>
			<input type="submit" value="Test!">
			<noscript>Your browser does not support JavaScript! Consider upgrading your browser...<br>
			</noscript>
		</fieldset>
	</form>
</div>
<script><!-- translate the form above and these constants, please keep the whitespaces! -->
const domainCheckerInit = {
	placeIntoElement: document.getElementById( "domain-checker" ),
	texts: {
		formTitle: 'Test your site',
		labelText: 'Domain name (without www): ',
		submitText: 'Test!',
		reportOkHtml: ': <span style="color: green;">All Ok!</span></div>' +
		'<div><img style="height: 5em;" src="/signs/ok.svg"/></div>' +
		'<div>This site is perfectly ready, congratulations!',

		reportFailHtml: ': <span style="font-weight: bold; color: red;">Fatal error detected!</span></div>' +
		'<div><img style="height: 5em;" src="/signs/dead.svg"/></div>' +
		'<div>This site is going to STOP WORKING after the 2030 IPv4 flag day! Please retry the test to eliminate random network failures. If the problem persists you really need to request a fix from your domain administrator. You can refer them to https://ipv4flagday.net/ ',

		reportTestErrorHtml: ': Test cannot be evaluated because of an error. Please make sure the domain name entered refers to a <strong>domain</strong>, i.e. use "example.com" instead of "www.example.com". Retry the test to eliminate random network failures or investigate.',
	},
	status: {
		loading: 'Testing in progress, please wait… It might take several tens of seconds.',
		done: 'Testing completed:',
		errorApi: 'Communication error! API unavailable… please try again later',
		errorInput: 'Invalid input or other unexpected error, sorry!',
	},
};
</script>
<script src="domain-checker.js"></script>
<br>

Server operators
======================

On or around Feb 1st, 2030, major open source software vendors will release updates that remove IPv4 backwards compatability.

Also <a href="#supporters">content and access ISPs listed below</a> will disable backwards compatability.

Webserver operators
====================
For introduction to IPv6 compatability we recommend you to use form above which produces simplified result for a whole domain.

It is also possible to test your servers directly using dig and any ping binary that supports IPv6. 

The summary result of the website tests should preferably be a green message `All Ok`.

If there is a problem, the tool displays an explanation for each failed test. Failures in these tests are typically caused by:
* lack of IPv6 AAAA dns record
* broken DNS software
* broken firewall configuration
* bad luck

To remediate problems please upgrade your software to the latest stable versions and test again. If the tests are still failing even after a upgrade please check your firewall configuration or talk to your hosting provider. 

**Firewalls must not drop IPv6 packets**, including unknown protocols. Modern software may deploy new protocols (e.g. [DHCPv6](https://en.wikipedia.org/wiki/DHCPv6) to protect from DoS attacks). Firewalls which drop IPv6 packets with such protocols are making the situation worse for everyone, including worsening DoS attacks and inducing higher latency for DNS traffic.

Everyone else
=======================
Make sure to use #ipv4flagday to warn everyone of the 2030 IPv4 flag day. Only if you spread the word your friends and family will be able to connect with you. Ensure to talk to your "internet provider" about IPv4 flag day. We also suggest you to take RIPE's [Introduction to IPv6 course](https://academy.ripe.net/enrol/index.php?id=2) before February 1st, 2030.

Researchers
===========
Researchers and other parties like TLD operators might be interested in:
 * [IPv6 statistics](https://www.google.com/intl/en/ipv6/statistics.html) generated by Google
 * [Why is IPv6 Deployment Important for the Internet Evolution?](http://yadda.icm.edu.pl/baztech/element/bwmeta1.element.baztech-article-BATA-0013-0045/c/httpwww_itl_waw_plczasopismajtit201125.pdf) featuring the National Institute of Telecommunications, Warsaw, Poland


Please read respective methodologies before interpreting the data. In any case, do not hesitate to reach out to people.

Presentations
=============

 * ITU : [slides](https://www.itu.int/osg/dsg/speeches/2009/apr15.ppt)
 * CERN: [slides](https://indico.cern.ch/event/592622/contributions/2576463/attachments/1475449/2285254/IPv6-Training-HEPSYSMAN-v6.pptx)
 * APNIC: [abstract](https://www.apnic.net/community/ipv6-program/ipv6-bcp/)



Contacts
========

 * Please file comments regarding this site in the [ipv4flagday repo](https://github.com/ipviolations/ipv4flagday/issues) on Github

Supporters
==========
They don't endorse anything on this page, but they love the internet.
<script id="do-not-translate-randomize-this-section" src="/supporters-randomiser.js" defer></script>

[![PowerDNS](/images/powerdns.svg)]()

[![ISC](/images/isc.png)]()

[![NLnet Labs](/images/nlnetlabs.svg)]()

[![CZ.NIC](/images/cznic.svg)]()

[![Quad9](/images/quad9.png)]()

[![CleanBrowsing](https://cleanbrowsing.org/images/CleanBrowsing-logo-small-dark.png)]()

[![Cloudflare](/images/cloudflare.png)]()

[![Cisco](/images/cisco.svg)]()

[![Google](/images/google.svg)]()

[![Facebook](/images/facebook.svg)]()
