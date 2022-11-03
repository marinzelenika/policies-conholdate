---
head_name: "Metered Licensing FAQ"
page_title: "Metered Licensing FAQ - Purchase - conholdate.com"
description: "Metered licenses are a form of pay as you use licensing for .NET and Java. Instead of paying upfront as with a standard license, you will pay for your usage monthly."
base_url: ""
---
{{< rightPanel >}}
{{< start-content >}}
1. [What are Metered Licenses and how do they work compared to other license types?](/faqs/licensing/metered#1)
2. [What are the advantages of Metered License types?](/faqs/licensing/metered#2)
3. [How does billing work and when does the billing period begin?](/faqs/licensing/metered#3) 
4. [What is the cost of use and how do I pay?](/faqs/licensing/metered#4)
5. [How are Metered Licenses activated and how do you monitor/track the usage of my application?](/faqs/licensing/metered#5)
6. [Are we able to easily see via the product how many credits have been used in a given usage period?](/faqs/licensing/metered#6)
7. [Can I upgrade/downgrade between metered and unmetered license types?](/faqs/licensing/metered#7)
8. [What provisions do you have in place to ensure your servers for the licensing infrastructure are available?](/faqs/licensing/metered#8)
9. [With regard to data protection and our customer files, can you clarify what data is sent to your servers?](/faqs/licensing/metered#9)
10. [What is the pricing?](/faqs/licensing/metered#10)
11. [How do I purchase a Metered License?](/faqs/licensing/metered#11)
12. [Can I test the product before signing up for a Metered License?](/faqs/licensing/metered#12)  

&nbsp;  
##### **1. What are Metered licenses and how do they work compared to other license types?**
{{< faqs 2 >}} Metered licenses are a form of "pay as you use" licensing for .NET and Java. When you purchase a Metered License you will receive a Public/Private Key pair to be set in your code instead of the usual license file; and instead of paying 'upfront' as with a standard license, you will pay for your usage monthly. When you use a Metered License your usage is recorded locally and regularly reported back to our servers, you are then billed monthly for what you use.  So long as you pay your monthly bill you will have equivalent features to a full license and be able to access to all updates and new versions of the product. Metered Licenses are the only license types that are suitable for SaaS products which target developers or any product which needs to provide an API for developers which uses Conholdate functionality.

Unmetered license types (Developer Small Business, Developer OEM, Site Small Business, Site OEM) are priced based on the number of developers using the product and the number of locations that end user software are deployed to.  The full cost of the license must be paid before the license is released (unless you are choosing an [installment plan](/policies/installment-plans)). The license includes a one year subscription to access to updates and new versions of the product. These license types do not support end user software that have an API for other developers to use.  

&nbsp;  
##### **2. What are the advantages of Metered licenses?**
{{< faqs 3 >}} Metered licenses combines the benefits of self-hosting our .NET and Java products with the flexibility of using a cloud service.

- Pay monthly for what you use instead of all upfront.
- Documents are processed on your own servers and are never transmitted over the internet.
- Add as many developers and locations using our APIs as you want.  The monthly charge is only based on usage.
- Access all of our .NET and Java products using the one license (public/private key pair).
- Create applications that provide an API for other developers to use. 

&nbsp;  
##### **3. How does billing work and when does the billing period begin?**
{{< faqs 4 >}} Your usage of the product is reported to our servers at regular intervals and we will invoice you monthly based on the number of open/save operations processed by our APIs. One 'credit' is counted each time you perform an open or a save operation on a document and you are billed for the total number of credits.

The billing period begins on the date you sign up so, for example, if you were to sign up on the 18th of the month then your billing period will run from 18th through to the 17th of the following month.

&nbsp;  
##### **4. What is the cost of Metered licenses and how do I pay?**
{{< faqs 5 >}} A list of our prices is available, along with an interactive pricing guide for you to calculate your expected monthly cost, is available [on the Metered pricing page](/pricing/total/net/metered-oem). Both the Metered Small Business and Metered OEM license types are billed at the same rate, but only Metered OEM customers have access to [Enterprise Support](https://helpdesk.conholdate.com/kb/faq/3-Enterprise-Support-Key-Benefits-Conditions).

Payment by credit card is preferred however payment by bank transfer is possible. [Contact a member of our sales team](https://about.conholdate.com/contact/) and they will be glad to assist you.  

&nbsp;  
##### **5. How are Metered licenses activated and how do you monitor/track the usage of my application?**
{{< faqs 6 >}} After installing the product, sign up through our sales team for a metered license and you will be issued a key pair consisting of a public and private key which you use to activate the product via the API. This enables the product to run in production mode and your usage of the product is recorded and that information is routinely sent back to our servers. 

Usage is tracked by the number of open/save operations calls to our API from your application.  Each of these operations consumes 1 'credit'.

To activate the license refer to the [Metered licensing documentation](/faqs/licensing/metered/how-to-use) for each product. 

&nbsp;  
##### **6. Are we able to easily see via the product how many credits have been reported to Conholdate?**
{{< faqs 7 >}} It is easy to check your usage via the API. Refer to [the documentation](/faqs/licensing/metered/how-to-use) for further instructions. 

_Note: Your local usage is only reported to Conholdate intermittently, usually once per hour, so the usage amount returned by the GetConsumptionQuantity() API call may reflect this delay._  

&nbsp;  
##### **7. Can I upgrade/downgrade between Metered and Unmetered license types?**
{{< faqs 8 >}} You can upgrade from an unmetered license type to a Metered license within the first 90 days of purchase. The payment from your unmetered license is credited to the balance of your account and deducted from your monthly bill until used up. We do not offer downgrades from a Metered license to an unmetered license.  

&nbsp;  
##### **8. What provisions do you have in place to ensure your servers for the licensing infrastructure are available?**
{{< faqs 9 >}} Our servers are monitored actively to ensure 24/7 uptime.  If your systems can’t reach ours, the billing mechanism on your side will retry hourly for 24 hours before reverting to a ‘trial’ state.
 
As long as your application connects to our licensing servers at least once every 24 hours your license will work correctly.  It is therefore important to ensure any firewalls are configured to allow communication with our licensing server.  

&nbsp;  
##### **9. With regard to data protection and our customer files, can you clarify what data is sent to your servers?**
{{< faqs 10 >}} Purely usage information (number of operations performed and total file size processed) is sent to our servers, no document data or your customer data is sent to us.  

&nbsp;  
##### **10. What is the pricing?**
{{< faqs 11 >}} Check out pricing using the interactive guide available for [Metered Small Business](/pricing/total/net/metered-small-business) and [Metered OEM](/pricing/total/net/metered-oem). Note that this pricing covers files up to 20MB in size. For large files over that size, every 20MB file chunk, after the first 20MB, will incur an additional one API call surcharge.

&nbsp;  
##### **11. How do I purchase a Metered License?**
{{< faqs 12 >}} To purchase a Metered license head to [the purchase page](https://purchase.conholdate.com/buy). Our [payment methods](/policies/payment-methods) include credit card and bank transfer. For any questions [contact a member of our sales team](https://about.conholdate.com/contact/) who will be glad to assist you.  

&nbsp;  
##### **12. Can I test the product before signing up for a Metered License?**
{{< faqs 13 >}} Yes, you can [request a temporary license](/temporary-license) to fully test Conholdate products. This free temporary license is unmetered and is used for testing only. Once you are ready for a production license you can proceed to [purchase](https://purchase.conholdate.com/buy) a Metered license.  

&nbsp;  

{{< questions-start >}}
##### Questions?
If you have any questions or problems, please feel free to [contact our sales support](https://about.conholdate.com/contact/) who will be glad to assist.
{{< questions-end >}}

{{< end-content >}}