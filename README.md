# chroot-lab-gcp

This project demonstrates launching a small GCP VM; Isolates a process using the unshare and creating cgroups to assign and monitor system resources. The goal of this lab is to solidify the understanding of how docker uses namespaces and cgroups under the hood.

## 🛠️ Steps Covered

- Set up a GCP project and enabled billing
- Used `gcloud` CLI from Cloud Shell to create a Debian VM
- Creat a cgroup; Stress the machine and monitor the system resources.
- Explored filesystem isolation by entering the jail environment

## ✅ VM Specs

- Name: `chroot-lab-vm`
- Type: `e2-micro` (free tier eligible)
- Image: Debian 11
- Region: `us-central1-a`

## 🔁 Cleanup

To delete the VM when done:
```bash
gcloud compute instances delete chroot-lab-vm --zone=us-central1-a

