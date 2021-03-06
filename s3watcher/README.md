# S3 Watcher

An AWS Lambda to consume S3 events and ingest all images added to an
S3 bucket into the image-loader service.

See also [ftp-watcher](../ftp-watcher) for an FTP-based ingestion
process.

## Running locally

You need to have run the CloudFormation DEV stack.

Run the `setup.sh` script the first time to get your `config.json`
setup written to your ingestion bucket:

```
$ ./setup.sh
```

To run the lambda locally on a given image file, run:

```
$ ./run-local <some-image.jpg>
```
