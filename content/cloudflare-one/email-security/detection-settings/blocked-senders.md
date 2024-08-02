---
title: Blocked senders
pcx_content_type: how-to
weight: 2
---

# Add a blocked sender

Email Security marks all messages from these senders with a [disposition](/cloudflare-one/email-security/reference/dispositions-and-attributes/).

To configure blocked senders:

1. Log in to the [Cloudflare dashboard](https://dash.cloudflare.com/).
2. Select **Email Security**.
3. Select **Settings**, go to **Detection settings** > **Blocked senders**.
4. On the **Detection settings** page, select **+ Add a sender**.
5. Select the **Input method**: Choose between **Manual input**, and **Upload blocked sender list**:
     - **Manual input**:
        - **Sender type**:
             - **Email addresses**: Must be a valid email.
             - **IP addresses**: Can only be IPv4. IPv6 and CIDR are invalid entries.
             - **Domains**: Must be a valid domain.
             - **Regular expressions**: Must be valid Java expressions. Regular expressions are matched with fields related to the sender email address (envelope from, header from, reply-to), the originating IP address, and the server name for the email.
         - **Notes**: Provide additional information about the blocked sender policy.
   - **Upload blocked sender list**: Upload a file no larger than 150 KB. The file cannot contain other fields, and the first row must be a header row.
6. Select **Save**.
   
## Export blocked senders

To export a list of blocked senders:

1. On the **Detection settings** page, select the blocked senders you want to export.
2. Select **Action**.
3. Select **Export to CSV**.

## Edit a blocked sender

To edit a blocked sender:

1. On the **Detection settings** page, select the blocked sender you want to edit.
2. Select the three dots > **Edit**.
3. Edit the blocked sender.
4. Select **Save**.

## Delete a blocked sender

To delete a blocked sender:

1. On the **Detection settings** page, select the blocked sender you want to delete.
2. Select the three dots > **Delete**.
3. On the pop up message, select **Delete**.

To delete multiple blocked senders at once:

1. On the **Detection settings** page, under **Blocked senders**, select the senders you want to delete.
2. Select **Action**
3. Select **Delete**.