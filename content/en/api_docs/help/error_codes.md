---
title: Error Codes
---

| Code | Meaning | Resolution |
| :--- | :--- | :--- |
| **Parameter Errors** | | |
| 40000 | Required parameters missing or format invalid | Check parameter names and types |
| 40001 | Requested resource (e.g., file, project) validation failed | Check resource ID validation |
| 40002 | Parameter cannot be empty | Provide required parameter |
| 40003 | Parameter is empty | Provide required parameter |
| 40004 | Callback status must be 'success' or 'fail' | Check callback parameters |
| 40005 | Callback origin_type not supported | Check callback parameters |
| 40007 | Uploaded file type not supported | Upload allowed formats only |
| 40008 | Base64 content contains invalid characters | Check Base64 string |
| 40010 | User ID exceeds length limit | Shorten ID length |
| 40020 | Project ID format invalid | Check ID format |
| 40021 | Project does not exist or has been revoked | Verify Project ID |
| 40030 | API Key name too long | Modify name |
| **Authentication & Permission Errors** | | |
| 40100 | Not logged in or session expired | Please log in |
| 40101 | No permission to operate this resource | Verify account permissions |
| 40102 | Username or account already exists | Use a different username |
| 40103 | Specified user does not exist | Check username |
| 40110 | Verification code expired | Request a new one |
| 40111 | Verification code error | Check and retry |
| 40112 | Too many verification code errors, locked for 10 min | Retry later |
| 40113 | Duplicate verification code requests within 60s | Retry later |
| 40114 | Daily verification code limit exceeded | Try again tomorrow |
| 40130 | Request missing API Key | Add Header |
| 40132 | API Key invalid or disabled | Check Key status |
| **Quota & Rate Limit Errors** | | |
| 40300 | API call frequency limit exceeded | <a href="/memos_cloud/limit#_4-obtaining-more-quota" target="_blank">Get more quota</a> |
| 40301 | Chat Request Token total limit exceeded | <a href="/memos_cloud/limit#_4-obtaining-more-quota" target="_blank">Get more quota</a> |
| 40302 | Chat Response Token total limit exceeded | <a href="/memos_cloud/limit#_4-obtaining-more-quota" target="_blank">Get more quota</a> |
| 40303 | Single chat length exceeds model limit | Reduce input/output length |
| 40304 | Account total API call limit reached | <a href="/memos_cloud/limit#_4-obtaining-more-quota" target="_blank">Get more quota</a> |
| 40305 | Input content exceeds single Token limit | Reduce input |
| 40307 | Memory for deletion does not exist | Refresh or check ID |
| **System & Service Errors** | | |
| 50000 | Internal server error | Contact support |
| 50004 | Memory service temporarily unavailable | Retry later |
| 50005 | Search service temporarily unavailable | Retry later |
| 50011 | SSE connection failed | Check network |
| **Knowledge Base & File Errors** | | |
| 50100 | File ID does not exist | Confirm file is not deleted |
| 50103 | Knowledge base file count limit exceeded | Clean up or upgrade |
| 50104 | Single file size limit exceeded | Compress file |
| 50105 | Knowledge base total capacity limit exceeded | Clean up unneeded documents |
| 50106 | Single file exceeds 100MB | Ensure < 100MB |
| 50107 | File format corrupted or mismatch | Check file |
| 50108 | Knowledge base capacity reached version limit | Clean up unneeded documents |
| 50110 | File does not belong to current knowledge base | Check relationship |
| 50120 | Knowledge base ID does not exist | Check ID |
| 50121 | Knowledge base count limit exceeded | Consider reusing knowledge bases |
| 50123 | Knowledge base does not belong to current project | Switch project |