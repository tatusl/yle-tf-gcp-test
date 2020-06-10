# yle-tf-gcp-test
PoC for handling Terraform remote state with yle_tf in GCP

See comments in [tf.yaml](https://github.com/tatusl/yle-tf-gcp-test/blob/master/tf.yaml)

With this setup we end up with the following state file hierarcy:

```
gsutil ls -r gs://gcp-tatusl-tf-state-test
gs://gcp-tatusl-tf-state-test/Users/:

gs://gcp-tatusl-tf-state-test/Users/tatu/:

gs://gcp-tatusl-tf-state-test/Users/tatu/git/:

gs://gcp-tatusl-tf-state-test/Users/tatu/git/misc/:

gs://gcp-tatusl-tf-state-test/Users/tatu/git/misc/yle-tf-gcp-test/:

gs://gcp-tatusl-tf-state-test/Users/tatu/git/misc/yle-tf-gcp-test/vm-bar/:
gs://gcp-tatusl-tf-state-test/Users/tatu/git/misc/yle-tf-gcp-test/vm-bar/default.tfstate

gs://gcp-tatusl-tf-state-test/Users/tatu/git/misc/yle-tf-gcp-test/vm-foo/:
gs://gcp-tatusl-tf-state-test/Users/tatu/git/misc/yle-tf-gcp-test/vm-foo/default.tfstate
```
