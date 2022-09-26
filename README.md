# Fluent Bit Helm chart deployment

1) Create the IAM role with s3 bucket permissions and associate an IAM role with a service account 

2) Update the value in values.yaml file

3) Refer the references for the flluentbits to configure the s3 bucket settings to push the nodes systemd logs to s3 bucket.

4) Install the helm charts
        
        helm install fluent-bit ./fluent-bit -f ./fluent-bit/values.yaml --namespace logging

## References:

1) https://docs.aws.amazon.com/eks/latest/userguide/iam-roles-for-service-accounts.html

2) https://docs.fluentbit.io/manual/pipeline/inputs

3) https://docs.fluentbit.io/manual/pipeline/outputs