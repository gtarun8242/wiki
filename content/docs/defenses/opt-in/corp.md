+++
title = "Cross-Origin-Resource-Policy"
description = ""
date = "2020-07-21"
category = "defenses"
menu = "main"
+++


## Explanation

Cross-Origin-Resource-Policy (CORP) response header is a complement of [Cross-Origin Read Blocking]({{< ref "../browser-intrinsic/corb.md" >}}) (CORB). CORP allows applications to **opt into the protection** for resources that might not be covered automatically by CORB[^1]. Applications can define which origins are allowed to read their resources.

If an application sets a certain resource CORP Header as `same-site`, an attacker is incapable of reading that resource because it's in a different origin.

[^1]: Cross-Origin Resource Policy (CORP), [link](https://developer.mozilla.org/en-US/docs/Web/HTTP/Cross-Origin_Resource_Policy_(CORP))