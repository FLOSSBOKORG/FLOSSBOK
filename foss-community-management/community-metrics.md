# Community Metrics

Community metrics program serves as a constant reminder of what you want to achieve in the program and should be used as metrics themselves when deciding exactly what they are going to measure.

The following article discusses basic strategy for deciding what to measure, and give examples of specific community metrics we've used in practice. Using the knowledge of community and the goals community managers came up with, it is important to ensure that the metrics that they choose are relevant.

## Types of metrics

There are two major types of metrics used to report on communities: qualitative and quantitative. Qualitative metrics are those that use spoken or written words to convey feedback, such as online surveys, formal usability testing, or in-person discussions. These can capture both structured and unstructured data, and if tracked over time can provide valuable measurement of progress toward your goals. Qualitative metrics are most useful to measure things like "Are the API docs effective enough for your project?" or "What do you think the community should focus on in the next 6-12 months?" The answers can help you understand the pulse of your community and what changes \(if any\) need to be made. Choosing good questions can be difficult, as it's easy to introduce[bias](https://en.wikipedia.org/wiki/Response_bias)accidentally, ask questions for which you have no plan to act on, or questions whose answers don't relate to your goals. Surveys also take a lot of effort each time you conduct them, so we used them sparingly \(about once a year\), primarily to ask the "what should we focus on" kinds of questions.

## Qualitative vs. quantitative metrics

Surveys and studies are great but take an ongoing commitment, whereas the collection and processing of quantitative metrics can often be automated and can provide long-term and consistent benefit after the upfront cost of setting it up. Minimizing \(if not removing\) human emotion and error from a metrics program is very attractive to technically oriented folks in our industry. Ben Yoskovitz, co-author of[Lean Analytics](http://leananalyticsbook.com/), put it this way: "Quantitative data abhors emotion; qualitative data marinates in it."

Basic quantitative metrics are readily available to most modern open source communities—the day-to-day operational online tools we use provide easy ways to obtain historical and sometimes real-time metrics about the activities that take place. We'll explore this in more detail and show you several specific metrics that relate to our community's goals.

#### 1st-order metrics

Take a look at the typical workflow for your community members. Which tools do they use, how do they use them, and what statistics might you be able to extract from them? Usually you'll have access to the basics, what I call 1st-order metrics. These metrics are easily obtainable, but they rarely tell the complete story on their own. The canonical example is the body count \(a.k.a., number of registered users\). If this number is increasing, is that a good thing? Maybe, maybe not. It might mean your recently implemented idea to attract community members is working. But it might also mean your sign-up form was hacked by automated spammers. The same ambiguity can be said about several other 1st-order metrics that we've[previously discussed](https://opensource.com/business/16/7/measuring-what-matters). Dave Neary \(fellow Red Hatter and community builder\) has even more to say on[metrics gone wrong](http://community.redhat.com/blog/2014/07/when-metrics-go-wrong/).

At Liferay, one of our goals was to increase the value of community participation, and metrics like these didn't indicate any real value to a community member. So we had to dig a little deeper.

#### 2nd-order metrics

What does it mean for community participation to be valuable? It's when a community member receives something of value from their participation. Each community is different, but the[results of the Liferay survey](http://www.slideshare.net/schtool/liferay-2012-community-survey-summary)showed that our community members valued sharing, learning, and giving back above all else. So we came up with a set of 2nd-order metrics that we felt indicated value \(or helped us meet our other goals\). These metrics were derived from post-processing and transforming our 1st-order metrics, so going from the easy-to-obtain, hard-to-interpret 1st-order data to our desired metric was not a huge technical feat. Here is a select sampling of the metrics we used, along with their relevancy toward our goals:

* **Number of company vs. non-company members**
  : Maintaining a healthy diversity between evil corporate and scrappy independent developers brings more real-world experience \(and therefore value\)
* **Time from code contribution to codebase commit**
* **Time from bug report to bug being fixed in codebase**
* **Time from initial forum post to first response/answer**
  * These three related metrics above all track aspects of value: If you contribute, and it's
    [ignored](https://opensource.com/business/16/6/bad-practice-foss-projects-management)
    , then you'll find less value and possibly go elsewhere. The more we had here, the more confident we were of the result.
* **Location of community members**
  : Ability to see results of regional business decisions
* **Evolution of contributor age over time**
  : Enabling a constant flow of knowledge and experience from the old guard to the up-and-comers means there's always an up-to-date knowledge base \(value\) in the community.
* **Number of ignored/unanswered messages**
  : Super important for newcomers to get a first response, even if it's not the answer they were looking for.
* **Distribution **
  **&**
  ** evolution of commits across functional areas in the code**
  : This allowed us to make future business decisions based on which areas of Liferay were evolving the fastest.

After coming up with these and other metrics, it took about 4-6 months to implement the mechanics of extracting, combining, and consuming the data \(from our own forums, blogs, and special projects, as well as JIRA, GitHub, IRC, Stack Overflow, and a few others\). These metrics allowed us to more accurately gauge both the community value and business performance related to it over time. As you can imagine, there were a lot of challenges in using this disparate collection of data sources, such as normalization of identities and companies, removing duplicates, filtering spam, and many more.

### 

### **Who contributes?**

* Summarize the primary classifications of the primary contributors to your community.
* Divide these by the types of value they bring, primarily in terms of different skills.

### **How do they participate?**

* For each type of contributor that you just wrote down, also note how each interacts with your community to make those contributions. These should primarily be the processes and infrastructure they use to participate.

### **What do they deliver?**

* For each group, write down what value they bring in a practical and measurable form.



