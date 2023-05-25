# openstack


**OpenStack Commands Cheat Sheet**

### Cheat Sheet

| Service | Command | Description |
| --- | --- | --- |
| **Block Storage (Cinder)** |
| | `openstack volume type list` | List all volume types |
| | `openstack volume type create <type_name>` | Create a new volume type |
| | `openstack volume type delete <type_id>` | Delete a volume type |
| | `openstack volume type set <type_id> --property <key=value>` | Set volume type properties |
| | `openstack volume type unset <type_id> --property <key>` | Unset volume type properties |
| | `openstack volume qos associate <qos_policy> <volume_type>` | Associate a QoS policy with a volume type |
| | `openstack volume qos disassociate <qos_policy> <volume_type>` | Disassociate a QoS policy from a volume type |
| | `openstack volume qos list` | List all QoS policies |
| | `openstack volume qos create <qos_name>` | Create a new QoS policy |
| | `openstack volume qos delete <qos_id>` | Delete a QoS policy |
| | `openstack volume qos set <qos_id> --property <key=value>` | Set QoS policy properties |
| | `openstack volume qos unset <qos_id> --property <key>` | Unset QoS policy properties |
| **Identity (Keystone)** |
| | `openstack project list` | List all projects |
| | `openstack project create <project_name>` | Create a new project |
| | `openstack project delete <project_id>` | Delete a project |
| | `openstack project set <project_id> --description <description>` | Set project description |
| | `openstack user list` | List all users |
| | `openstack user create --project <project_id> --password <password> <user_name>` | Create a new user |
| | `openstack user delete <user_id>` | Delete a user |
| | `openstack user set <user_id> --password <password>` | Change a user's password |
| | `openstack user add role --project <project_id> --user <user_id> <role_id>` | Add a role to a user in a project |
| | `openstack user remove role --project <project_id> --user <user_id> <role_id>` | Remove a role from a user in a project |
| | `openstack role list` | List all roles |
| | `openstack role create <role_name>` | Create a new role |
| | `openstack role delete <role_id>` | Delete a role |
| | `openstack token list` | List all tokens |
| | `openstack token issue` | Issue a new token |
| | `openstack token revoke <token_id>` | Revoke a token |
| | `openstack service list` | List all services |