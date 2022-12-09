# Tornado S3 Sync 🌪️
Welcome to the easiest way to get your local files to your favorite Amazon S3 bucket. 

## Requirements
Below you'll find a list of requirements you'll need to get started with Tornado S3 Sync.
- [MacOS Ventura `v13.0+`](https://www.apple.com/macos/ventura/)
- An [Amazon Web Services (AWS)](https://console.aws.amazon.com) Account
- An [Amazon S3 Bucket](https://docs.aws.amazon.com/AmazonS3/latest/userguide/create-bucket-overview.html)
- An IAM User with at _least_ the following permissions:
    - `s3:ListBucket`
    - `s3:PutObject`
    - `s3:GetObject`

## Frequently Asked Questions

### How do I get started?
Getting started with Tornado S3 Sync is super simple. Just follow the steps below:

1. Download the latest version of Tornado S3 Sync from the MacOS App Store.
1. Open Tornado S3 Sync
1. Click the Tornado S3 Sync icon in the menu bar, and select `⚙️ Settings`
1. Navigate to the `AWS` tab of the settings window, and enter your credentials under `🔐 IAM Settings`. **Close Tornado S3 Sync after entering your credentials.**.
1. Re-open Tornado S3 Sync, and navigate back to the `AWS` tab of the settings window. Click the `S3 Bucket` dropdown picker under `🪣 S3 Bucket Settings` and select the bucket you'd like to sync with. **Please note, your `S3 Bucket Region` must match the region of your bucket.**
1. Enter the full bucket path where you would like your local files to end up in the `Bucket Path` text field.
1. Navigate to the `Local` tab of the settings window, and click the `Select Sync Directory` button. Select the directory you'd like to sync with your S3 bucket.
1. Enter the frequency in which you'd like your files to sync (in seconds)
1. Set your notification preferences
1. Close the settings window, and click the Tornado S3 Sync icon in the menu bar, and click `🔁 Sync Now`

Once you've confirmed your files are ending up in your S3 bucket, you're all set! 🎉

### My files aren't syncing!
If your files aren't syncing, there are a few things you can check to make sure everything is configured correctly.
* Verify your IAM User has the correct permissions
* Verify your `S3 Bucket Region` matches the region of your bucket
* Verify your `Bucket Path` is correct
* Verify your `Sync Directory` is correct
* Verify you've clicked "Sync Now" after making changes to your settings to trigger the sync timer

### I keep having to select my local directory!
Unfortunately, due to the nature of MacOS' filesystem, we're unable to persist the directory you've on app restarts. We're working on a fix for this, but for now, you'll have to select your directory every time you open Tornado S3 Sync.

Fortunately, however, once you've set your local path, as long as you don't close Tornado S3 Sync, you won't have to select your directory again! 