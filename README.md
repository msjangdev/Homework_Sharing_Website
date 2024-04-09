# Homework_Sharing_Website

##DB create code
###groups
'''
CREATE TABLE `groups` (
	`group_id` TEXT NULL DEFAULT NULL COLLATE 'utf8mb4_general_ci',
	`group_name` TEXT NULL DEFAULT NULL COLLATE 'utf8mb4_general_ci',
	`group_pw` TEXT NULL DEFAULT NULL COLLATE 'utf8mb4_general_ci',
	`ban` TINYINT(3) UNSIGNED NOT NULL DEFAULT '0'
)
COLLATE='utf8mb4_general_ci'
ENGINE=InnoDB
;
'''

###items
'''
CREATE TABLE `items` (
	`group_id` TEXT NULL DEFAULT NULL COLLATE 'utf8mb4_general_ci',
	`item_id` TEXT NULL DEFAULT NULL COLLATE 'utf8mb4_general_ci',
	`deadline` DATE NULL DEFAULT NULL,
	`sub1` TEXT NULL DEFAULT NULL COLLATE 'utf8mb4_general_ci',
	`sub2` TEXT NULL DEFAULT NULL COLLATE 'utf8mb4_general_ci',
	`title` TEXT NULL DEFAULT NULL COLLATE 'utf8mb4_general_ci',
	`deleted` TINYINT(3) UNSIGNED NOT NULL DEFAULT '0',
	`creation_datetime` DATETIME NULL DEFAULT NULL,
	`creation_ip` TEXT NULL DEFAULT NULL COLLATE 'utf8mb4_general_ci'
)
COLLATE='utf8mb4_general_ci'
ENGINE=InnoDB
;
'''
