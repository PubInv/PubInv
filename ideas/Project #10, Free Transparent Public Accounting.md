# Provide free, transparent accounting services

The idea here would be to make an API based way to do basic accounting (and allow backups) and auditing and to let anybody use this.

I’m not sure how this relates to the blocckhain idea, but I think it is similar --- particularly around identity management.

Allow anyone to reuse the code that will store accounts, and allow anyone to duplicate the books.

This could be extremely powerful and extremely simple.  If we can make it secure in some way, it could be done in a single sprint.

## Details.

Here is a bit more detail that I wrote in response to some questions in the issues from Ryan Wold:

The value proposition it that many organizations, primarily governments, charities and non-profits, would value from operating completely transparently. (Public Invention is such an organization, but is not yet a registered 501c3 nor has it sought funds except from its founder (me).) That is, a charity would like to be able to say "We operate completely transparently and all of our income and expenses and transactions are available for public review. You may look for yourself at precisely how we spend our money." This statement would be backed up by the fact that all transactions would be available at least through and API, if not not necessarily a GUI. Such a systems would allow anyone to take make a copy of the General Ledger, so that it would be virtually impossible to "cook the books" later and change something without being detected. That is, the general accounting principle of making each transaction immutable, subject only to correction by additional future double-entry transactions, would be verifiable (at least in principle.)

When I say "basic" accounting, I mean a general ledger and a chart of accounts that has a history of double-entry transactions. I personally this should be built using clearly defined standards and APIs, with GUIs being considered a valuable but secondary function. So, for example, in an early release, accounting could be offered as a "Software as a Service" online-application. The credentialized owner can add transactions to the system through and API and but anyone can read the entire GL if they choose to do so. By defining standards and APIs, we allow anyone to make a GUI if they choose. We would of course have to make our own GUI, if only for explanation and testing, but we would not force people to use our GUI --- if somebody writes a better one, or one in Spanish, or one for an iPhone or whatever, they are welcome to use it.

I believe that "basic" should also include the ability to compute income and expense statements and balance sheets at any point in time in a standardized (e.g., JSON) format. However, I would tend to think of most "reporting" as an additional and secondary feature. Likewise, budgeting, however valuable, would not be considered "basic".

Integration would be handled by modular APIs. That is, we would not offer integration per se, but an API for accomplishing this.

Permission would have to be intrinsic in the API definitions for throttling and to control write access. It could also be used to control "read" access, although then you are blurring the line between public and private accounting.

With respect to ongoing maintenance, it is very important to lean on the very "basic" nature of such a system. For example, backup and recovery are an important part of any accounting system. However, if you are offering a free service, you don't really have to offer that---you could say "You have an API that allows you to make a checkpoint of the entire GL at any point in time. It is therefore you responsibility to make your own backups (although we have provided a JSON format for this). Because we are offering a free service and taking no money from you, we are not obligated to continue this service."


<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">PIFAH Project #10: Free Transparent Public Accounting</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/PIFAH/PIFAH" property="cc:attributionName" rel="cc:attributionURL">Robert L. Read</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/PIFAH/PIFAH" rel="dct:source">https://github.com/PIFAH/PIFAH</a>.
