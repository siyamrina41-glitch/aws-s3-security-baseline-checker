# aws-s3-security-baseline-checker
“Read-only Python/Boto3 checks for one S3 bucket’s baseline security settings.
{
  "bucket": "aws-s3-security-baseline-checker",
  "scope": "One bucket; read-only checks",
  "checks": {
    "public_access_block": {
      "status": "PASS",
      "settings": {
        "BlockPublicAcls": true,
        "IgnorePublicAcls": true,
        "BlockPublicPolicy": true,
        "RestrictPublicBuckets": true
      }
    },
    "bucket_policy": {
      "status": "NO_BUCKET_POLICY",
      "code": "NoSuchBucketPolicy"
    },
    "bucket_acl": {
      "status": "PASS",
      "public_grants": []
    },
    "encryption": {
      "status": "PASS",
      "algorithms": [
        "AES256"
      ]
    },
    "versioning": {
      "status": "PASS",
      "versioning_status": "Enabled"
    }
  }
}
