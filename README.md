# ProxMox CT Install Guide

## Description
A full guide on installing a CT (Container) in the ProxMox environment.

---

## Program Walk-through

1. **Log into your ProxMox homepage.**

2. **Download a Container Template** from a trusted source or upload an existing template manually.

   - **If downloading a template**:
     - Click on the **ProxMox node** in the left sidebar.
     - Navigate to `local` → `CT Templates`.
     - Click **Templates**, choose a template from the list (e.g., `debian-12-standard_...`), then click **Download**.

   - **If uploading an existing template manually**:
     - Navigate to `local` → `CT Templates`.
     - Click **Upload**, then select your `.tar.gz` template file.

   - **Having issues with unsupported format types or disk volumes?**
     - Click the link below to learn more about supported storage types and volume configuration:
     - [ProxMox Post-Install Storage Guide](https://github.com/joshkoo1988/ProxMox-postinstall)

3. **Click "Create CT"** on the top-right corner of the ProxMox dashboard.

4. **Follow the prompts** and adjust settings according to your needs. Here's a breakdown of the steps:

   - **Page 1 – General**:
     - Set a CT ID and hostname.
     - Choose a strong password and (optionally) SSH public key.

   - **Page 2 – Template**:
     - Select the template you downloaded or uploaded.

   - **Page 3 – Root Disk**:
     - Choose storage location (e.g., `local-lvm`).
     - Set disk size according to your needs.

   - **Page 4 – CPU**:
     - Set the number of cores you want to allocate.

   - **Page 5 – Memory**:
     - Allocate RAM.
     - Optionally configure swap space.

   - **Page 6 – Network**:
     - Attach to a virtual bridge (e.g., `vmbr0`).
     - Assign IPv4 and/or IPv6 addresses, or set to DHCP.

   - **Page 7 – DNS**:
     - Configure DNS servers or use host settings.

   - **Page 8 – Confirm**:
     - Review your settings and click **Finish**.

5. **Start your CT** and begin configuring it as needed.

6. **Feel free to spin up more CTs** using the same steps!


