![N|Solid](https://www.ncsc.gov.uk/global/logos/logo.png)
 
# MailCheck
MailCheck is the [National Cyber Security Centre's](http://www.ncsc.gov.uk/) tooling to test and report on email security for a large number of UK public sector domains.
 
MailCheck processes aggregate DMARC reports for UK public sector organisations and tests the configuration of anti-spoofing controls and support for TLS to encrypt email over SMTP. These tests will be used to help track adoption of the UK government's [email security standard](https://www.gov.uk/guidance/securing-government-email) by the public sector.
 
For an introduction to DMARC and other anti-spoofing controls there is a [good introduction on GOV.UK](https://www.gov.uk/government/publications/email-security-standards/domain-based-message-authentication-reporting-and-conformance-dmarc).
 
## Public repositories
The NCSC has released the core parts of the Mail Check application code, these are broadly responsible for:

- Processing DMARC reports 
- Verifying email related DNS records
- Verifying secure mail server configuration


- **AggregateReport** the Mail Check AggregateReport Microservice is responsible for processing DMARC reports. The service also "aggregates" this data in useful formats which are then fed to the front-end to be displayed.
https://github.com/ukncsc/MailCheck.Public.AggregateReport

- **Dkim** the Mail Check Dkim Microservice is responsible for polling DKIM records for a domain.
https://github.com/ukncsc/MailCheck.Public.Dkim

- **DMARC** the Mail Check DMARC Microservice is responsible for polling DMARC records for a domain.
https://github.com/ukncsc/MailCheck.Public.Dmarc

- **Mx** the Mail Check Mx Microservice is responsible for polling MX records for a domain and verifying TLS configuration. Polled records are then evaluated and saved.
https://github.com/ukncsc/MailCheck.Public.Mx

- **SPF** the Mail Check SPF Microservice is responsible for polling SPF records for a domain.
https://github.com/ukncsc/MailCheck.Public.Spf

- **TlsRpt** the Mail Check TlsRpt Microservice is responsible for polling TlsRpt records for a domain
https://github.com/ukncsc/MailCheck.Public.TlsRpt

- **MtaSts** the Mail Check MtaSts Microservice is responsible for polling MtaSts records for a domain
https://github.com/ukncsc/MailCheck.Public.MtaSts

- **Insights** the Mail Check Insights Microservice is responsible for interpreting DMARC aggregate report data
https://github.com/ukncsc/MailCheck.Public.Insights

- **EmailSecurity** the Mail Check EmailSecurity Microservice is responsible for merging outputs of other microservices
https://github.com/ukncsc/MailCheck.Public.EmailSecurity

- **DomainStatus** the Mail Check DomainStatus Microservice is responsible for summarising the test results of other microservices
https://github.com/ukncsc/MailCheck.Public.DomainStatus

- **Scheduler** the Mail Check Scheduler Microservice is responsible for scheduling tests in other microservices
https://github.com/ukncsc/MailCheck.Public.Scheduler

- **Common** the Mail Check Common Library contains various utilitiy, contract and common code
https://github.com/ukncsc/MailCheck.Public.Common

- **Frontend** the Mail Check Frontend application is the react frontend user interface to Mail Check
https://github.com/ukncsc/MailCheck.Public.Frontend


## Contributing
If you'd like to contribute please follow these steps:

1. Sign the [GCHQ Contributor Licence Agreement](https://github.com/gchq/Gaffer/wiki/GCHQ-OSS-Contributor-License-Agreement-V1.0).
2. Push your changes to your fork.
3. Submit a pull request.
