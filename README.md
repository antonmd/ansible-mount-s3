## Usage:

Start the playbook with the command:

```
ansible-playbook mount-s3.yml -e "bucket_name=mybucket mount_folder=/mnt/mybucket"
```

Replace mybucket with the name of the bucket to mount and /mnt/mybucket with the name of the directory to mount to

It is assumed that a service account with access to the bucket is bound to the virtual machine.

The fast fuse driver developed by Yandex is used.

Instruction from Yandex on the basis of which the playbook was created: https://cloud.yandex.ru/docs/storage/tools/geesefs.