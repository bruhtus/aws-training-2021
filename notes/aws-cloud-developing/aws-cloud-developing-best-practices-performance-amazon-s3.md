# When optimizing Amazon S3 request performance:

## Avoid unnecessary requests

- For example, if your code uses a particular S3 bucket, you don't want to check every time you make a request to see whether that bucket exists because it's an extra unnecessary request. Instead, have an if-else statement (for example) so that if you get a 400-series `NoSuchBucket` error, your code can then create that bucket as part of the request.
- Set the object metadate before you upload the object.
- Cache the bucket and key names if your application design allows it.

## Use as many prefixes as you need in parallel to achieve the required request rate throughput

Amazon S3 automatically scales high request rate.

For example: <br>
Your application can achieve at least 3500 PUT, POST, or DELETE and 5500 GET requests per second per prefix in a bucket.

There are no limits to the number of prefixes in a bucket. It is simple to increase your read or write performance exponentially.

For example: <br>
If you create 10 prefixes in an Amazon S3 bucket to parallelize reads, you could scale your read performance to 55000 read requests per second.

# To reduce network latency

- Select a Region for the bucket that is close to your users, if possible. You will also need to consider other factors, such as legal restrictions and cost.
- Consider compressing data to reduce the size of data that is transferred.
- Use a content delivery network (CDN) such as Amazon CloudFront to distribute content with low latency and high data transfer speeds.
