# linode-firewall-operator-rule
Linode Firewall Rule for Linode Firewall Operator

The linode firewall operator allows us to apply linode firewall rules to each node on the linode Kubernetes Engine (LKE) cluster. When the node is created, deleted, and recycled, the Operator automatically applies the firewall rule to the node in the cluster. The following is an excellent repository.
https://github.com/gangyi89/deploy-linode-operator

This firewall rule is effective when you want to drop packets by default. Linode Firewall Operator internally uses some ports and protocols. A firewall-rules-sample.json is a sample JSON rule for the Linode firewall ID.

You can call the following Linode API to update your firewall rule.
https://techdocs.akamai.com/linode-api/reference/put-firewall-rules
