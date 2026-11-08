# Serverless - Processing orders with SQS and SNS

> Serverless order processing.

A hands-on workshop from the [AWS First Cloud Journey](https://github.com/vanhoangkha/aws-first-cloud-journey) series, available in English and Vietnamese.

**Read the workshop online:** https://vanhoangkha.github.io/000083-Orderbook/

## Overview

In the workshop 6 of this series, we will process user orders using Amazon SQS and SNS. When a user places an order, the order will be sent to the queue and SNS will notify the admin about the new order. Admin has the right to view all orders and process or delete them.

Amazon Simple Queue Service (Amazon SQS) offers a secure, durable, and available hosted queue that lets you integrate and decouple distributed software systems and components. It can scale independently from our application. It provides a generic web services API that you can access using any programming language that the AWS SDK supports.

## Workshop contents

1. Preparation
2. Create queue and SNS topic
   - Create queue
   - Create SNS topic
3. Create API and Lambda function
   - Create Lambda function
   - Create APIs
4. Test web operation
5. Clean up

## Prerequisites

- An AWS account with permissions to create the resources used in the labs
- Basic familiarity with the AWS Management Console
- [Hugo](https://gohugo.io/installation/) (extended edition) if you want to run the site locally

## Run locally

```bash
git clone https://github.com/vanhoangkha/000083-Orderbook.git
cd 000083-Orderbook
hugo server
```

Then open http://localhost:1313 in your browser.

## Repository structure

| Path | Purpose |
| --- | --- |
| `content/` | Workshop pages (`*.md` English, `*.vi.md` Vietnamese) |
| `static/` | Images and other static assets |
| `layouts/` | Hugo layout overrides |
| `themes/` | Hugo theme |
| `config.toml` | Site configuration |

## Cost and cleanup

The labs create AWS resources that may incur charges. Complete the **Clean up** chapter when you finish to remove them.

## Contributing

Contributions are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md).

To report a security issue, see [SECURITY.md](SECURITY.md).

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE).
