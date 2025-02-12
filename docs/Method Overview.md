## PyMonday Client Method Overview

This table presents a categorized list of all available client methods, grouped as **Getters**, **Setters**, or 
**Deleters** to indicate whether they retrieve, modify, or remove data. 

For more details and usage examples, refer to the following sections.

| Class            | Method Name                     | Method Type | Category | Created in Version |
|------------------|--------------------------------|-------------|----------|--------------------|
| *BaseClient*     | __async_post                   | Private     | -        | v2 (updated in v3)|
| *BaseClient*     | __column_task_handler          | Private     | -        | v2                |
| *BaseClient*     | __get_next_page                | Private     | -        | v2                |
| *BaseClient*     | __send_post_request            | Private     | -        | v2                |
| *BaseClient*     | __upload_file                  | Private     | -        | v2                |
| **Account**      | get_account_details            | Public      | Getter   | v2                |
| **Activity Log** | get_activity_logs             | Public      | Getter   | v3                |
| **Boards**       | get_all_boards                 | Public      | Getter   | v2                |
| **Boards**       | get_board_info                 | Public      | Getter   | v2                |
| **Boards**       | get_board_groups               | Public      | Getter   | v2                |
| **Boards**       | get_board_from_item            | Public      | Getter   | v2                |
| **Boards**       | get_board_views                | Public      | Getter   | v3                |
| **Boards**       | create_board                   | Public      | Setter   | v2                |
| **Boards**       | update_board_description       | Public      | Setter   | v2                |
| **Boards**       | archive_board                  | Public      | Deleter  | v2                |
| **Boards**       | duplicate_board                | Public      | Setter   | v3                |
| **Boards**       | delete_board                   | Public      | Deleter  | v2                |
| **Columns**      | get_column_metadata            | Public      | Getter   | v3                |
| **Columns**      | column_id_formatter            | Static      | Getter   | v2                |
| **Columns**      | create_column                  | Public      | Setter   | v3                |
| **Columns**      | change_column_values           | Public      | Setter   | v2                |
| **Columns**      | change_column_title            | Public      | Setter   | v3                |
| **Columns**      | clear_column                   | Public      | Deleter  | v3                |
| **Doc Blocks**   | fetch_doc_blocks               | Public      | Getter   | v3                |
| **Doc Blocks**   | create_doc_block               | Public      | Setter   | v3                |
| **Doc Blocks**   | update_doc_block               | Public      | Setter   | v3                |
| **Doc Blocks**   | delete_doc_block               | Public      | Deleter  | v3                |
| **Docs**         | fetch_docs                     | Public      | Getter   | v3                |
| **Docs**         | create_doc                     | Public      | Setter   | v3                |
| **Files**        | get_assets                     | Public      | Getter   | v2                |
| **Files**        | upload_file_to_column          | Public      | Setter   | v2                |
| **Files**        | add_file_to_update             | Public      | Setter   | v2                |
| **Folders**      | get_folders                    | Public      | Getter   | v2                |
| **Folders**      | create_folder                  | Public      | Setter   | v2                |
| **Folders**      | update_folder                  | Public      | Setter   | v2                |
| **Folders**      | delete_folder                  | Public      | Deleter  | v2                |
| **Groups**       | create_group                   | Public      | Setter   | v2                |
| **Groups**       | move_item_to_group             | Public      | Setter   | v2                |
| **Groups**       | update_group                   | Public      | Setter   | v3                |
| **Groups**       | duplicate_group                | Public      | Setter   | v3                |
| **Groups**       | is_group_empty                 | Public      | Getter   | v3                |
| **Groups**       | archive_group                  | Public      | Deleter  | v2                |
| **Groups**       | delete_group                   | Public      | Deleter  | v2                |
| **Items**        | get_item_ids_from_group        | Public      | Getter   | v2                |
| **Items**        | get_items_page_from_group      | Public      | Getter   | v2                |
| **Items**        | get_items_from_column          | Public      | Getter   | v2                |
| **Items**        | get_items_with_status          | Public      | Getter   | v2                |
| **Items**        | get_items_page_between_dates   | Public      | Getter   | v2                |
| **Items**        | get_items_page_between_date    | Public      | Getter   | v2                |
| **Items**        | get_item_ids_between_dates     | Public      | Getter   | v2                |
| **Items**        | get_item_ids_between_date      | Public      | Getter   | v2                |
| **Items**        | get_item_columns               | Public      | Getter   | v2                |
| **Items**        | get_items_by_column_values     | Public      | Getter   | v3                |
| **Items**        | create_item                    | Public      | Setter   | v2                |
| **Items**        | create_item_with_column_values | Public      | Setter   | v2                |
| **Items**        | archive_item                   | Public      | Deleter  | v3                |
| **Items**        | duplicate_item                 | Public      | Setter   | v3                |
| **Items**        | move_item_to_board             | Public      | Setter   | v3                |
| **Items**        | delete_item                    | Public      | Deleter  | v2                |
| **Notifications**| create_notification            | Public      | Setter   | v2                |
| **Subitems**     | get_subitems                   | Public      | Getter   | v2                |
| **Subitems**     | get_subitem_names              | Public      | Getter   | v2                |
| **Subitems**     | get_subitem_info               | Public      | Getter   | v2                |
| **Subitems**     | create_subitem                 | Public      | Setter   | v2                |
| **Tags**         | create_or_get_tag              | Public      | Setter   | v3                |
| **Teams**        | get_teams                      | Public      | Getter   | v2                |
| **Teams**        | get_team_members               | Public      | Getter   | v2                |
| **Updates**      | get_item_updates               | Public      | Getter   | v2                |
| **Updates**      | create_update                  | Public      | Setter   | v2                |
| **Updates**      | create_reply                   | Public      | Setter   | v2                |
| **Updates**      | clear_updates                  | Public      | Deleter  | v2                |
| **Updates**      | delete_update                  | Public      | Deleter  | v2                |
| **Users**        | get_all_users                  | Public      | Getter   | v2                |
| **Users**        | get_user_info                  | Public      | Getter   | v2                |
| **Users**        | add_user_to_board              | Public      | Setter   | v2                |
| **Users**        | remove_user_from_board         | Public      | Deleter  | v2                |
| **Workspaces**   | get_workspaces                 | Public      | Getter   | v2                |
| **Workspaces**   | create_workspace               | Public      | Setter   | v3                |
| **Workspaces**   | add_users_to_workspace         | Public      | Setter   | v3                |
| **Workspaces**   | add_teams_to_workspace         | Public      | Setter   | v3                |
| **Workspaces**   | update_workspace               | Public      | Setter   | v3                |
| **Workspaces**   | delete_workspace               | Public      | Deleter  | v3                |
| **Workspaces**   | delete_users_from_workspace    | Public      | Deleter  | v3                |
| **Workspaces**   | delete_teams_from_workspace    | Public      | Deleter  | v3                |


