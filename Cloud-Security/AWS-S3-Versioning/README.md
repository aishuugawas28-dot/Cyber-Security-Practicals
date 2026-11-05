# AWS S3 Bucket Versioning Practical

## Objective
Enable S3 bucket versioning, upload an object, and inspect the available object versions.

## AWS Service
- Amazon S3
- Region shown: Asia Pacific (Mumbai), `ap-south-1`

## Practical Steps
1. Create an S3 general-purpose bucket.
2. Open the bucket's **Properties** tab.
3. Enable **Bucket Versioning** and save the change.
4. Upload a text object named `version-test.txt`.
5. Open the object's **Versions** tab and verify that object versions are listed.

## Evidence Included
- `01-S3-Bucket-Created.png` – S3 bucket list.
- `02-Versioning-Enabled.png` – Bucket Versioning shown as Enabled.
- `03-File-Upload-Success.png` – Successful upload of `version-test.txt`.
- `04-S3-Object-Versions.png` – Versions tab showing two object versions.

## Observation
The screenshots show Bucket Versioning enabled and two versions of `version-test.txt`; one is marked as the current version.

## Screenshot Label Note
The visible name “Manaswi” was replaced with “Aishwarya” in these presentation copies as requested. The actual bucket name in AWS may still differ. Make sure the final submission accurately reflects the resources in your own AWS account.

## Disclaimer
For educational use. Avoid publishing AWS account identifiers or other personal information in public repositories.
