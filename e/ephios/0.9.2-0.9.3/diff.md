# Comparing `tmp/ephios-0.9.2.tar.gz` & `tmp/ephios-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ephios-0.9.2.tar", last modified: Sun Oct  3 16:46:24 2021, max compression
+gzip compressed data, was "ephios-0.9.3.tar", last modified: Sun Oct 10 21:33:52 2021, max compression
```

## Comparing `ephios-0.9.2.tar` & `ephios-0.9.3.tar`

### file list

```diff
@@ -1,452 +1,452 @@
--rw-r--r--   0        0        0        0 2021-03-21 23:27:39.730437 ephios-0.9.2/ephios/__init__.py
--rw-r--r--   0        0        0      647 2021-03-21 23:27:39.730437 ephios-0.9.2/ephios/__main__.py
--rw-r--r--   0        0        0      405 2021-03-21 23:27:39.730437 ephios-0.9.2/ephios/asgi.py
--rw-r--r--   0        0        0        0 2021-06-13 17:00:50.934458 ephios-0.9.2/ephios/core/__init__.py
--rw-r--r--   0        0        0      801 2021-07-20 21:40:27.739008 ephios-0.9.2/ephios/core/admin.py
--rw-r--r--   0        0        0      510 2021-06-13 17:00:50.934458 ephios-0.9.2/ephios/core/apps.py
--rw-r--r--   0        0        0     1883 2021-10-03 15:39:09.766769 ephios-0.9.2/ephios/core/calendar.py
--rw-r--r--   0        0        0     7772 2021-07-03 12:30:08.117715 ephios-0.9.2/ephios/core/consequences.py
--rw-r--r--   0        0        0      818 2021-08-03 14:26:37.836252 ephios-0.9.2/ephios/core/context.py
--rw-r--r--   0        0        0     4006 2021-10-03 15:39:09.766769 ephios-0.9.2/ephios/core/dynamic_preferences_registry.py
--rw-r--r--   0        0        0        0 2021-03-21 23:27:39.730437 ephios-0.9.2/ephios/core/forms/__init__.py
--rw-r--r--   0        0        0    12447 2021-10-03 15:39:09.767769 ephios-0.9.2/ephios/core/forms/events.py
--rw-r--r--   0        0        0    12434 2021-10-03 15:39:09.769769 ephios-0.9.2/ephios/core/forms/users.py
--rw-r--r--   0        0        0     1768 2021-05-04 20:28:57.897392 ephios-0.9.2/ephios/core/ical.py
--rw-r--r--   0        0        0     4961 2021-03-21 23:27:39.730437 ephios-0.9.2/ephios/core/migrations/0001_initial.py
--rw-r--r--   0        0        0    17507 2021-03-21 23:27:39.730437 ephios-0.9.2/ephios/core/migrations/0001_squashed_0008_auto_20210207_1309.py
--rw-r--r--   0        0        0    10162 2021-03-21 23:27:39.730437 ephios-0.9.2/ephios/core/migrations/0001_squashed_event_management_0007_auto_20210207_1309.py
--rw-r--r--   0        0        0      829 2021-03-21 23:27:39.730437 ephios-0.9.2/ephios/core/migrations/0002_initial_permissions.py
--rw-r--r--   0        0        0      643 2021-03-21 23:27:39.730437 ephios-0.9.2/ephios/core/migrations/0002_merge_content_type_20210208_0020.py
--rw-r--r--   0        0        0      623 2021-03-21 23:27:39.730437 ephios-0.9.2/ephios/core/migrations/0003_migrate_content_type_to_core_20210219_1642.py
--rw-r--r--   0        0        0     7348 2021-03-21 23:27:39.746063 ephios-0.9.2/ephios/core/migrations/0003_userprofile_calendar_token_squashed_0008_auto_20200925_1640.py
--rw-r--r--   0        0        0     1000 2021-03-21 23:27:39.746063 ephios-0.9.2/ephios/core/migrations/0004_auto_20201014_1648.py
--rw-r--r--   0        0        0     1152 2021-05-04 20:28:57.898392 ephios-0.9.2/ephios/core/migrations/0004_auto_20210305_1855.py
--rw-r--r--   0        0        0     3288 2021-03-21 23:27:39.746063 ephios-0.9.2/ephios/core/migrations/0005_auto_20210106_2219.py
--rw-r--r--   0        0        0      347 2021-05-04 20:28:57.898392 ephios-0.9.2/ephios/core/migrations/0005_remove_event_mail_updates.py
--rw-r--r--   0        0        0      881 2021-03-21 23:27:39.746063 ephios-0.9.2/ephios/core/migrations/0006_auto_20210109_2230.py
--rw-r--r--   0        0        0     1509 2021-05-04 20:28:57.898392 ephios-0.9.2/ephios/core/migrations/0006_notification.py
--rw-r--r--   0        0        0     1117 2021-03-21 23:27:39.746063 ephios-0.9.2/ephios/core/migrations/0007_auto_20210110_0050.py
--rw-r--r--   0        0        0      614 2021-05-04 20:28:57.899393 ephios-0.9.2/ephios/core/migrations/0007_auto_20210324_2101.py
--rw-r--r--   0        0        0      435 2021-05-04 20:28:57.899393 ephios-0.9.2/ephios/core/migrations/0007_eventtype_color.py
--rw-r--r--   0        0        0      971 2021-03-21 23:27:39.746063 ephios-0.9.2/ephios/core/migrations/0008_auto_20210207_1309.py
--rw-r--r--   0        0        0     2725 2021-05-04 20:28:57.900393 ephios-0.9.2/ephios/core/migrations/0008_auto_20210403_2348.py
--rw-r--r--   0        0        0     3475 2021-06-13 17:00:50.937460 ephios-0.9.2/ephios/core/migrations/0009_auto_20210528_2230.py
--rw-r--r--   0        0        0     1171 2021-07-20 21:40:27.739008 ephios-0.9.2/ephios/core/migrations/0010_placeholderparticipation.py
--rw-r--r--   0        0        0      871 2021-10-03 15:39:09.770769 ephios-0.9.2/ephios/core/migrations/0011_auto_20210903_1258.py
--rw-r--r--   0        0        0      404 2021-10-03 15:39:09.770769 ephios-0.9.2/ephios/core/migrations/0012_rename_included_qualifications_qualification_includes.py
--rw-r--r--   0        0        0        0 2021-03-21 23:27:39.746063 ephios-0.9.2/ephios/core/migrations/__init__.py
--rw-r--r--   0        0        0      317 2021-05-04 20:28:57.900393 ephios-0.9.2/ephios/core/models/__init__.py
--rw-r--r--   0        0        0    10395 2021-10-03 15:39:09.771770 ephios-0.9.2/ephios/core/models/events.py
--rw-r--r--   0        0        0    14788 2021-10-03 15:39:09.772770 ephios-0.9.2/ephios/core/models/users.py
--rw-r--r--   0        0        0     6945 2021-05-04 20:28:57.903394 ephios-0.9.2/ephios/core/pdf.py
--rw-r--r--   0        0        0     3369 2021-10-03 15:39:09.772770 ephios-0.9.2/ephios/core/plugins.py
--rw-r--r--   0        0        0        0 2021-05-04 20:28:57.904393 ephios-0.9.2/ephios/core/services/__init__.py
--rw-r--r--   0        0        0        0 2021-05-04 20:28:57.904393 ephios-0.9.2/ephios/core/services/notifications/__init__.py
--rw-r--r--   0        0        0     4064 2021-08-01 21:03:19.080402 ephios-0.9.2/ephios/core/services/notifications/backends.py
--rw-r--r--   0        0        0    16402 2021-08-01 21:03:19.081404 ephios-0.9.2/ephios/core/services/notifications/types.py
--rw-r--r--   0        0        0     1179 2021-05-04 20:28:57.906394 ephios-0.9.2/ephios/core/services/participation.py
--rw-r--r--   0        0        0     1066 2021-05-04 20:28:58.024911 ephios-0.9.2/ephios/core/services/password_reset.py
--rw-r--r--   0        0        0     4859 2021-05-04 20:28:57.907395 ephios-0.9.2/ephios/core/signals.py
--rw-r--r--   0        0        0       33 2021-03-21 23:27:39.746063 ephios-0.9.2/ephios/core/signup/__init__.py
--rw-r--r--   0        0        0     9476 2021-10-03 15:39:09.773770 ephios-0.9.2/ephios/core/signup/disposition.py
--rw-r--r--   0        0        0    21720 2021-10-03 15:39:09.774791 ephios-0.9.2/ephios/core/signup/methods.py
--rw-r--r--   0        0        0      333 2021-03-21 23:27:39.752569 ephios-0.9.2/ephios/core/templates/core/account_updated_email.html
--rw-r--r--   0        0        0      275 2021-03-21 23:27:39.752569 ephios-0.9.2/ephios/core/templates/core/disposition/base_participation.html
--rw-r--r--   0        0        0     5972 2021-07-20 21:40:27.742897 ephios-0.9.2/ephios/core/templates/core/disposition/disposition.html
--rw-r--r--   0        0        0     1672 2021-07-20 21:40:27.743888 ephios-0.9.2/ephios/core/templates/core/disposition/fragment_participation.html
--rw-r--r--   0        0        0     1543 2021-05-04 20:28:57.911395 ephios-0.9.2/ephios/core/templates/core/event_archive.html
--rw-r--r--   0        0        0      942 2021-03-21 23:27:39.752569 ephios-0.9.2/ephios/core/templates/core/event_bulk_delete.html
--rw-r--r--   0        0        0     1147 2021-08-03 14:26:37.840278 ephios-0.9.2/ephios/core/templates/core/event_calendar.html
--rw-r--r--   0        0        0      623 2021-05-04 20:28:57.911395 ephios-0.9.2/ephios/core/templates/core/event_confirm_delete.html
--rw-r--r--   0        0        0     2015 2021-07-03 12:30:08.121716 ephios-0.9.2/ephios/core/templates/core/event_copy.html
--rw-r--r--   0        0        0     6594 2021-10-03 15:39:09.775771 ephios-0.9.2/ephios/core/templates/core/event_detail.html
--rw-r--r--   0        0        0     2532 2021-07-03 12:30:08.123716 ephios-0.9.2/ephios/core/templates/core/event_form.html
--rw-r--r--   0        0        0     9456 2021-08-03 16:16:25.853938 ephios-0.9.2/ephios/core/templates/core/event_list.html
--rw-r--r--   0        0        0      587 2021-05-04 20:28:57.914397 ephios-0.9.2/ephios/core/templates/core/event_notification.html
--rw-r--r--   0        0        0      515 2021-03-21 23:27:39.752569 ephios-0.9.2/ephios/core/templates/core/eventtype_confirm_delete.html
--rw-r--r--   0        0        0      754 2021-07-03 12:30:08.124717 ephios-0.9.2/ephios/core/templates/core/eventtype_form.html
--rw-r--r--   0        0        0     1364 2021-07-03 12:30:08.124717 ephios-0.9.2/ephios/core/templates/core/eventtype_list.html
--rw-r--r--   0        0        0     1388 2021-05-04 20:28:57.915397 ephios-0.9.2/ephios/core/templates/core/fragments/approve_consequences.html
--rw-r--r--   0        0        0      177 2021-03-21 23:27:39.752569 ephios-0.9.2/ephios/core/templates/core/fragments/custom_date_input.html
--rw-r--r--   0        0        0      207 2021-07-03 12:30:08.125717 ephios-0.9.2/ephios/core/templates/core/fragments/custom_split_date_time_widget.html
--rw-r--r--   0        0        0      177 2021-03-21 23:27:39.752569 ephios-0.9.2/ephios/core/templates/core/fragments/custom_time_input.html
--rw-r--r--   0        0        0      430 2021-07-03 12:30:08.126717 ephios-0.9.2/ephios/core/templates/core/fragments/event_plugin_form.html
--rw-r--r--   0        0        0      699 2021-05-04 22:04:58.666611 ephios-0.9.2/ephios/core/templates/core/fragments/pending_consequences.html
--rw-r--r--   0        0        0     4405 2021-08-03 14:26:37.841272 ephios-0.9.2/ephios/core/templates/core/fragments/shift_box_big.html
--rw-r--r--   0        0        0     1270 2021-07-03 12:30:08.127720 ephios-0.9.2/ephios/core/templates/core/fragments/shift_box_small.html
--rw-r--r--   0        0        0      957 2021-08-03 16:16:25.854937 ephios-0.9.2/ephios/core/templates/core/fragments/signup_stats_indicator.html
--rw-r--r--   0        0        0      620 2021-03-21 23:27:39.752569 ephios-0.9.2/ephios/core/templates/core/group_confirm_delete.html
--rw-r--r--   0        0        0      660 2021-03-21 23:27:39.752569 ephios-0.9.2/ephios/core/templates/core/group_form.html
--rw-r--r--   0        0        0     1408 2021-07-03 12:30:08.128718 ephios-0.9.2/ephios/core/templates/core/group_list.html
--rw-r--r--   0        0        0     4308 2021-08-03 14:26:37.843282 ephios-0.9.2/ephios/core/templates/core/home.html
--rw-r--r--   0        0        0     2463 2021-08-03 14:26:37.843282 ephios-0.9.2/ephios/core/templates/core/logentry_list.html
--rw-r--r--   0        0        0      509 2021-05-04 20:28:58.021185 ephios-0.9.2/ephios/core/templates/core/mails/new_account_email.html
--rw-r--r--   0        0        0      536 2021-05-04 20:28:57.918396 ephios-0.9.2/ephios/core/templates/core/mails/new_event.html
--rw-r--r--   0        0        0     2016 2021-05-04 20:28:57.918396 ephios-0.9.2/ephios/core/templates/core/pagination.html
--rw-r--r--   0        0        0      316 2021-03-21 23:27:39.752569 ephios-0.9.2/ephios/core/templates/core/settings/general.html
--rw-r--r--   0        0        0      924 2021-07-03 12:30:08.130718 ephios-0.9.2/ephios/core/templates/core/settings/settings_base.html
--rw-r--r--   0        0        0      627 2021-05-04 20:28:57.919397 ephios-0.9.2/ephios/core/templates/core/shift_confirm_delete.html
--rw-r--r--   0        0        0     4045 2021-10-03 15:40:55.836260 ephios-0.9.2/ephios/core/templates/core/shift_form.html
--rw-r--r--   0        0        0      298 2021-07-03 12:30:08.132718 ephios-0.9.2/ephios/core/templates/core/userprofile_badges.html
--rw-r--r--   0        0        0      724 2021-03-21 23:27:39.752569 ephios-0.9.2/ephios/core/templates/core/userprofile_confirm_delete.html
--rw-r--r--   0        0        0      829 2021-05-04 20:28:57.920397 ephios-0.9.2/ephios/core/templates/core/userprofile_confirm_password_reset.html
--rw-r--r--   0        0        0     4847 2021-07-03 12:30:08.132718 ephios-0.9.2/ephios/core/templates/core/userprofile_detail.html
--rw-r--r--   0        0        0     5685 2021-10-03 15:39:09.776770 ephios-0.9.2/ephios/core/templates/core/userprofile_form.html
--rw-r--r--   0        0        0     2894 2021-07-03 12:30:08.134719 ephios-0.9.2/ephios/core/templates/core/userprofile_list.html
--rw-r--r--   0        0        0     1061 2021-05-04 20:28:57.923398 ephios-0.9.2/ephios/core/templates/core/userprofile_notifications.html
--rw-r--r--   0        0        0      300 2021-03-21 23:27:39.752569 ephios-0.9.2/ephios/core/templates/core/workinghour_request.html
--rw-r--r--   0        0        0        0 2021-03-21 23:27:39.752569 ephios-0.9.2/ephios/core/templatetags/__init__.py
--rw-r--r--   0        0        0     3751 2021-08-03 14:26:37.844273 ephios-0.9.2/ephios/core/templatetags/event_extras.py
--rw-r--r--   0        0        0      393 2021-05-04 20:28:57.924399 ephios-0.9.2/ephios/core/templatetags/param_replace.py
--rw-r--r--   0        0        0     2420 2021-08-03 14:26:37.845274 ephios-0.9.2/ephios/core/templatetags/user_extras.py
--rw-r--r--   0        0        0     6707 2021-10-03 15:39:09.777771 ephios-0.9.2/ephios/core/urls.py
--rw-r--r--   0        0        0        0 2021-03-21 23:27:39.768202 ephios-0.9.2/ephios/core/views/__init__.py
--rw-r--r--   0        0        0     9555 2021-10-03 15:39:09.777771 ephios-0.9.2/ephios/core/views/accounts.py
--rw-r--r--   0        0        0     1106 2021-05-04 20:28:57.926398 ephios-0.9.2/ephios/core/views/bulk.py
--rw-r--r--   0        0        0     1784 2021-07-03 12:30:08.136720 ephios-0.9.2/ephios/core/views/consequences.py
--rw-r--r--   0        0        0    14010 2021-08-03 16:16:25.855938 ephios-0.9.2/ephios/core/views/event.py
--rw-r--r--   0        0        0     3356 2021-07-03 12:30:08.138719 ephios-0.9.2/ephios/core/views/eventtype.py
--rw-r--r--   0        0        0     3810 2021-10-03 15:39:09.778771 ephios-0.9.2/ephios/core/views/log.py
--rw-r--r--   0        0        0     1227 2021-05-04 20:28:57.929401 ephios-0.9.2/ephios/core/views/pwa.py
--rw-r--r--   0        0        0     1796 2021-05-04 20:28:57.929401 ephios-0.9.2/ephios/core/views/settings.py
--rw-r--r--   0        0        0     7421 2021-10-03 16:45:48.485798 ephios-0.9.2/ephios/core/views/shift.py
--rw-r--r--   0        0        0     1099 2021-05-04 20:28:57.931400 ephios-0.9.2/ephios/core/views/signup.py
--rw-r--r--   0        0        0      607 2021-03-21 23:27:39.768202 ephios-0.9.2/ephios/core/widgets.py
--rw-r--r--   0        0        0        0 2021-06-13 17:00:50.940461 ephios-0.9.2/ephios/extra/__init__.py
--rw-r--r--   0        0        0      196 2021-06-13 17:00:50.940461 ephios-0.9.2/ephios/extra/apps.py
--rw-r--r--   0        0        0      638 2021-10-03 15:39:09.779773 ephios-0.9.2/ephios/extra/bootstrap.py
--rw-r--r--   0        0        0     1000 2021-05-04 20:28:57.931400 ephios-0.9.2/ephios/extra/colors.py
--rw-r--r--   0        0        0     1837 2021-10-03 15:39:09.780773 ephios-0.9.2/ephios/extra/crispy.py
--rw-r--r--   0        0        0      535 2021-10-03 15:39:09.780773 ephios-0.9.2/ephios/extra/fields.py
--rw-r--r--   0        0        0      868 2021-03-21 23:27:39.768202 ephios-0.9.2/ephios/extra/json.py
--rw-r--r--   0        0        0        0 2021-03-21 23:27:39.768202 ephios-0.9.2/ephios/extra/management/__init__.py
--rw-r--r--   0        0        0        0 2021-03-21 23:27:39.768202 ephios-0.9.2/ephios/extra/management/commands/__init__.py
--rw-r--r--   0        0        0     3524 2021-10-03 15:39:09.781773 ephios-0.9.2/ephios/extra/management/commands/devdata.py
--rw-r--r--   0        0        0      209 2021-05-04 20:28:57.931400 ephios-0.9.2/ephios/extra/management/commands/run_periodic.py
--rw-r--r--   0        0        0      238 2021-05-04 20:28:57.932401 ephios-0.9.2/ephios/extra/management/commands/send_notifications.py
--rw-r--r--   0        0        0     5219 2021-05-04 20:28:57.932401 ephios-0.9.2/ephios/extra/mixins.py
--rw-r--r--   0        0        0     3177 2021-10-03 15:39:09.781773 ephios-0.9.2/ephios/extra/permissions.py
--rw-r--r--   0        0        0      802 2021-10-03 15:39:09.782772 ephios-0.9.2/ephios/extra/preferences.py
--rw-r--r--   0        0        0        0 2021-03-21 23:27:39.768202 ephios-0.9.2/ephios/extra/signals.py
--rw-r--r--   0        0        0      494 2021-03-21 23:27:39.768202 ephios-0.9.2/ephios/extra/templatetags/bootstrap.py
--rw-r--r--   0        0        0      366 2021-03-21 23:27:39.768202 ephios-0.9.2/ephios/extra/templatetags/ephios_crispy.py
--rw-r--r--   0        0        0     1648 2021-03-21 23:27:39.768202 ephios-0.9.2/ephios/extra/templatetags/rich_text.py
--rw-r--r--   0        0        0      339 2021-03-22 14:23:39.771663 ephios-0.9.2/ephios/extra/templatetags/utils.py
--rw-r--r--   0        0        0      168 2021-05-04 20:28:57.934401 ephios-0.9.2/ephios/extra/utils.py
--rw-r--r--   0        0        0     1402 2021-10-03 15:39:09.783772 ephios-0.9.2/ephios/extra/widgets.py
--rw-r--r--   0        0        0    85486 2021-10-03 16:45:32.711461 ephios-0.9.2/ephios/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2021-06-13 17:00:50.941460 ephios-0.9.2/ephios/modellogging/__init__.py
--rw-r--r--   0        0        0      118 2021-05-04 20:28:57.937403 ephios-0.9.2/ephios/modellogging/admin.py
--rw-r--r--   0        0        0      109 2021-06-13 17:00:50.942046 ephios-0.9.2/ephios/modellogging/apps.py
--rw-r--r--   0        0        0     2975 2021-05-04 20:28:57.937403 ephios-0.9.2/ephios/modellogging/json.py
--rw-r--r--   0        0        0     6561 2021-05-04 20:28:57.938402 ephios-0.9.2/ephios/modellogging/log.py
--rw-r--r--   0        0        0      663 2021-05-04 20:28:57.938402 ephios-0.9.2/ephios/modellogging/middleware.py
--rw-r--r--   0        0        0     3442 2021-05-04 20:28:57.939402 ephios-0.9.2/ephios/modellogging/migrations/0001_initial.py
--rw-r--r--   0        0        0     1629 2021-05-04 20:28:57.939402 ephios-0.9.2/ephios/modellogging/migrations/0002_auto_20210403_2348.py
--rw-r--r--   0        0        0      500 2021-06-13 17:00:50.942046 ephios-0.9.2/ephios/modellogging/migrations/0003_alter_logentry_id.py
--rw-r--r--   0        0        0      761 2021-07-03 12:30:08.139721 ephios-0.9.2/ephios/modellogging/migrations/0004_alter_logentry_user.py
--rw-r--r--   0        0        0        0 2021-05-04 20:28:57.940403 ephios-0.9.2/ephios/modellogging/migrations/__init__.py
--rw-r--r--   0        0        0     2976 2021-07-03 12:30:08.139721 ephios-0.9.2/ephios/modellogging/models.py
--rw-r--r--   0        0        0    17007 2021-07-03 12:30:08.140720 ephios-0.9.2/ephios/modellogging/recorders.py
--rw-r--r--   0        0        0     1473 2021-05-04 20:28:57.942404 ephios-0.9.2/ephios/modellogging/templates/modellogging/logentry.html
--rw-r--r--   0        0        0     1232 2021-08-03 14:26:37.847278 ephios-0.9.2/ephios/modellogging/templates/modellogging/logentry_grouped_list.html
--rw-r--r--   0        0        0      548 2021-05-04 20:28:57.943362 ephios-0.9.2/ephios/modellogging/templates/modellogging/statement.html
--rw-r--r--   0        0        0     1297 2021-05-04 20:28:57.943403 ephios-0.9.2/ephios/modellogging/templatetags/logentries.py
--rw-r--r--   0        0        0        0 2021-03-21 23:27:39.768202 ephios-0.9.2/ephios/plugins/__init__.py
--rw-r--r--   0        0        0        0 2021-06-13 17:00:50.943026 ephios-0.9.2/ephios/plugins/basesignup/__init__.py
--rw-r--r--   0        0        0      439 2021-06-13 17:00:50.943026 ephios-0.9.2/ephios/plugins/basesignup/apps.py
--rw-r--r--   0        0        0      906 2021-10-03 15:39:09.785772 ephios-0.9.2/ephios/plugins/basesignup/signals.py
--rw-r--r--   0        0        0        0 2021-03-21 23:27:39.768202 ephios-0.9.2/ephios/plugins/basesignup/signup/__init__.py
--rw-r--r--   0        0        0     7562 2021-10-03 15:39:09.786774 ephios-0.9.2/ephios/plugins/basesignup/signup/common.py
--rw-r--r--   0        0        0     4756 2021-10-03 15:39:09.787774 ephios-0.9.2/ephios/plugins/basesignup/signup/coupled_signup.py
--rw-r--r--   0        0        0      860 2021-08-03 14:26:37.849287 ephios-0.9.2/ephios/plugins/basesignup/signup/instant.py
--rw-r--r--   0        0        0     1653 2021-10-03 15:39:09.787774 ephios-0.9.2/ephios/plugins/basesignup/signup/no_selfservice.py
--rw-r--r--   0        0        0      941 2021-08-03 14:26:37.850279 ephios-0.9.2/ephios/plugins/basesignup/signup/request_confirm.py
--rw-r--r--   0        0        0    17688 2021-09-14 10:26:09.869801 ephios-0.9.2/ephios/plugins/basesignup/signup/section_based.py
--rw-r--r--   0        0        0      752 2021-08-03 14:26:37.852286 ephios-0.9.2/ephios/plugins/basesignup/templates/basesignup/fragment_state_common.html
--rw-r--r--   0        0        0     1182 2021-08-03 16:16:25.858940 ephios-0.9.2/ephios/plugins/basesignup/templates/basesignup/participation_card_inline.html
--rw-r--r--   0        0        0     3598 2021-07-03 12:30:08.143721 ephios-0.9.2/ephios/plugins/basesignup/templates/basesignup/section_based/configuration_form.html
--rw-r--r--   0        0        0     2259 2021-07-03 12:30:08.144720 ephios-0.9.2/ephios/plugins/basesignup/templates/basesignup/section_based/fragment_participant.html
--rw-r--r--   0        0        0     1474 2021-08-03 15:13:00.372942 ephios-0.9.2/ephios/plugins/basesignup/templates/basesignup/section_based/fragment_state.html
--rw-r--r--   0        0        0      670 2021-03-21 23:27:39.783827 ephios-0.9.2/ephios/plugins/basesignup/templates/basesignup/section_based/signup.html
--rw-r--r--   0        0        0       43 2021-03-21 23:27:39.783827 ephios-0.9.2/ephios/plugins/basesignup/urls.py
--rw-r--r--   0        0        0        0 2021-06-13 17:00:50.944026 ephios-0.9.2/ephios/plugins/eventautoqualification/__init__.py
--rw-r--r--   0        0        0      563 2021-06-13 17:00:50.944026 ephios-0.9.2/ephios/plugins/eventautoqualification/apps.py
--rw-r--r--   0        0        0     2779 2021-05-04 20:28:57.949405 ephios-0.9.2/ephios/plugins/eventautoqualification/consequences.py
--rw-r--r--   0        0        0     2261 2021-10-03 15:39:09.788772 ephios-0.9.2/ephios/plugins/eventautoqualification/forms.py
--rw-r--r--   0        0        0     2261 2021-05-04 20:28:57.950404 ephios-0.9.2/ephios/plugins/eventautoqualification/migrations/0001_initial.py
--rw-r--r--   0        0        0     1220 2021-05-04 20:28:57.951405 ephios-0.9.2/ephios/plugins/eventautoqualification/migrations/0002_auto_20210403_2348.py
--rw-r--r--   0        0        0      537 2021-06-13 17:00:50.945026 ephios-0.9.2/ephios/plugins/eventautoqualification/migrations/0003_alter_eventautoqualificationconfiguration_id.py
--rw-r--r--   0        0        0        0 2021-05-04 20:28:57.951405 ephios-0.9.2/ephios/plugins/eventautoqualification/migrations/__init__.py
--rw-r--r--   0        0        0     1726 2021-10-03 15:39:09.789773 ephios-0.9.2/ephios/plugins/eventautoqualification/models.py
--rw-r--r--   0        0        0      860 2021-05-04 20:28:57.952404 ephios-0.9.2/ephios/plugins/eventautoqualification/signals.py
--rw-r--r--   0        0        0        0 2021-06-13 17:00:50.946027 ephios-0.9.2/ephios/plugins/guests/__init__.py
--rw-r--r--   0        0        0      122 2021-05-04 20:28:57.953405 ephios-0.9.2/ephios/plugins/guests/admin.py
--rw-r--r--   0        0        0      545 2021-06-13 17:00:50.946027 ephios-0.9.2/ephios/plugins/guests/apps.py
--rw-r--r--   0        0        0     1916 2021-05-04 20:28:57.953405 ephios-0.9.2/ephios/plugins/guests/forms.py
--rw-r--r--   0        0        0     3680 2021-05-04 20:28:57.954405 ephios-0.9.2/ephios/plugins/guests/migrations/0001_initial.py
--rw-r--r--   0        0        0      597 2021-05-04 20:28:57.954405 ephios-0.9.2/ephios/plugins/guests/migrations/0002_auto_20210403_2348.py
--rw-r--r--   0        0        0      751 2021-06-13 17:00:50.947027 ephios-0.9.2/ephios/plugins/guests/migrations/0003_auto_20210528_2230.py
--rw-r--r--   0        0        0        0 2021-05-04 20:28:57.954405 ephios-0.9.2/ephios/plugins/guests/migrations/__init__.py
--rw-r--r--   0        0        0     3804 2021-07-03 12:30:08.145720 ephios-0.9.2/ephios/plugins/guests/models.py
--rw-r--r--   0        0        0      899 2021-05-04 20:28:57.955406 ephios-0.9.2/ephios/plugins/guests/signals.py
--rw-r--r--   0        0        0      257 2021-07-03 12:30:08.146722 ephios-0.9.2/ephios/plugins/guests/templates/guests/event_detail.html
--rw-r--r--   0        0        0      914 2021-05-04 20:28:57.957406 ephios-0.9.2/ephios/plugins/guests/templates/guests/guestuser_form.html
--rw-r--r--   0        0        0      772 2021-05-04 20:28:57.957406 ephios-0.9.2/ephios/plugins/guests/urls.py
--rw-r--r--   0        0        0     4169 2021-10-03 15:39:09.789773 ephios-0.9.2/ephios/plugins/guests/views.py
--rw-r--r--   0        0        0        0 2021-06-13 17:00:50.947027 ephios-0.9.2/ephios/plugins/pages/__init__.py
--rw-r--r--   0        0        0      111 2021-03-21 23:27:39.783827 ephios-0.9.2/ephios/plugins/pages/admin.py
--rw-r--r--   0        0        0      529 2021-06-13 17:00:50.948027 ephios-0.9.2/ephios/plugins/pages/apps.py
--rw-r--r--   0        0        0      892 2021-03-21 23:27:39.783827 ephios-0.9.2/ephios/plugins/pages/migrations/0001_initial.py
--rw-r--r--   0        0        0      478 2021-06-13 17:00:50.948027 ephios-0.9.2/ephios/plugins/pages/migrations/0002_alter_page_id.py
--rw-r--r--   0        0        0        0 2021-03-21 23:27:39.783827 ephios-0.9.2/ephios/plugins/pages/migrations/__init__.py
--rw-r--r--   0        0        0      383 2021-03-21 23:27:39.783827 ephios-0.9.2/ephios/plugins/pages/models.py
--rw-r--r--   0        0        0     1041 2021-05-04 20:28:57.959406 ephios-0.9.2/ephios/plugins/pages/signals.py
--rw-r--r--   0        0        0      728 2021-05-04 20:28:57.959406 ephios-0.9.2/ephios/plugins/pages/templates/pages/page_confirm_delete.html
--rw-r--r--   0        0        0      307 2021-03-21 23:27:39.783827 ephios-0.9.2/ephios/plugins/pages/templates/pages/page_detail.html
--rw-r--r--   0        0        0      515 2021-05-04 20:28:57.960406 ephios-0.9.2/ephios/plugins/pages/templates/pages/page_form.html
--rw-r--r--   0        0        0     1570 2021-10-03 15:39:09.790774 ephios-0.9.2/ephios/plugins/pages/templates/pages/page_list.html
--rw-r--r--   0        0        0      659 2021-10-03 15:39:09.790774 ephios-0.9.2/ephios/plugins/pages/urls.py
--rw-r--r--   0        0        0     1894 2021-10-03 15:39:09.791773 ephios-0.9.2/ephios/plugins/pages/views.py
--rw-r--r--   0        0        0        0 2021-10-03 15:39:09.791773 ephios-0.9.2/ephios/plugins/qualification_management/__init__.py
--rw-r--r--   0        0        0      470 2021-10-03 15:39:09.791773 ephios-0.9.2/ephios/plugins/qualification_management/apps.py
--rw-r--r--   0        0        0     1227 2021-10-03 15:39:09.792774 ephios-0.9.2/ephios/plugins/qualification_management/dynamic_preferences_registry.py
--rw-r--r--   0        0        0     9796 2021-10-03 15:39:09.792774 ephios-0.9.2/ephios/plugins/qualification_management/forms.py
--rw-r--r--   0        0        0     9603 2021-10-03 15:39:09.793775 ephios-0.9.2/ephios/plugins/qualification_management/importing.py
--rw-r--r--   0        0        0        0 2021-10-03 15:39:09.793775 ephios-0.9.2/ephios/plugins/qualification_management/migrations/__init__.py
--rw-r--r--   0        0        0     1208 2021-10-03 15:39:09.793775 ephios-0.9.2/ephios/plugins/qualification_management/serializers.py
--rw-r--r--   0        0        0      677 2021-10-03 15:39:09.794774 ephios-0.9.2/ephios/plugins/qualification_management/signals.py
--rw-r--r--   0        0        0      238 2021-10-03 15:39:09.795776 ephios-0.9.2/ephios/plugins/qualification_management/templates/core/import.html
--rw-r--r--   0        0        0      852 2021-10-03 15:39:09.795776 ephios-0.9.2/ephios/plugins/qualification_management/templates/core/qualification_confirm_delete.html
--rw-r--r--   0        0        0     1025 2021-10-03 15:39:09.796775 ephios-0.9.2/ephios/plugins/qualification_management/templates/core/qualification_form.html
--rw-r--r--   0        0        0     3377 2021-10-03 15:39:09.796775 ephios-0.9.2/ephios/plugins/qualification_management/templates/core/qualification_list.html
--rw-r--r--   0        0        0      173 2021-10-03 15:39:09.796775 ephios-0.9.2/ephios/plugins/qualification_management/templates/core/qualification_reassignment.html
--rw-r--r--   0        0        0     4563 2021-10-03 15:39:09.797775 ephios-0.9.2/ephios/plugins/qualification_management/templates/core/qualificationcategories_form.html
--rw-r--r--   0        0        0     1694 2021-10-03 15:39:09.797775 ephios-0.9.2/ephios/plugins/qualification_management/urls.py
--rw-r--r--   0        0        0     5109 2021-10-03 15:39:09.798776 ephios-0.9.2/ephios/plugins/qualification_management/views.py
--rw-r--r--   0        0        0     8844 2021-10-03 15:39:09.798776 ephios-0.9.2/ephios/settings.py
--rw-r--r--   0        0        0   214350 2021-07-03 12:30:08.150721 ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0        0        0   425796 2021-07-03 12:30:08.153723 ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0        0        0    78754 2021-07-03 12:30:08.154724 ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   326390 2021-07-03 12:30:08.158310 ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0   144086 2021-07-03 12:30:08.159310 ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.esm.js
--rw-r--r--   0        0        0   290443 2021-07-03 12:30:08.160311 ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.esm.js.map
--rw-r--r--   0        0        0    72782 2021-07-03 12:30:08.161311 ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.esm.min.js
--rw-r--r--   0        0        0   223119 2021-07-03 12:30:08.162312 ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.esm.min.js.map
--rw-r--r--   0        0        0   153248 2021-07-03 12:30:08.163311 ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.js
--rw-r--r--   0        0        0   291645 2021-07-03 12:30:08.164312 ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.js.map
--rw-r--r--   0        0        0    60097 2021-07-03 12:30:08.164312 ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.min.js
--rw-r--r--   0        0        0   217655 2021-07-03 12:30:08.165313 ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.min.js.map
--rw-r--r--   0        0        0     1153 2021-07-03 12:30:08.148722 ephios-0.9.2/ephios/static/bootstrap/LICENSE
--rw-r--r--   0        0        0     2739 2021-07-03 12:30:08.166313 ephios-0.9.2/ephios/static/bootstrap/scss/_accordion.scss
--rw-r--r--   0        0        0     1531 2021-07-03 12:30:08.166313 ephios-0.9.2/ephios/static/bootstrap/scss/_alert.scss
--rw-r--r--   0        0        0      653 2021-07-03 12:30:08.166313 ephios-0.9.2/ephios/static/bootstrap/scss/_badge.scss
--rw-r--r--   0        0        0      951 2021-07-03 12:30:08.167313 ephios-0.9.2/ephios/static/bootstrap/scss/_breadcrumb.scss
--rw-r--r--   0        0        0     3108 2021-07-03 12:30:08.167313 ephios-0.9.2/ephios/static/bootstrap/scss/_button-group.scss
--rw-r--r--   0        0        0     2343 2021-07-03 12:30:08.168314 ephios-0.9.2/ephios/static/bootstrap/scss/_buttons.scss
--rw-r--r--   0        0        0     4922 2021-07-03 12:30:08.168314 ephios-0.9.2/ephios/static/bootstrap/scss/_card.scss
--rw-r--r--   0        0        0     5852 2021-07-03 12:30:08.169313 ephios-0.9.2/ephios/static/bootstrap/scss/_carousel.scss
--rw-r--r--   0        0        0     1167 2021-07-03 12:30:08.169313 ephios-0.9.2/ephios/static/bootstrap/scss/_close.scss
--rw-r--r--   0        0        0     1237 2021-07-03 12:30:08.169313 ephios-0.9.2/ephios/static/bootstrap/scss/_containers.scss
--rw-r--r--   0        0        0     5829 2021-07-03 12:30:08.170314 ephios-0.9.2/ephios/static/bootstrap/scss/_dropdown.scss
--rw-r--r--   0        0        0      265 2021-07-03 12:30:08.170314 ephios-0.9.2/ephios/static/bootstrap/scss/_forms.scss
--rw-r--r--   0        0        0     8111 2021-07-03 12:30:08.171314 ephios-0.9.2/ephios/static/bootstrap/scss/_functions.scss
--rw-r--r--   0        0        0      308 2021-07-03 12:30:08.171314 ephios-0.9.2/ephios/static/bootstrap/scss/_grid.scss
--rw-r--r--   0        0        0      225 2021-07-03 12:30:08.171314 ephios-0.9.2/ephios/static/bootstrap/scss/_helpers.scss
--rw-r--r--   0        0        0     1199 2021-07-03 12:30:08.172314 ephios-0.9.2/ephios/static/bootstrap/scss/_images.scss
--rw-r--r--   0        0        0     4726 2021-07-03 12:30:08.172314 ephios-0.9.2/ephios/static/bootstrap/scss/_list-group.scss
--rw-r--r--   0        0        0      914 2021-07-03 12:30:08.172314 ephios-0.9.2/ephios/static/bootstrap/scss/_mixins.scss
--rw-r--r--   0        0        0     6016 2021-07-03 12:30:08.173314 ephios-0.9.2/ephios/static/bootstrap/scss/_modal.scss
--rw-r--r--   0        0        0     2807 2021-07-03 12:30:08.173314 ephios-0.9.2/ephios/static/bootstrap/scss/_nav.scss
--rw-r--r--   0        0        0     7119 2021-07-03 12:30:08.174314 ephios-0.9.2/ephios/static/bootstrap/scss/_navbar.scss
--rw-r--r--   0        0        0     1838 2021-07-03 12:30:08.174314 ephios-0.9.2/ephios/static/bootstrap/scss/_offcanvas.scss
--rw-r--r--   0        0        0     1745 2021-07-03 12:30:08.175314 ephios-0.9.2/ephios/static/bootstrap/scss/_pagination.scss
--rw-r--r--   0        0        0     4560 2021-07-03 12:30:08.175314 ephios-0.9.2/ephios/static/bootstrap/scss/_popover.scss
--rw-r--r--   0        0        0     1217 2021-07-03 12:30:08.175314 ephios-0.9.2/ephios/static/bootstrap/scss/_progress.scss
--rw-r--r--   0        0        0    12882 2021-07-03 12:30:08.176315 ephios-0.9.2/ephios/static/bootstrap/scss/_reboot.scss
--rw-r--r--   0        0        0      613 2021-07-03 12:30:08.177319 ephios-0.9.2/ephios/static/bootstrap/scss/_root.scss
--rw-r--r--   0        0        0     1590 2021-07-03 12:30:08.178316 ephios-0.9.2/ephios/static/bootstrap/scss/_spinners.scss
--rw-r--r--   0        0        0     4290 2021-07-03 12:30:08.178316 ephios-0.9.2/ephios/static/bootstrap/scss/_tables.scss
--rw-r--r--   0        0        0     1229 2021-07-03 12:30:08.178316 ephios-0.9.2/ephios/static/bootstrap/scss/_toasts.scss
--rw-r--r--   0        0        0     2717 2021-07-03 12:30:08.179316 ephios-0.9.2/ephios/static/bootstrap/scss/_tooltip.scss
--rw-r--r--   0        0        0      330 2021-07-03 12:30:08.179316 ephios-0.9.2/ephios/static/bootstrap/scss/_transitions.scss
--rw-r--r--   0        0        0     1448 2021-07-03 12:30:08.180316 ephios-0.9.2/ephios/static/bootstrap/scss/_type.scss
--rw-r--r--   0        0        0    13999 2021-07-03 12:30:08.180316 ephios-0.9.2/ephios/static/bootstrap/scss/_utilities.scss
--rw-r--r--   0        0        0    64684 2021-07-03 12:30:08.181316 ephios-0.9.2/ephios/static/bootstrap/scss/_variables.scss
--rw-r--r--   0        0        0     1399 2021-07-03 12:30:08.182316 ephios-0.9.2/ephios/static/bootstrap/scss/bootstrap-grid.scss
--rw-r--r--   0        0        0      708 2021-07-03 12:30:08.182316 ephios-0.9.2/ephios/static/bootstrap/scss/bootstrap-reboot.scss
--rw-r--r--   0        0        0      411 2021-07-03 12:30:08.182316 ephios-0.9.2/ephios/static/bootstrap/scss/bootstrap-utilities.scss
--rw-r--r--   0        0        0     1089 2021-07-03 12:30:08.183316 ephios-0.9.2/ephios/static/bootstrap/scss/bootstrap.scss
--rw-r--r--   0        0        0     1770 2021-07-03 12:30:08.183316 ephios-0.9.2/ephios/static/bootstrap/scss/forms/_floating-labels.scss
--rw-r--r--   0        0        0     4017 2021-07-03 12:30:08.184317 ephios-0.9.2/ephios/static/bootstrap/scss/forms/_form-check.scss
--rw-r--r--   0        0        0     6948 2021-07-03 12:30:08.185317 ephios-0.9.2/ephios/static/bootstrap/scss/forms/_form-control.scss
--rw-r--r--   0        0        0     2886 2021-07-03 12:30:08.185317 ephios-0.9.2/ephios/static/bootstrap/scss/forms/_form-range.scss
--rw-r--r--   0        0        0     2106 2021-07-03 12:30:08.185317 ephios-0.9.2/ephios/static/bootstrap/scss/forms/_form-select.scss
--rw-r--r--   0        0        0      230 2021-07-03 12:30:08.186317 ephios-0.9.2/ephios/static/bootstrap/scss/forms/_form-text.scss
--rw-r--r--   0        0        0     3485 2021-07-03 12:30:08.186317 ephios-0.9.2/ephios/static/bootstrap/scss/forms/_input-group.scss
--rw-r--r--   0        0        0     1178 2021-07-03 12:30:08.186317 ephios-0.9.2/ephios/static/bootstrap/scss/forms/_labels.scss
--rw-r--r--   0        0        0      490 2021-07-03 12:30:08.187317 ephios-0.9.2/ephios/static/bootstrap/scss/forms/_validation.scss
--rw-r--r--   0        0        0       40 2021-07-03 12:30:08.187317 ephios-0.9.2/ephios/static/bootstrap/scss/helpers/_clearfix.scss
--rw-r--r--   0        0        0      338 2021-07-03 12:30:08.188317 ephios-0.9.2/ephios/static/bootstrap/scss/helpers/_colored-links.scss
--rw-r--r--   0        0        0      531 2021-07-03 12:30:08.188317 ephios-0.9.2/ephios/static/bootstrap/scss/helpers/_position.scss
--rw-r--r--   0        0        0      443 2021-07-03 12:30:08.189317 ephios-0.9.2/ephios/static/bootstrap/scss/helpers/_ratio.scss
--rw-r--r--   0        0        0      238 2021-07-03 12:30:08.189317 ephios-0.9.2/ephios/static/bootstrap/scss/helpers/_stretched-link.scss
--rw-r--r--   0        0        0       80 2021-07-03 12:30:08.189317 ephios-0.9.2/ephios/static/bootstrap/scss/helpers/_text-truncation.scss
--rw-r--r--   0        0        0      144 2021-07-03 12:30:08.189317 ephios-0.9.2/ephios/static/bootstrap/scss/helpers/_visually-hidden.scss
--rw-r--r--   0        0        0      279 2021-07-03 12:30:08.190317 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_alert.scss
--rw-r--r--   0        0        0     2109 2021-07-03 12:30:08.190317 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_border-radius.scss
--rw-r--r--   0        0        0      416 2021-07-03 12:30:08.191318 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_box-shadow.scss
--rw-r--r--   0        0        0     4611 2021-07-03 12:30:08.191318 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_breakpoints.scss
--rw-r--r--   0        0        0     4357 2021-07-03 12:30:08.192318 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_buttons.scss
--rw-r--r--   0        0        0     1537 2021-07-03 12:30:08.192318 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_caret.scss
--rw-r--r--   0        0        0      156 2021-07-03 12:30:08.192318 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_clearfix.scss
--rw-r--r--   0        0        0      174 2021-07-03 12:30:08.192318 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_color-scheme.scss
--rw-r--r--   0        0        0      274 2021-07-03 12:30:08.193318 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_container.scss
--rw-r--r--   0        0        0      623 2021-07-03 12:30:08.193318 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_deprecate.scss
--rw-r--r--   0        0        0     4032 2021-07-03 12:30:08.193318 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_forms.scss
--rw-r--r--   0        0        0     2012 2021-07-03 12:30:08.194318 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_gradients.scss
--rw-r--r--   0        0        0     4098 2021-07-03 12:30:08.194318 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_grid.scss
--rw-r--r--   0        0        0      411 2021-07-03 12:30:08.195319 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_image.scss
--rw-r--r--   0        0        0      533 2021-07-03 12:30:08.195319 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_list-group.scss
--rw-r--r--   0        0        0      175 2021-07-03 12:30:08.195319 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_lists.scss
--rw-r--r--   0        0        0      772 2021-07-03 12:30:08.196320 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_pagination.scss
--rw-r--r--   0        0        0      512 2021-07-03 12:30:08.197321 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_reset-text.scss
--rw-r--r--   0        0        0      208 2021-07-03 12:30:08.197321 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_resize.scss
--rw-r--r--   0        0        0     1001 2021-07-03 12:30:08.198320 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_table-variants.scss
--rw-r--r--   0        0        0      176 2021-07-03 12:30:08.198320 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_text-truncate.scss
--rw-r--r--   0        0        0      687 2021-07-03 12:30:08.198320 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_transition.scss
--rw-r--r--   0        0        0     2354 2021-07-03 12:30:08.199320 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_utilities.scss
--rw-r--r--   0        0        0     1040 2021-07-03 12:30:08.199320 ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_visually-hidden.scss
--rw-r--r--   0        0        0     1784 2021-07-03 12:30:08.200321 ephios-0.9.2/ephios/static/bootstrap/scss/utilities/_api.scss
--rw-r--r--   0        0        0     9136 2021-07-03 12:30:08.201322 ephios-0.9.2/ephios/static/bootstrap/scss/vendor/_rfs.scss
--rw-r--r--   0        0        0    10459 2021-03-21 23:27:39.815080 ephios-0.9.2/ephios/static/clipboardjs/js/clipboard.min.js
--rw-r--r--   0        0        0    42114 2021-05-04 20:28:57.964407 ephios-0.9.2/ephios/static/ephios/img/ephios-1024x.png
--rw-r--r--   0        0        0     4369 2021-05-04 20:28:57.964407 ephios-0.9.2/ephios/static/ephios/img/ephios-192x.png
--rw-r--r--   0        0        0    15978 2021-05-04 20:28:57.965407 ephios-0.9.2/ephios/static/ephios/img/ephios-512x.png
--rw-r--r--   0        0        0      621 2021-05-04 20:28:57.965407 ephios-0.9.2/ephios/static/ephios/img/ephios-symbol-red.svg
--rw-r--r--   0        0        0     6534 2021-05-04 20:28:57.966409 ephios-0.9.2/ephios/static/ephios/img/ephios-text-black.png
--rw-r--r--   0        0        0     2446 2021-07-20 21:40:27.755881 ephios-0.9.2/ephios/static/ephios/img/mannequin_confirmed.svg
--rw-r--r--   0        0        0     2658 2021-08-03 14:26:37.855296 ephios-0.9.2/ephios/static/ephios/img/mannequin_denied.svg
--rw-r--r--   0        0        0     1773 2021-07-20 21:40:27.756881 ephios-0.9.2/ephios/static/ephios/img/mannequin_neutral.svg
--rw-r--r--   0        0        0     2312 2021-07-20 21:40:27.757882 ephios-0.9.2/ephios/static/ephios/img/mannequin_requested.svg
--rw-r--r--   0        0        0      974 2021-05-04 20:28:57.966409 ephios-0.9.2/ephios/static/ephios/js/consequences.js
--rw-r--r--   0        0        0     1115 2021-03-21 23:27:39.815080 ephios-0.9.2/ephios/static/ephios/js/event_copy.js
--rw-r--r--   0        0        0      454 2021-07-03 12:30:08.202321 ephios-0.9.2/ephios/static/ephios/js/event_notifications.js
--rw-r--r--   0        0        0    14058 2021-03-21 23:27:39.815080 ephios-0.9.2/ephios/static/ephios/js/formset/formset.js
--rw-r--r--   0        0        0     1316 2021-03-21 23:27:39.815080 ephios-0.9.2/ephios/static/ephios/js/formset/LICENSE
--rw-r--r--   0        0        0      860 2021-05-04 20:28:57.967409 ephios-0.9.2/ephios/static/ephios/js/group_form.js
--rw-r--r--   0        0        0     3400 2021-07-20 21:40:27.758976 ephios-0.9.2/ephios/static/ephios/js/main.js
--rw-r--r--   0        0        0     2647 2021-05-04 20:28:57.968409 ephios-0.9.2/ephios/static/ephios/js/serviceworker.js
--rw-r--r--   0        0        0      653 2021-10-03 15:39:09.799775 ephios-0.9.2/ephios/static/ephios/js/shift_form.js
--rw-r--r--   0        0        0      316 2021-03-21 23:27:39.815080 ephios-0.9.2/ephios/static/ephios/js/userprofile.js
--rw-r--r--   0        0        0     1161 2021-07-20 21:40:27.759882 ephios-0.9.2/ephios/static/ephios/scss/ephios_bootstrap_variables.scss
--rw-r--r--   0        0        0     3460 2021-08-03 14:26:37.856285 ephios-0.9.2/ephios/static/ephios/scss/ephios_custom.scss
--rw-r--r--   0        0        0     1802 2021-07-03 12:30:08.204321 ephios-0.9.2/ephios/static/ephios/scss/main.scss
--rw-r--r--   0        0        0    77703 2021-03-21 23:27:39.815080 ephios-0.9.2/ephios/static/fontawesome/css/all.css
--rw-r--r--   0        0        0   134622 2021-03-21 23:27:39.830706 ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-brands-400.eot
--rw-r--r--   0        0        0   733896 2021-03-21 23:27:39.830706 ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-brands-400.svg
--rw-r--r--   0        0        0   134316 2021-03-21 23:27:39.830706 ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0    90672 2021-03-21 23:27:39.830706 ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-brands-400.woff
--rw-r--r--   0        0        0    77400 2021-03-21 23:27:39.830706 ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    34350 2021-03-21 23:27:39.830706 ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-regular-400.eot
--rw-r--r--   0        0        0   145477 2021-03-21 23:27:39.830706 ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-regular-400.svg
--rw-r--r--   0        0        0    34052 2021-03-21 23:27:39.830706 ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    16780 2021-03-21 23:27:39.830706 ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-regular-400.woff
--rw-r--r--   0        0        0    13600 2021-03-21 23:27:39.830706 ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   204266 2021-03-21 23:27:39.830706 ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-solid-900.eot
--rw-r--r--   0        0        0   919097 2021-03-21 23:27:39.846346 ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-solid-900.svg
--rw-r--r--   0        0        0   203980 2021-03-21 23:27:39.846346 ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   104004 2021-03-21 23:27:39.846346 ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-solid-900.woff
--rw-r--r--   0        0        0    80148 2021-03-21 23:27:39.846346 ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0    89476 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/jquery/js/jquery-3.5.1.min.js
--rw-r--r--   0        0        0     6923 2021-08-03 14:26:37.857285 ephios-0.9.2/ephios/static/plugins/basesignup/js/disposition.js
--rw-r--r--   0        0        0     5478 2021-07-03 12:30:08.204321 ephios-0.9.2/ephios/static/select2/css/select2-bootstrap5.min.css
--rw-r--r--   0        0        0    17839 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/css/select2.css
--rw-r--r--   0        0        0    14967 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/css/select2.min.css
--rw-r--r--   0        0        0      868 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/af.js
--rw-r--r--   0        0        0      907 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/ar.js
--rw-r--r--   0        0        0      723 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/az.js
--rw-r--r--   0        0        0      970 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/bg.js
--rw-r--r--   0        0        0     1293 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/bn.js
--rw-r--r--   0        0        0      967 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/bs.js
--rw-r--r--   0        0        0      902 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/ca.js
--rw-r--r--   0        0        0     1294 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/cs.js
--rw-r--r--   0        0        0      830 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/da.js
--rw-r--r--   0        0        0      868 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/de.js
--rw-r--r--   0        0        0     1019 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/dsb.js
--rw-r--r--   0        0        0     1184 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/el.js
--rw-r--r--   0        0        0      846 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/en.js
--rw-r--r--   0        0        0      924 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/es.js
--rw-r--r--   0        0        0      803 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/et.js
--rw-r--r--   0        0        0      870 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/eu.js
--rw-r--r--   0        0        0     1025 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/fa.js
--rw-r--r--   0        0        0      805 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/fi.js
--rw-r--r--   0        0        0      926 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/fr.js
--rw-r--r--   0        0        0      926 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/gl.js
--rw-r--r--   0        0        0      986 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/he.js
--rw-r--r--   0        0        0     1177 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/hi.js
--rw-r--r--   0        0        0      854 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/hr.js
--rw-r--r--   0        0        0     1020 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/hsb.js
--rw-r--r--   0        0        0      833 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/hu.js
--rw-r--r--   0        0        0     1030 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/hy.js
--rw-r--r--   0        0        0      770 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/id.js
--rw-r--r--   0        0        0      809 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/is.js
--rw-r--r--   0        0        0      899 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/it.js
--rw-r--r--   0        0        0      864 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/ja.js
--rw-r--r--   0        0        0     1197 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/ka.js
--rw-r--r--   0        0        0     1090 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/km.js
--rw-r--r--   0        0        0      857 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/ko.js
--rw-r--r--   0        0        0      946 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/lt.js
--rw-r--r--   0        0        0      902 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/lv.js
--rw-r--r--   0        0        0     1040 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/mk.js
--rw-r--r--   0        0        0      813 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/ms.js
--rw-r--r--   0        0        0      780 2021-03-21 23:27:39.852867 ephios-0.9.2/ephios/static/select2/js/i18n/nb.js
--rw-r--r--   0        0        0     1359 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/i18n/ne.js
--rw-r--r--   0        0        0      906 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/i18n/nl.js
--rw-r--r--   0        0        0      949 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/i18n/pl.js
--rw-r--r--   0        0        0     1051 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/i18n/ps.js
--rw-r--r--   0        0        0      878 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/i18n/pt-BR.js
--rw-r--r--   0        0        0      880 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/i18n/pt.js
--rw-r--r--   0        0        0      940 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/i18n/ro.js
--rw-r--r--   0        0        0     1173 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/i18n/ru.js
--rw-r--r--   0        0        0     1308 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/i18n/sk.js
--rw-r--r--   0        0        0      927 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/i18n/sl.js
--rw-r--r--   0        0        0      905 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/i18n/sq.js
--rw-r--r--   0        0        0     1111 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/i18n/sr-Cyrl.js
--rw-r--r--   0        0        0      982 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/i18n/sr.js
--rw-r--r--   0        0        0      788 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/i18n/sv.js
--rw-r--r--   0        0        0     1076 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/i18n/th.js
--rw-r--r--   0        0        0      773 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/i18n/tk.js
--rw-r--r--   0        0        0      777 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/i18n/tr.js
--rw-r--r--   0        0        0     1158 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/i18n/uk.js
--rw-r--r--   0        0        0      798 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/i18n/vi.js
--rw-r--r--   0        0        0      770 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/i18n/zh-CN.js
--rw-r--r--   0        0        0      709 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/i18n/zh-TW.js
--rw-r--r--   0        0        0   180386 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/select2.full.js
--rw-r--r--   0        0        0    79213 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/select2.full.min.js
--rw-r--r--   0        0        0   159697 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/select2.js
--rw-r--r--   0        0        0    70892 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/select2/js/select2.min.js
--rw-r--r--   0        0        0     1106 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/sortablejs/LICENSE
--rw-r--r--   0        0        0    43304 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/static/sortablejs/Sortable.min.js
--rw-r--r--   0        0        0      356 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/templates/400.html
--rw-r--r--   0        0        0      309 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/templates/403.html
--rw-r--r--   0        0        0      297 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/templates/404.html
--rw-r--r--   0        0        0      372 2021-03-27 14:26:48.977753 ephios-0.9.2/ephios/templates/500.html
--rw-r--r--   0        0        0     9178 2021-08-03 16:16:25.859939 ephios-0.9.2/ephios/templates/base.html
--rw-r--r--   0        0        0      250 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/templates/email_base.html
--rw-r--r--   0        0        0      288 2021-05-04 20:28:57.970408 ephios-0.9.2/ephios/templates/offline.html
--rw-r--r--   0        0        0      290 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/templates/registration/logged_out.html
--rw-r--r--   0        0        0      536 2021-07-03 12:30:08.206321 ephios-0.9.2/ephios/templates/registration/login.html
--rw-r--r--   0        0        0      323 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/templates/registration/password_change_done.html
--rw-r--r--   0        0        0      412 2021-03-21 23:27:39.868499 ephios-0.9.2/ephios/templates/registration/password_change_form.html
--rw-r--r--   0        0        0      385 2021-03-21 23:27:39.884125 ephios-0.9.2/ephios/templates/registration/password_reset_complete.html
--rw-r--r--   0        0        0      805 2021-03-21 23:27:39.884125 ephios-0.9.2/ephios/templates/registration/password_reset_confirm.html
--rw-r--r--   0        0        0      388 2021-03-21 23:27:39.884125 ephios-0.9.2/ephios/templates/registration/password_reset_done.html
--rw-r--r--   0        0        0      419 2021-03-21 23:27:39.884125 ephios-0.9.2/ephios/templates/registration/password_reset_form.html
--rw-r--r--   0        0        0     1639 2021-05-04 20:28:57.970408 ephios-0.9.2/ephios/urls.py
--rw-r--r--   0        0        0      405 2021-03-21 23:27:39.884125 ephios-0.9.2/ephios/wsgi.py
--rw-r--r--   0        0        0     1088 2021-03-21 23:27:39.730437 ephios-0.9.2/LICENSE
--rw-r--r--   0        0        0     2733 2021-10-03 16:45:59.885007 ephios-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     1936 2021-03-21 23:27:39.730437 ephios-0.9.2/README.md
--rw-r--r--   0        0        0     5791 2021-10-03 16:46:26.122058 ephios-0.9.2/setup.py
--rw-r--r--   0        0        0     3732 2021-10-03 16:46:26.123059 ephios-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2021-03-21 23:27:39.730437 ephios-0.9.3/ephios/__init__.py
+-rw-r--r--   0        0        0      647 2021-03-21 23:27:39.730437 ephios-0.9.3/ephios/__main__.py
+-rw-r--r--   0        0        0      405 2021-03-21 23:27:39.730437 ephios-0.9.3/ephios/asgi.py
+-rw-r--r--   0        0        0        0 2021-06-13 17:00:50.934458 ephios-0.9.3/ephios/core/__init__.py
+-rw-r--r--   0        0        0      801 2021-07-20 21:40:27.739008 ephios-0.9.3/ephios/core/admin.py
+-rw-r--r--   0        0        0      510 2021-06-13 17:00:50.934458 ephios-0.9.3/ephios/core/apps.py
+-rw-r--r--   0        0        0     1883 2021-10-03 15:39:09.766769 ephios-0.9.3/ephios/core/calendar.py
+-rw-r--r--   0        0        0     7772 2021-07-03 12:30:08.117715 ephios-0.9.3/ephios/core/consequences.py
+-rw-r--r--   0        0        0      818 2021-08-03 14:26:37.836252 ephios-0.9.3/ephios/core/context.py
+-rw-r--r--   0        0        0     4006 2021-10-03 15:39:09.766769 ephios-0.9.3/ephios/core/dynamic_preferences_registry.py
+-rw-r--r--   0        0        0        0 2021-03-21 23:27:39.730437 ephios-0.9.3/ephios/core/forms/__init__.py
+-rw-r--r--   0        0        0    12447 2021-10-03 15:39:09.767769 ephios-0.9.3/ephios/core/forms/events.py
+-rw-r--r--   0        0        0    12434 2021-10-03 15:39:09.769769 ephios-0.9.3/ephios/core/forms/users.py
+-rw-r--r--   0        0        0     1768 2021-05-04 20:28:57.897392 ephios-0.9.3/ephios/core/ical.py
+-rw-r--r--   0        0        0     4961 2021-03-21 23:27:39.730437 ephios-0.9.3/ephios/core/migrations/0001_initial.py
+-rw-r--r--   0        0        0    17507 2021-03-21 23:27:39.730437 ephios-0.9.3/ephios/core/migrations/0001_squashed_0008_auto_20210207_1309.py
+-rw-r--r--   0        0        0    10162 2021-03-21 23:27:39.730437 ephios-0.9.3/ephios/core/migrations/0001_squashed_event_management_0007_auto_20210207_1309.py
+-rw-r--r--   0        0        0      829 2021-03-21 23:27:39.730437 ephios-0.9.3/ephios/core/migrations/0002_initial_permissions.py
+-rw-r--r--   0        0        0      643 2021-03-21 23:27:39.730437 ephios-0.9.3/ephios/core/migrations/0002_merge_content_type_20210208_0020.py
+-rw-r--r--   0        0        0      623 2021-03-21 23:27:39.730437 ephios-0.9.3/ephios/core/migrations/0003_migrate_content_type_to_core_20210219_1642.py
+-rw-r--r--   0        0        0     7348 2021-03-21 23:27:39.746063 ephios-0.9.3/ephios/core/migrations/0003_userprofile_calendar_token_squashed_0008_auto_20200925_1640.py
+-rw-r--r--   0        0        0     1000 2021-03-21 23:27:39.746063 ephios-0.9.3/ephios/core/migrations/0004_auto_20201014_1648.py
+-rw-r--r--   0        0        0     1152 2021-05-04 20:28:57.898392 ephios-0.9.3/ephios/core/migrations/0004_auto_20210305_1855.py
+-rw-r--r--   0        0        0     3288 2021-03-21 23:27:39.746063 ephios-0.9.3/ephios/core/migrations/0005_auto_20210106_2219.py
+-rw-r--r--   0        0        0      347 2021-05-04 20:28:57.898392 ephios-0.9.3/ephios/core/migrations/0005_remove_event_mail_updates.py
+-rw-r--r--   0        0        0      881 2021-03-21 23:27:39.746063 ephios-0.9.3/ephios/core/migrations/0006_auto_20210109_2230.py
+-rw-r--r--   0        0        0     1509 2021-05-04 20:28:57.898392 ephios-0.9.3/ephios/core/migrations/0006_notification.py
+-rw-r--r--   0        0        0     1117 2021-03-21 23:27:39.746063 ephios-0.9.3/ephios/core/migrations/0007_auto_20210110_0050.py
+-rw-r--r--   0        0        0      614 2021-05-04 20:28:57.899393 ephios-0.9.3/ephios/core/migrations/0007_auto_20210324_2101.py
+-rw-r--r--   0        0        0      435 2021-05-04 20:28:57.899393 ephios-0.9.3/ephios/core/migrations/0007_eventtype_color.py
+-rw-r--r--   0        0        0      971 2021-03-21 23:27:39.746063 ephios-0.9.3/ephios/core/migrations/0008_auto_20210207_1309.py
+-rw-r--r--   0        0        0     2725 2021-05-04 20:28:57.900393 ephios-0.9.3/ephios/core/migrations/0008_auto_20210403_2348.py
+-rw-r--r--   0        0        0     3475 2021-06-13 17:00:50.937460 ephios-0.9.3/ephios/core/migrations/0009_auto_20210528_2230.py
+-rw-r--r--   0        0        0     1171 2021-07-20 21:40:27.739008 ephios-0.9.3/ephios/core/migrations/0010_placeholderparticipation.py
+-rw-r--r--   0        0        0      871 2021-10-03 15:39:09.770769 ephios-0.9.3/ephios/core/migrations/0011_auto_20210903_1258.py
+-rw-r--r--   0        0        0      404 2021-10-03 15:39:09.770769 ephios-0.9.3/ephios/core/migrations/0012_rename_included_qualifications_qualification_includes.py
+-rw-r--r--   0        0        0        0 2021-03-21 23:27:39.746063 ephios-0.9.3/ephios/core/migrations/__init__.py
+-rw-r--r--   0        0        0      317 2021-05-04 20:28:57.900393 ephios-0.9.3/ephios/core/models/__init__.py
+-rw-r--r--   0        0        0    10395 2021-10-03 15:39:09.771770 ephios-0.9.3/ephios/core/models/events.py
+-rw-r--r--   0        0        0    14773 2021-10-10 21:33:14.221992 ephios-0.9.3/ephios/core/models/users.py
+-rw-r--r--   0        0        0     6945 2021-05-04 20:28:57.903394 ephios-0.9.3/ephios/core/pdf.py
+-rw-r--r--   0        0        0     3369 2021-10-03 15:39:09.772770 ephios-0.9.3/ephios/core/plugins.py
+-rw-r--r--   0        0        0        0 2021-05-04 20:28:57.904393 ephios-0.9.3/ephios/core/services/__init__.py
+-rw-r--r--   0        0        0        0 2021-05-04 20:28:57.904393 ephios-0.9.3/ephios/core/services/notifications/__init__.py
+-rw-r--r--   0        0        0     4064 2021-08-01 21:03:19.080402 ephios-0.9.3/ephios/core/services/notifications/backends.py
+-rw-r--r--   0        0        0    16402 2021-08-01 21:03:19.081404 ephios-0.9.3/ephios/core/services/notifications/types.py
+-rw-r--r--   0        0        0     1179 2021-05-04 20:28:57.906394 ephios-0.9.3/ephios/core/services/participation.py
+-rw-r--r--   0        0        0     1066 2021-05-04 20:28:58.024911 ephios-0.9.3/ephios/core/services/password_reset.py
+-rw-r--r--   0        0        0     4859 2021-05-04 20:28:57.907395 ephios-0.9.3/ephios/core/signals.py
+-rw-r--r--   0        0        0       33 2021-03-21 23:27:39.746063 ephios-0.9.3/ephios/core/signup/__init__.py
+-rw-r--r--   0        0        0     9476 2021-10-03 15:39:09.773770 ephios-0.9.3/ephios/core/signup/disposition.py
+-rw-r--r--   0        0        0    21720 2021-10-03 15:39:09.774791 ephios-0.9.3/ephios/core/signup/methods.py
+-rw-r--r--   0        0        0      333 2021-03-21 23:27:39.752569 ephios-0.9.3/ephios/core/templates/core/account_updated_email.html
+-rw-r--r--   0        0        0      275 2021-03-21 23:27:39.752569 ephios-0.9.3/ephios/core/templates/core/disposition/base_participation.html
+-rw-r--r--   0        0        0     5972 2021-07-20 21:40:27.742897 ephios-0.9.3/ephios/core/templates/core/disposition/disposition.html
+-rw-r--r--   0        0        0     1672 2021-07-20 21:40:27.743888 ephios-0.9.3/ephios/core/templates/core/disposition/fragment_participation.html
+-rw-r--r--   0        0        0     1543 2021-05-04 20:28:57.911395 ephios-0.9.3/ephios/core/templates/core/event_archive.html
+-rw-r--r--   0        0        0      942 2021-03-21 23:27:39.752569 ephios-0.9.3/ephios/core/templates/core/event_bulk_delete.html
+-rw-r--r--   0        0        0     1147 2021-08-03 14:26:37.840278 ephios-0.9.3/ephios/core/templates/core/event_calendar.html
+-rw-r--r--   0        0        0      623 2021-05-04 20:28:57.911395 ephios-0.9.3/ephios/core/templates/core/event_confirm_delete.html
+-rw-r--r--   0        0        0     2015 2021-07-03 12:30:08.121716 ephios-0.9.3/ephios/core/templates/core/event_copy.html
+-rw-r--r--   0        0        0     6594 2021-10-03 15:39:09.775771 ephios-0.9.3/ephios/core/templates/core/event_detail.html
+-rw-r--r--   0        0        0     2532 2021-07-03 12:30:08.123716 ephios-0.9.3/ephios/core/templates/core/event_form.html
+-rw-r--r--   0        0        0     9456 2021-08-03 16:16:25.853938 ephios-0.9.3/ephios/core/templates/core/event_list.html
+-rw-r--r--   0        0        0      587 2021-05-04 20:28:57.914397 ephios-0.9.3/ephios/core/templates/core/event_notification.html
+-rw-r--r--   0        0        0      515 2021-03-21 23:27:39.752569 ephios-0.9.3/ephios/core/templates/core/eventtype_confirm_delete.html
+-rw-r--r--   0        0        0      754 2021-07-03 12:30:08.124717 ephios-0.9.3/ephios/core/templates/core/eventtype_form.html
+-rw-r--r--   0        0        0     1364 2021-07-03 12:30:08.124717 ephios-0.9.3/ephios/core/templates/core/eventtype_list.html
+-rw-r--r--   0        0        0     1388 2021-05-04 20:28:57.915397 ephios-0.9.3/ephios/core/templates/core/fragments/approve_consequences.html
+-rw-r--r--   0        0        0      177 2021-03-21 23:27:39.752569 ephios-0.9.3/ephios/core/templates/core/fragments/custom_date_input.html
+-rw-r--r--   0        0        0      207 2021-07-03 12:30:08.125717 ephios-0.9.3/ephios/core/templates/core/fragments/custom_split_date_time_widget.html
+-rw-r--r--   0        0        0      177 2021-03-21 23:27:39.752569 ephios-0.9.3/ephios/core/templates/core/fragments/custom_time_input.html
+-rw-r--r--   0        0        0      430 2021-07-03 12:30:08.126717 ephios-0.9.3/ephios/core/templates/core/fragments/event_plugin_form.html
+-rw-r--r--   0        0        0      699 2021-05-04 22:04:58.666611 ephios-0.9.3/ephios/core/templates/core/fragments/pending_consequences.html
+-rw-r--r--   0        0        0     4405 2021-08-03 14:26:37.841272 ephios-0.9.3/ephios/core/templates/core/fragments/shift_box_big.html
+-rw-r--r--   0        0        0     1270 2021-07-03 12:30:08.127720 ephios-0.9.3/ephios/core/templates/core/fragments/shift_box_small.html
+-rw-r--r--   0        0        0      957 2021-08-03 16:16:25.854937 ephios-0.9.3/ephios/core/templates/core/fragments/signup_stats_indicator.html
+-rw-r--r--   0        0        0      620 2021-03-21 23:27:39.752569 ephios-0.9.3/ephios/core/templates/core/group_confirm_delete.html
+-rw-r--r--   0        0        0      660 2021-03-21 23:27:39.752569 ephios-0.9.3/ephios/core/templates/core/group_form.html
+-rw-r--r--   0        0        0     1408 2021-07-03 12:30:08.128718 ephios-0.9.3/ephios/core/templates/core/group_list.html
+-rw-r--r--   0        0        0     4308 2021-08-03 14:26:37.843282 ephios-0.9.3/ephios/core/templates/core/home.html
+-rw-r--r--   0        0        0     2463 2021-08-03 14:26:37.843282 ephios-0.9.3/ephios/core/templates/core/logentry_list.html
+-rw-r--r--   0        0        0      509 2021-05-04 20:28:58.021185 ephios-0.9.3/ephios/core/templates/core/mails/new_account_email.html
+-rw-r--r--   0        0        0      536 2021-05-04 20:28:57.918396 ephios-0.9.3/ephios/core/templates/core/mails/new_event.html
+-rw-r--r--   0        0        0     2016 2021-05-04 20:28:57.918396 ephios-0.9.3/ephios/core/templates/core/pagination.html
+-rw-r--r--   0        0        0      316 2021-03-21 23:27:39.752569 ephios-0.9.3/ephios/core/templates/core/settings/general.html
+-rw-r--r--   0        0        0      924 2021-07-03 12:30:08.130718 ephios-0.9.3/ephios/core/templates/core/settings/settings_base.html
+-rw-r--r--   0        0        0      627 2021-05-04 20:28:57.919397 ephios-0.9.3/ephios/core/templates/core/shift_confirm_delete.html
+-rw-r--r--   0        0        0     4045 2021-10-03 15:40:55.836260 ephios-0.9.3/ephios/core/templates/core/shift_form.html
+-rw-r--r--   0        0        0      298 2021-07-03 12:30:08.132718 ephios-0.9.3/ephios/core/templates/core/userprofile_badges.html
+-rw-r--r--   0        0        0      724 2021-03-21 23:27:39.752569 ephios-0.9.3/ephios/core/templates/core/userprofile_confirm_delete.html
+-rw-r--r--   0        0        0      829 2021-05-04 20:28:57.920397 ephios-0.9.3/ephios/core/templates/core/userprofile_confirm_password_reset.html
+-rw-r--r--   0        0        0     4878 2021-10-10 21:33:14.222992 ephios-0.9.3/ephios/core/templates/core/userprofile_detail.html
+-rw-r--r--   0        0        0     5685 2021-10-03 15:39:09.776770 ephios-0.9.3/ephios/core/templates/core/userprofile_form.html
+-rw-r--r--   0        0        0     2894 2021-07-03 12:30:08.134719 ephios-0.9.3/ephios/core/templates/core/userprofile_list.html
+-rw-r--r--   0        0        0     1061 2021-05-04 20:28:57.923398 ephios-0.9.3/ephios/core/templates/core/userprofile_notifications.html
+-rw-r--r--   0        0        0      300 2021-03-21 23:27:39.752569 ephios-0.9.3/ephios/core/templates/core/workinghour_request.html
+-rw-r--r--   0        0        0        0 2021-03-21 23:27:39.752569 ephios-0.9.3/ephios/core/templatetags/__init__.py
+-rw-r--r--   0        0        0     3751 2021-08-03 14:26:37.844273 ephios-0.9.3/ephios/core/templatetags/event_extras.py
+-rw-r--r--   0        0        0      393 2021-05-04 20:28:57.924399 ephios-0.9.3/ephios/core/templatetags/param_replace.py
+-rw-r--r--   0        0        0     2420 2021-08-03 14:26:37.845274 ephios-0.9.3/ephios/core/templatetags/user_extras.py
+-rw-r--r--   0        0        0     6707 2021-10-03 15:39:09.777771 ephios-0.9.3/ephios/core/urls.py
+-rw-r--r--   0        0        0        0 2021-03-21 23:27:39.768202 ephios-0.9.3/ephios/core/views/__init__.py
+-rw-r--r--   0        0        0     9555 2021-10-03 15:39:09.777771 ephios-0.9.3/ephios/core/views/accounts.py
+-rw-r--r--   0        0        0     1106 2021-05-04 20:28:57.926398 ephios-0.9.3/ephios/core/views/bulk.py
+-rw-r--r--   0        0        0     1784 2021-07-03 12:30:08.136720 ephios-0.9.3/ephios/core/views/consequences.py
+-rw-r--r--   0        0        0    14010 2021-08-03 16:16:25.855938 ephios-0.9.3/ephios/core/views/event.py
+-rw-r--r--   0        0        0     3356 2021-07-03 12:30:08.138719 ephios-0.9.3/ephios/core/views/eventtype.py
+-rw-r--r--   0        0        0     3810 2021-10-03 15:39:09.778771 ephios-0.9.3/ephios/core/views/log.py
+-rw-r--r--   0        0        0     1227 2021-05-04 20:28:57.929401 ephios-0.9.3/ephios/core/views/pwa.py
+-rw-r--r--   0        0        0     1796 2021-05-04 20:28:57.929401 ephios-0.9.3/ephios/core/views/settings.py
+-rw-r--r--   0        0        0     7421 2021-10-03 16:52:40.166392 ephios-0.9.3/ephios/core/views/shift.py
+-rw-r--r--   0        0        0     1099 2021-05-04 20:28:57.931400 ephios-0.9.3/ephios/core/views/signup.py
+-rw-r--r--   0        0        0      607 2021-03-21 23:27:39.768202 ephios-0.9.3/ephios/core/widgets.py
+-rw-r--r--   0        0        0        0 2021-06-13 17:00:50.940461 ephios-0.9.3/ephios/extra/__init__.py
+-rw-r--r--   0        0        0      196 2021-06-13 17:00:50.940461 ephios-0.9.3/ephios/extra/apps.py
+-rw-r--r--   0        0        0      638 2021-10-03 15:39:09.779773 ephios-0.9.3/ephios/extra/bootstrap.py
+-rw-r--r--   0        0        0     1000 2021-05-04 20:28:57.931400 ephios-0.9.3/ephios/extra/colors.py
+-rw-r--r--   0        0        0     1837 2021-10-03 15:39:09.780773 ephios-0.9.3/ephios/extra/crispy.py
+-rw-r--r--   0        0        0      535 2021-10-03 15:39:09.780773 ephios-0.9.3/ephios/extra/fields.py
+-rw-r--r--   0        0        0      868 2021-03-21 23:27:39.768202 ephios-0.9.3/ephios/extra/json.py
+-rw-r--r--   0        0        0        0 2021-03-21 23:27:39.768202 ephios-0.9.3/ephios/extra/management/__init__.py
+-rw-r--r--   0        0        0        0 2021-03-21 23:27:39.768202 ephios-0.9.3/ephios/extra/management/commands/__init__.py
+-rw-r--r--   0        0        0     3524 2021-10-03 15:39:09.781773 ephios-0.9.3/ephios/extra/management/commands/devdata.py
+-rw-r--r--   0        0        0      209 2021-05-04 20:28:57.931400 ephios-0.9.3/ephios/extra/management/commands/run_periodic.py
+-rw-r--r--   0        0        0      238 2021-05-04 20:28:57.932401 ephios-0.9.3/ephios/extra/management/commands/send_notifications.py
+-rw-r--r--   0        0        0     5219 2021-05-04 20:28:57.932401 ephios-0.9.3/ephios/extra/mixins.py
+-rw-r--r--   0        0        0     3177 2021-10-03 15:39:09.781773 ephios-0.9.3/ephios/extra/permissions.py
+-rw-r--r--   0        0        0      802 2021-10-03 15:39:09.782772 ephios-0.9.3/ephios/extra/preferences.py
+-rw-r--r--   0        0        0        0 2021-03-21 23:27:39.768202 ephios-0.9.3/ephios/extra/signals.py
+-rw-r--r--   0        0        0      494 2021-03-21 23:27:39.768202 ephios-0.9.3/ephios/extra/templatetags/bootstrap.py
+-rw-r--r--   0        0        0      366 2021-03-21 23:27:39.768202 ephios-0.9.3/ephios/extra/templatetags/ephios_crispy.py
+-rw-r--r--   0        0        0     1648 2021-03-21 23:27:39.768202 ephios-0.9.3/ephios/extra/templatetags/rich_text.py
+-rw-r--r--   0        0        0      647 2021-10-10 21:33:14.223993 ephios-0.9.3/ephios/extra/templatetags/utils.py
+-rw-r--r--   0        0        0      168 2021-05-04 20:28:57.934401 ephios-0.9.3/ephios/extra/utils.py
+-rw-r--r--   0        0        0     1402 2021-10-03 15:39:09.783772 ephios-0.9.3/ephios/extra/widgets.py
+-rw-r--r--   0        0        0    85486 2021-10-10 21:32:05.255781 ephios-0.9.3/ephios/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2021-06-13 17:00:50.941460 ephios-0.9.3/ephios/modellogging/__init__.py
+-rw-r--r--   0        0        0      118 2021-05-04 20:28:57.937403 ephios-0.9.3/ephios/modellogging/admin.py
+-rw-r--r--   0        0        0      109 2021-06-13 17:00:50.942046 ephios-0.9.3/ephios/modellogging/apps.py
+-rw-r--r--   0        0        0     2975 2021-05-04 20:28:57.937403 ephios-0.9.3/ephios/modellogging/json.py
+-rw-r--r--   0        0        0     6561 2021-05-04 20:28:57.938402 ephios-0.9.3/ephios/modellogging/log.py
+-rw-r--r--   0        0        0      663 2021-05-04 20:28:57.938402 ephios-0.9.3/ephios/modellogging/middleware.py
+-rw-r--r--   0        0        0     3442 2021-05-04 20:28:57.939402 ephios-0.9.3/ephios/modellogging/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1629 2021-05-04 20:28:57.939402 ephios-0.9.3/ephios/modellogging/migrations/0002_auto_20210403_2348.py
+-rw-r--r--   0        0        0      500 2021-06-13 17:00:50.942046 ephios-0.9.3/ephios/modellogging/migrations/0003_alter_logentry_id.py
+-rw-r--r--   0        0        0      761 2021-07-03 12:30:08.139721 ephios-0.9.3/ephios/modellogging/migrations/0004_alter_logentry_user.py
+-rw-r--r--   0        0        0        0 2021-05-04 20:28:57.940403 ephios-0.9.3/ephios/modellogging/migrations/__init__.py
+-rw-r--r--   0        0        0     2976 2021-07-03 12:30:08.139721 ephios-0.9.3/ephios/modellogging/models.py
+-rw-r--r--   0        0        0    17007 2021-07-03 12:30:08.140720 ephios-0.9.3/ephios/modellogging/recorders.py
+-rw-r--r--   0        0        0     1473 2021-05-04 20:28:57.942404 ephios-0.9.3/ephios/modellogging/templates/modellogging/logentry.html
+-rw-r--r--   0        0        0     1232 2021-08-03 14:26:37.847278 ephios-0.9.3/ephios/modellogging/templates/modellogging/logentry_grouped_list.html
+-rw-r--r--   0        0        0      548 2021-05-04 20:28:57.943362 ephios-0.9.3/ephios/modellogging/templates/modellogging/statement.html
+-rw-r--r--   0        0        0     1297 2021-05-04 20:28:57.943403 ephios-0.9.3/ephios/modellogging/templatetags/logentries.py
+-rw-r--r--   0        0        0        0 2021-03-21 23:27:39.768202 ephios-0.9.3/ephios/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2021-06-13 17:00:50.943026 ephios-0.9.3/ephios/plugins/basesignup/__init__.py
+-rw-r--r--   0        0        0      439 2021-06-13 17:00:50.943026 ephios-0.9.3/ephios/plugins/basesignup/apps.py
+-rw-r--r--   0        0        0      906 2021-10-03 15:39:09.785772 ephios-0.9.3/ephios/plugins/basesignup/signals.py
+-rw-r--r--   0        0        0        0 2021-03-21 23:27:39.768202 ephios-0.9.3/ephios/plugins/basesignup/signup/__init__.py
+-rw-r--r--   0        0        0     7562 2021-10-03 15:39:09.786774 ephios-0.9.3/ephios/plugins/basesignup/signup/common.py
+-rw-r--r--   0        0        0     4756 2021-10-03 15:39:09.787774 ephios-0.9.3/ephios/plugins/basesignup/signup/coupled_signup.py
+-rw-r--r--   0        0        0      860 2021-08-03 14:26:37.849287 ephios-0.9.3/ephios/plugins/basesignup/signup/instant.py
+-rw-r--r--   0        0        0     1653 2021-10-03 15:39:09.787774 ephios-0.9.3/ephios/plugins/basesignup/signup/no_selfservice.py
+-rw-r--r--   0        0        0      941 2021-08-03 14:26:37.850279 ephios-0.9.3/ephios/plugins/basesignup/signup/request_confirm.py
+-rw-r--r--   0        0        0    17688 2021-09-14 10:26:09.869801 ephios-0.9.3/ephios/plugins/basesignup/signup/section_based.py
+-rw-r--r--   0        0        0      752 2021-08-03 14:26:37.852286 ephios-0.9.3/ephios/plugins/basesignup/templates/basesignup/fragment_state_common.html
+-rw-r--r--   0        0        0     1182 2021-08-03 16:16:25.858940 ephios-0.9.3/ephios/plugins/basesignup/templates/basesignup/participation_card_inline.html
+-rw-r--r--   0        0        0     3598 2021-07-03 12:30:08.143721 ephios-0.9.3/ephios/plugins/basesignup/templates/basesignup/section_based/configuration_form.html
+-rw-r--r--   0        0        0     2259 2021-07-03 12:30:08.144720 ephios-0.9.3/ephios/plugins/basesignup/templates/basesignup/section_based/fragment_participant.html
+-rw-r--r--   0        0        0     1474 2021-08-03 15:13:00.372942 ephios-0.9.3/ephios/plugins/basesignup/templates/basesignup/section_based/fragment_state.html
+-rw-r--r--   0        0        0      670 2021-03-21 23:27:39.783827 ephios-0.9.3/ephios/plugins/basesignup/templates/basesignup/section_based/signup.html
+-rw-r--r--   0        0        0       43 2021-03-21 23:27:39.783827 ephios-0.9.3/ephios/plugins/basesignup/urls.py
+-rw-r--r--   0        0        0        0 2021-06-13 17:00:50.944026 ephios-0.9.3/ephios/plugins/eventautoqualification/__init__.py
+-rw-r--r--   0        0        0      563 2021-06-13 17:00:50.944026 ephios-0.9.3/ephios/plugins/eventautoqualification/apps.py
+-rw-r--r--   0        0        0     2779 2021-05-04 20:28:57.949405 ephios-0.9.3/ephios/plugins/eventautoqualification/consequences.py
+-rw-r--r--   0        0        0     2261 2021-10-03 15:39:09.788772 ephios-0.9.3/ephios/plugins/eventautoqualification/forms.py
+-rw-r--r--   0        0        0     2261 2021-05-04 20:28:57.950404 ephios-0.9.3/ephios/plugins/eventautoqualification/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1220 2021-05-04 20:28:57.951405 ephios-0.9.3/ephios/plugins/eventautoqualification/migrations/0002_auto_20210403_2348.py
+-rw-r--r--   0        0        0      537 2021-06-13 17:00:50.945026 ephios-0.9.3/ephios/plugins/eventautoqualification/migrations/0003_alter_eventautoqualificationconfiguration_id.py
+-rw-r--r--   0        0        0        0 2021-05-04 20:28:57.951405 ephios-0.9.3/ephios/plugins/eventautoqualification/migrations/__init__.py
+-rw-r--r--   0        0        0     1726 2021-10-03 15:39:09.789773 ephios-0.9.3/ephios/plugins/eventautoqualification/models.py
+-rw-r--r--   0        0        0      860 2021-05-04 20:28:57.952404 ephios-0.9.3/ephios/plugins/eventautoqualification/signals.py
+-rw-r--r--   0        0        0        0 2021-06-13 17:00:50.946027 ephios-0.9.3/ephios/plugins/guests/__init__.py
+-rw-r--r--   0        0        0      122 2021-05-04 20:28:57.953405 ephios-0.9.3/ephios/plugins/guests/admin.py
+-rw-r--r--   0        0        0      545 2021-06-13 17:00:50.946027 ephios-0.9.3/ephios/plugins/guests/apps.py
+-rw-r--r--   0        0        0     1916 2021-05-04 20:28:57.953405 ephios-0.9.3/ephios/plugins/guests/forms.py
+-rw-r--r--   0        0        0     3680 2021-05-04 20:28:57.954405 ephios-0.9.3/ephios/plugins/guests/migrations/0001_initial.py
+-rw-r--r--   0        0        0      597 2021-05-04 20:28:57.954405 ephios-0.9.3/ephios/plugins/guests/migrations/0002_auto_20210403_2348.py
+-rw-r--r--   0        0        0      751 2021-06-13 17:00:50.947027 ephios-0.9.3/ephios/plugins/guests/migrations/0003_auto_20210528_2230.py
+-rw-r--r--   0        0        0        0 2021-05-04 20:28:57.954405 ephios-0.9.3/ephios/plugins/guests/migrations/__init__.py
+-rw-r--r--   0        0        0     3804 2021-07-03 12:30:08.145720 ephios-0.9.3/ephios/plugins/guests/models.py
+-rw-r--r--   0        0        0      899 2021-05-04 20:28:57.955406 ephios-0.9.3/ephios/plugins/guests/signals.py
+-rw-r--r--   0        0        0      257 2021-07-03 12:30:08.146722 ephios-0.9.3/ephios/plugins/guests/templates/guests/event_detail.html
+-rw-r--r--   0        0        0      914 2021-05-04 20:28:57.957406 ephios-0.9.3/ephios/plugins/guests/templates/guests/guestuser_form.html
+-rw-r--r--   0        0        0      772 2021-05-04 20:28:57.957406 ephios-0.9.3/ephios/plugins/guests/urls.py
+-rw-r--r--   0        0        0     4169 2021-10-03 15:39:09.789773 ephios-0.9.3/ephios/plugins/guests/views.py
+-rw-r--r--   0        0        0        0 2021-06-13 17:00:50.947027 ephios-0.9.3/ephios/plugins/pages/__init__.py
+-rw-r--r--   0        0        0      111 2021-03-21 23:27:39.783827 ephios-0.9.3/ephios/plugins/pages/admin.py
+-rw-r--r--   0        0        0      529 2021-06-13 17:00:50.948027 ephios-0.9.3/ephios/plugins/pages/apps.py
+-rw-r--r--   0        0        0      892 2021-03-21 23:27:39.783827 ephios-0.9.3/ephios/plugins/pages/migrations/0001_initial.py
+-rw-r--r--   0        0        0      478 2021-06-13 17:00:50.948027 ephios-0.9.3/ephios/plugins/pages/migrations/0002_alter_page_id.py
+-rw-r--r--   0        0        0        0 2021-03-21 23:27:39.783827 ephios-0.9.3/ephios/plugins/pages/migrations/__init__.py
+-rw-r--r--   0        0        0      383 2021-03-21 23:27:39.783827 ephios-0.9.3/ephios/plugins/pages/models.py
+-rw-r--r--   0        0        0     1041 2021-05-04 20:28:57.959406 ephios-0.9.3/ephios/plugins/pages/signals.py
+-rw-r--r--   0        0        0      728 2021-05-04 20:28:57.959406 ephios-0.9.3/ephios/plugins/pages/templates/pages/page_confirm_delete.html
+-rw-r--r--   0        0        0      307 2021-03-21 23:27:39.783827 ephios-0.9.3/ephios/plugins/pages/templates/pages/page_detail.html
+-rw-r--r--   0        0        0      515 2021-05-04 20:28:57.960406 ephios-0.9.3/ephios/plugins/pages/templates/pages/page_form.html
+-rw-r--r--   0        0        0     1570 2021-10-03 15:39:09.790774 ephios-0.9.3/ephios/plugins/pages/templates/pages/page_list.html
+-rw-r--r--   0        0        0      659 2021-10-03 15:39:09.790774 ephios-0.9.3/ephios/plugins/pages/urls.py
+-rw-r--r--   0        0        0     1894 2021-10-03 15:39:09.791773 ephios-0.9.3/ephios/plugins/pages/views.py
+-rw-r--r--   0        0        0        0 2021-10-03 15:39:09.791773 ephios-0.9.3/ephios/plugins/qualification_management/__init__.py
+-rw-r--r--   0        0        0      470 2021-10-03 15:39:09.791773 ephios-0.9.3/ephios/plugins/qualification_management/apps.py
+-rw-r--r--   0        0        0     1227 2021-10-03 15:39:09.792774 ephios-0.9.3/ephios/plugins/qualification_management/dynamic_preferences_registry.py
+-rw-r--r--   0        0        0     9796 2021-10-03 15:39:09.792774 ephios-0.9.3/ephios/plugins/qualification_management/forms.py
+-rw-r--r--   0        0        0     9603 2021-10-03 15:39:09.793775 ephios-0.9.3/ephios/plugins/qualification_management/importing.py
+-rw-r--r--   0        0        0        0 2021-10-03 15:39:09.793775 ephios-0.9.3/ephios/plugins/qualification_management/migrations/__init__.py
+-rw-r--r--   0        0        0     1208 2021-10-03 15:39:09.793775 ephios-0.9.3/ephios/plugins/qualification_management/serializers.py
+-rw-r--r--   0        0        0      677 2021-10-03 15:39:09.794774 ephios-0.9.3/ephios/plugins/qualification_management/signals.py
+-rw-r--r--   0        0        0      238 2021-10-03 15:39:09.795776 ephios-0.9.3/ephios/plugins/qualification_management/templates/core/import.html
+-rw-r--r--   0        0        0      852 2021-10-03 15:39:09.795776 ephios-0.9.3/ephios/plugins/qualification_management/templates/core/qualification_confirm_delete.html
+-rw-r--r--   0        0        0     1025 2021-10-03 15:39:09.796775 ephios-0.9.3/ephios/plugins/qualification_management/templates/core/qualification_form.html
+-rw-r--r--   0        0        0     3377 2021-10-03 15:39:09.796775 ephios-0.9.3/ephios/plugins/qualification_management/templates/core/qualification_list.html
+-rw-r--r--   0        0        0      173 2021-10-03 15:39:09.796775 ephios-0.9.3/ephios/plugins/qualification_management/templates/core/qualification_reassignment.html
+-rw-r--r--   0        0        0     4563 2021-10-03 15:39:09.797775 ephios-0.9.3/ephios/plugins/qualification_management/templates/core/qualificationcategories_form.html
+-rw-r--r--   0        0        0     1694 2021-10-03 15:39:09.797775 ephios-0.9.3/ephios/plugins/qualification_management/urls.py
+-rw-r--r--   0        0        0     5109 2021-10-03 15:39:09.798776 ephios-0.9.3/ephios/plugins/qualification_management/views.py
+-rw-r--r--   0        0        0     8844 2021-10-03 15:39:09.798776 ephios-0.9.3/ephios/settings.py
+-rw-r--r--   0        0        0   214350 2021-07-03 12:30:08.150721 ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0        0        0   425796 2021-07-03 12:30:08.153723 ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0        0        0    78754 2021-07-03 12:30:08.154724 ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   326390 2021-07-03 12:30:08.158310 ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0   144086 2021-07-03 12:30:08.159310 ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.esm.js
+-rw-r--r--   0        0        0   290443 2021-07-03 12:30:08.160311 ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.esm.js.map
+-rw-r--r--   0        0        0    72782 2021-07-03 12:30:08.161311 ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.esm.min.js
+-rw-r--r--   0        0        0   223119 2021-07-03 12:30:08.162312 ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.esm.min.js.map
+-rw-r--r--   0        0        0   153248 2021-07-03 12:30:08.163311 ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.js
+-rw-r--r--   0        0        0   291645 2021-07-03 12:30:08.164312 ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.js.map
+-rw-r--r--   0        0        0    60097 2021-07-03 12:30:08.164312 ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0        0        0   217655 2021-07-03 12:30:08.165313 ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0     1153 2021-07-03 12:30:08.148722 ephios-0.9.3/ephios/static/bootstrap/LICENSE
+-rw-r--r--   0        0        0     2739 2021-07-03 12:30:08.166313 ephios-0.9.3/ephios/static/bootstrap/scss/_accordion.scss
+-rw-r--r--   0        0        0     1531 2021-07-03 12:30:08.166313 ephios-0.9.3/ephios/static/bootstrap/scss/_alert.scss
+-rw-r--r--   0        0        0      653 2021-07-03 12:30:08.166313 ephios-0.9.3/ephios/static/bootstrap/scss/_badge.scss
+-rw-r--r--   0        0        0      951 2021-07-03 12:30:08.167313 ephios-0.9.3/ephios/static/bootstrap/scss/_breadcrumb.scss
+-rw-r--r--   0        0        0     3108 2021-07-03 12:30:08.167313 ephios-0.9.3/ephios/static/bootstrap/scss/_button-group.scss
+-rw-r--r--   0        0        0     2343 2021-07-03 12:30:08.168314 ephios-0.9.3/ephios/static/bootstrap/scss/_buttons.scss
+-rw-r--r--   0        0        0     4922 2021-07-03 12:30:08.168314 ephios-0.9.3/ephios/static/bootstrap/scss/_card.scss
+-rw-r--r--   0        0        0     5852 2021-07-03 12:30:08.169313 ephios-0.9.3/ephios/static/bootstrap/scss/_carousel.scss
+-rw-r--r--   0        0        0     1167 2021-07-03 12:30:08.169313 ephios-0.9.3/ephios/static/bootstrap/scss/_close.scss
+-rw-r--r--   0        0        0     1237 2021-07-03 12:30:08.169313 ephios-0.9.3/ephios/static/bootstrap/scss/_containers.scss
+-rw-r--r--   0        0        0     5829 2021-07-03 12:30:08.170314 ephios-0.9.3/ephios/static/bootstrap/scss/_dropdown.scss
+-rw-r--r--   0        0        0      265 2021-07-03 12:30:08.170314 ephios-0.9.3/ephios/static/bootstrap/scss/_forms.scss
+-rw-r--r--   0        0        0     8111 2021-07-03 12:30:08.171314 ephios-0.9.3/ephios/static/bootstrap/scss/_functions.scss
+-rw-r--r--   0        0        0      308 2021-07-03 12:30:08.171314 ephios-0.9.3/ephios/static/bootstrap/scss/_grid.scss
+-rw-r--r--   0        0        0      225 2021-07-03 12:30:08.171314 ephios-0.9.3/ephios/static/bootstrap/scss/_helpers.scss
+-rw-r--r--   0        0        0     1199 2021-07-03 12:30:08.172314 ephios-0.9.3/ephios/static/bootstrap/scss/_images.scss
+-rw-r--r--   0        0        0     4726 2021-07-03 12:30:08.172314 ephios-0.9.3/ephios/static/bootstrap/scss/_list-group.scss
+-rw-r--r--   0        0        0      914 2021-07-03 12:30:08.172314 ephios-0.9.3/ephios/static/bootstrap/scss/_mixins.scss
+-rw-r--r--   0        0        0     6016 2021-07-03 12:30:08.173314 ephios-0.9.3/ephios/static/bootstrap/scss/_modal.scss
+-rw-r--r--   0        0        0     2807 2021-07-03 12:30:08.173314 ephios-0.9.3/ephios/static/bootstrap/scss/_nav.scss
+-rw-r--r--   0        0        0     7119 2021-07-03 12:30:08.174314 ephios-0.9.3/ephios/static/bootstrap/scss/_navbar.scss
+-rw-r--r--   0        0        0     1838 2021-07-03 12:30:08.174314 ephios-0.9.3/ephios/static/bootstrap/scss/_offcanvas.scss
+-rw-r--r--   0        0        0     1745 2021-07-03 12:30:08.175314 ephios-0.9.3/ephios/static/bootstrap/scss/_pagination.scss
+-rw-r--r--   0        0        0     4560 2021-07-03 12:30:08.175314 ephios-0.9.3/ephios/static/bootstrap/scss/_popover.scss
+-rw-r--r--   0        0        0     1217 2021-07-03 12:30:08.175314 ephios-0.9.3/ephios/static/bootstrap/scss/_progress.scss
+-rw-r--r--   0        0        0    12882 2021-07-03 12:30:08.176315 ephios-0.9.3/ephios/static/bootstrap/scss/_reboot.scss
+-rw-r--r--   0        0        0      613 2021-07-03 12:30:08.177319 ephios-0.9.3/ephios/static/bootstrap/scss/_root.scss
+-rw-r--r--   0        0        0     1590 2021-07-03 12:30:08.178316 ephios-0.9.3/ephios/static/bootstrap/scss/_spinners.scss
+-rw-r--r--   0        0        0     4290 2021-07-03 12:30:08.178316 ephios-0.9.3/ephios/static/bootstrap/scss/_tables.scss
+-rw-r--r--   0        0        0     1229 2021-07-03 12:30:08.178316 ephios-0.9.3/ephios/static/bootstrap/scss/_toasts.scss
+-rw-r--r--   0        0        0     2717 2021-07-03 12:30:08.179316 ephios-0.9.3/ephios/static/bootstrap/scss/_tooltip.scss
+-rw-r--r--   0        0        0      330 2021-07-03 12:30:08.179316 ephios-0.9.3/ephios/static/bootstrap/scss/_transitions.scss
+-rw-r--r--   0        0        0     1448 2021-07-03 12:30:08.180316 ephios-0.9.3/ephios/static/bootstrap/scss/_type.scss
+-rw-r--r--   0        0        0    13999 2021-07-03 12:30:08.180316 ephios-0.9.3/ephios/static/bootstrap/scss/_utilities.scss
+-rw-r--r--   0        0        0    64684 2021-07-03 12:30:08.181316 ephios-0.9.3/ephios/static/bootstrap/scss/_variables.scss
+-rw-r--r--   0        0        0     1399 2021-07-03 12:30:08.182316 ephios-0.9.3/ephios/static/bootstrap/scss/bootstrap-grid.scss
+-rw-r--r--   0        0        0      708 2021-07-03 12:30:08.182316 ephios-0.9.3/ephios/static/bootstrap/scss/bootstrap-reboot.scss
+-rw-r--r--   0        0        0      411 2021-07-03 12:30:08.182316 ephios-0.9.3/ephios/static/bootstrap/scss/bootstrap-utilities.scss
+-rw-r--r--   0        0        0     1089 2021-07-03 12:30:08.183316 ephios-0.9.3/ephios/static/bootstrap/scss/bootstrap.scss
+-rw-r--r--   0        0        0     1770 2021-07-03 12:30:08.183316 ephios-0.9.3/ephios/static/bootstrap/scss/forms/_floating-labels.scss
+-rw-r--r--   0        0        0     4017 2021-07-03 12:30:08.184317 ephios-0.9.3/ephios/static/bootstrap/scss/forms/_form-check.scss
+-rw-r--r--   0        0        0     6948 2021-07-03 12:30:08.185317 ephios-0.9.3/ephios/static/bootstrap/scss/forms/_form-control.scss
+-rw-r--r--   0        0        0     2886 2021-07-03 12:30:08.185317 ephios-0.9.3/ephios/static/bootstrap/scss/forms/_form-range.scss
+-rw-r--r--   0        0        0     2106 2021-07-03 12:30:08.185317 ephios-0.9.3/ephios/static/bootstrap/scss/forms/_form-select.scss
+-rw-r--r--   0        0        0      230 2021-07-03 12:30:08.186317 ephios-0.9.3/ephios/static/bootstrap/scss/forms/_form-text.scss
+-rw-r--r--   0        0        0     3485 2021-07-03 12:30:08.186317 ephios-0.9.3/ephios/static/bootstrap/scss/forms/_input-group.scss
+-rw-r--r--   0        0        0     1178 2021-07-03 12:30:08.186317 ephios-0.9.3/ephios/static/bootstrap/scss/forms/_labels.scss
+-rw-r--r--   0        0        0      490 2021-07-03 12:30:08.187317 ephios-0.9.3/ephios/static/bootstrap/scss/forms/_validation.scss
+-rw-r--r--   0        0        0       40 2021-07-03 12:30:08.187317 ephios-0.9.3/ephios/static/bootstrap/scss/helpers/_clearfix.scss
+-rw-r--r--   0        0        0      338 2021-07-03 12:30:08.188317 ephios-0.9.3/ephios/static/bootstrap/scss/helpers/_colored-links.scss
+-rw-r--r--   0        0        0      531 2021-07-03 12:30:08.188317 ephios-0.9.3/ephios/static/bootstrap/scss/helpers/_position.scss
+-rw-r--r--   0        0        0      443 2021-07-03 12:30:08.189317 ephios-0.9.3/ephios/static/bootstrap/scss/helpers/_ratio.scss
+-rw-r--r--   0        0        0      238 2021-07-03 12:30:08.189317 ephios-0.9.3/ephios/static/bootstrap/scss/helpers/_stretched-link.scss
+-rw-r--r--   0        0        0       80 2021-07-03 12:30:08.189317 ephios-0.9.3/ephios/static/bootstrap/scss/helpers/_text-truncation.scss
+-rw-r--r--   0        0        0      144 2021-07-03 12:30:08.189317 ephios-0.9.3/ephios/static/bootstrap/scss/helpers/_visually-hidden.scss
+-rw-r--r--   0        0        0      279 2021-07-03 12:30:08.190317 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_alert.scss
+-rw-r--r--   0        0        0     2109 2021-07-03 12:30:08.190317 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_border-radius.scss
+-rw-r--r--   0        0        0      416 2021-07-03 12:30:08.191318 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_box-shadow.scss
+-rw-r--r--   0        0        0     4611 2021-07-03 12:30:08.191318 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_breakpoints.scss
+-rw-r--r--   0        0        0     4357 2021-07-03 12:30:08.192318 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_buttons.scss
+-rw-r--r--   0        0        0     1537 2021-07-03 12:30:08.192318 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_caret.scss
+-rw-r--r--   0        0        0      156 2021-07-03 12:30:08.192318 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_clearfix.scss
+-rw-r--r--   0        0        0      174 2021-07-03 12:30:08.192318 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_color-scheme.scss
+-rw-r--r--   0        0        0      274 2021-07-03 12:30:08.193318 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_container.scss
+-rw-r--r--   0        0        0      623 2021-07-03 12:30:08.193318 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_deprecate.scss
+-rw-r--r--   0        0        0     4032 2021-07-03 12:30:08.193318 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_forms.scss
+-rw-r--r--   0        0        0     2012 2021-07-03 12:30:08.194318 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_gradients.scss
+-rw-r--r--   0        0        0     4098 2021-07-03 12:30:08.194318 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_grid.scss
+-rw-r--r--   0        0        0      411 2021-07-03 12:30:08.195319 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_image.scss
+-rw-r--r--   0        0        0      533 2021-07-03 12:30:08.195319 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_list-group.scss
+-rw-r--r--   0        0        0      175 2021-07-03 12:30:08.195319 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_lists.scss
+-rw-r--r--   0        0        0      772 2021-07-03 12:30:08.196320 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_pagination.scss
+-rw-r--r--   0        0        0      512 2021-07-03 12:30:08.197321 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_reset-text.scss
+-rw-r--r--   0        0        0      208 2021-07-03 12:30:08.197321 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_resize.scss
+-rw-r--r--   0        0        0     1001 2021-07-03 12:30:08.198320 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_table-variants.scss
+-rw-r--r--   0        0        0      176 2021-07-03 12:30:08.198320 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_text-truncate.scss
+-rw-r--r--   0        0        0      687 2021-07-03 12:30:08.198320 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_transition.scss
+-rw-r--r--   0        0        0     2354 2021-07-03 12:30:08.199320 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_utilities.scss
+-rw-r--r--   0        0        0     1040 2021-07-03 12:30:08.199320 ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_visually-hidden.scss
+-rw-r--r--   0        0        0     1784 2021-07-03 12:30:08.200321 ephios-0.9.3/ephios/static/bootstrap/scss/utilities/_api.scss
+-rw-r--r--   0        0        0     9136 2021-07-03 12:30:08.201322 ephios-0.9.3/ephios/static/bootstrap/scss/vendor/_rfs.scss
+-rw-r--r--   0        0        0    10459 2021-03-21 23:27:39.815080 ephios-0.9.3/ephios/static/clipboardjs/js/clipboard.min.js
+-rw-r--r--   0        0        0    42114 2021-05-04 20:28:57.964407 ephios-0.9.3/ephios/static/ephios/img/ephios-1024x.png
+-rw-r--r--   0        0        0     4369 2021-05-04 20:28:57.964407 ephios-0.9.3/ephios/static/ephios/img/ephios-192x.png
+-rw-r--r--   0        0        0    15978 2021-05-04 20:28:57.965407 ephios-0.9.3/ephios/static/ephios/img/ephios-512x.png
+-rw-r--r--   0        0        0      621 2021-05-04 20:28:57.965407 ephios-0.9.3/ephios/static/ephios/img/ephios-symbol-red.svg
+-rw-r--r--   0        0        0     6534 2021-05-04 20:28:57.966409 ephios-0.9.3/ephios/static/ephios/img/ephios-text-black.png
+-rw-r--r--   0        0        0     2446 2021-07-20 21:40:27.755881 ephios-0.9.3/ephios/static/ephios/img/mannequin_confirmed.svg
+-rw-r--r--   0        0        0     2658 2021-08-03 14:26:37.855296 ephios-0.9.3/ephios/static/ephios/img/mannequin_denied.svg
+-rw-r--r--   0        0        0     1773 2021-07-20 21:40:27.756881 ephios-0.9.3/ephios/static/ephios/img/mannequin_neutral.svg
+-rw-r--r--   0        0        0     2312 2021-07-20 21:40:27.757882 ephios-0.9.3/ephios/static/ephios/img/mannequin_requested.svg
+-rw-r--r--   0        0        0      974 2021-05-04 20:28:57.966409 ephios-0.9.3/ephios/static/ephios/js/consequences.js
+-rw-r--r--   0        0        0     1115 2021-03-21 23:27:39.815080 ephios-0.9.3/ephios/static/ephios/js/event_copy.js
+-rw-r--r--   0        0        0      454 2021-07-03 12:30:08.202321 ephios-0.9.3/ephios/static/ephios/js/event_notifications.js
+-rw-r--r--   0        0        0    14058 2021-03-21 23:27:39.815080 ephios-0.9.3/ephios/static/ephios/js/formset/formset.js
+-rw-r--r--   0        0        0     1316 2021-03-21 23:27:39.815080 ephios-0.9.3/ephios/static/ephios/js/formset/LICENSE
+-rw-r--r--   0        0        0      860 2021-05-04 20:28:57.967409 ephios-0.9.3/ephios/static/ephios/js/group_form.js
+-rw-r--r--   0        0        0     3400 2021-07-20 21:40:27.758976 ephios-0.9.3/ephios/static/ephios/js/main.js
+-rw-r--r--   0        0        0     2647 2021-05-04 20:28:57.968409 ephios-0.9.3/ephios/static/ephios/js/serviceworker.js
+-rw-r--r--   0        0        0      653 2021-10-03 15:39:09.799775 ephios-0.9.3/ephios/static/ephios/js/shift_form.js
+-rw-r--r--   0        0        0      316 2021-03-21 23:27:39.815080 ephios-0.9.3/ephios/static/ephios/js/userprofile.js
+-rw-r--r--   0        0        0     1161 2021-07-20 21:40:27.759882 ephios-0.9.3/ephios/static/ephios/scss/ephios_bootstrap_variables.scss
+-rw-r--r--   0        0        0     3460 2021-08-03 14:26:37.856285 ephios-0.9.3/ephios/static/ephios/scss/ephios_custom.scss
+-rw-r--r--   0        0        0     1802 2021-07-03 12:30:08.204321 ephios-0.9.3/ephios/static/ephios/scss/main.scss
+-rw-r--r--   0        0        0    77703 2021-03-21 23:27:39.815080 ephios-0.9.3/ephios/static/fontawesome/css/all.css
+-rw-r--r--   0        0        0   134622 2021-03-21 23:27:39.830706 ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-brands-400.eot
+-rw-r--r--   0        0        0   733896 2021-03-21 23:27:39.830706 ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-brands-400.svg
+-rw-r--r--   0        0        0   134316 2021-03-21 23:27:39.830706 ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0    90672 2021-03-21 23:27:39.830706 ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-brands-400.woff
+-rw-r--r--   0        0        0    77400 2021-03-21 23:27:39.830706 ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    34350 2021-03-21 23:27:39.830706 ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-regular-400.eot
+-rw-r--r--   0        0        0   145477 2021-03-21 23:27:39.830706 ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-regular-400.svg
+-rw-r--r--   0        0        0    34052 2021-03-21 23:27:39.830706 ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    16780 2021-03-21 23:27:39.830706 ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-regular-400.woff
+-rw-r--r--   0        0        0    13600 2021-03-21 23:27:39.830706 ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   204266 2021-03-21 23:27:39.830706 ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-solid-900.eot
+-rw-r--r--   0        0        0   919097 2021-03-21 23:27:39.846346 ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-solid-900.svg
+-rw-r--r--   0        0        0   203980 2021-03-21 23:27:39.846346 ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   104004 2021-03-21 23:27:39.846346 ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-solid-900.woff
+-rw-r--r--   0        0        0    80148 2021-03-21 23:27:39.846346 ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0    89476 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/jquery/js/jquery-3.5.1.min.js
+-rw-r--r--   0        0        0     6923 2021-08-03 14:26:37.857285 ephios-0.9.3/ephios/static/plugins/basesignup/js/disposition.js
+-rw-r--r--   0        0        0     5478 2021-07-03 12:30:08.204321 ephios-0.9.3/ephios/static/select2/css/select2-bootstrap5.min.css
+-rw-r--r--   0        0        0    17839 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/css/select2.css
+-rw-r--r--   0        0        0    14967 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/css/select2.min.css
+-rw-r--r--   0        0        0      868 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/af.js
+-rw-r--r--   0        0        0      907 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/ar.js
+-rw-r--r--   0        0        0      723 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/az.js
+-rw-r--r--   0        0        0      970 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/bg.js
+-rw-r--r--   0        0        0     1293 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/bn.js
+-rw-r--r--   0        0        0      967 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/bs.js
+-rw-r--r--   0        0        0      902 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/ca.js
+-rw-r--r--   0        0        0     1294 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/cs.js
+-rw-r--r--   0        0        0      830 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/da.js
+-rw-r--r--   0        0        0      868 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/de.js
+-rw-r--r--   0        0        0     1019 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/dsb.js
+-rw-r--r--   0        0        0     1184 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/el.js
+-rw-r--r--   0        0        0      846 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/en.js
+-rw-r--r--   0        0        0      924 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/es.js
+-rw-r--r--   0        0        0      803 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/et.js
+-rw-r--r--   0        0        0      870 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/eu.js
+-rw-r--r--   0        0        0     1025 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/fa.js
+-rw-r--r--   0        0        0      805 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/fi.js
+-rw-r--r--   0        0        0      926 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/fr.js
+-rw-r--r--   0        0        0      926 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/gl.js
+-rw-r--r--   0        0        0      986 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/he.js
+-rw-r--r--   0        0        0     1177 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/hi.js
+-rw-r--r--   0        0        0      854 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/hr.js
+-rw-r--r--   0        0        0     1020 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/hsb.js
+-rw-r--r--   0        0        0      833 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/hu.js
+-rw-r--r--   0        0        0     1030 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/hy.js
+-rw-r--r--   0        0        0      770 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/id.js
+-rw-r--r--   0        0        0      809 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/is.js
+-rw-r--r--   0        0        0      899 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/it.js
+-rw-r--r--   0        0        0      864 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/ja.js
+-rw-r--r--   0        0        0     1197 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/ka.js
+-rw-r--r--   0        0        0     1090 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/km.js
+-rw-r--r--   0        0        0      857 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/ko.js
+-rw-r--r--   0        0        0      946 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/lt.js
+-rw-r--r--   0        0        0      902 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/lv.js
+-rw-r--r--   0        0        0     1040 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/mk.js
+-rw-r--r--   0        0        0      813 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/ms.js
+-rw-r--r--   0        0        0      780 2021-03-21 23:27:39.852867 ephios-0.9.3/ephios/static/select2/js/i18n/nb.js
+-rw-r--r--   0        0        0     1359 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/i18n/ne.js
+-rw-r--r--   0        0        0      906 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/i18n/nl.js
+-rw-r--r--   0        0        0      949 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/i18n/pl.js
+-rw-r--r--   0        0        0     1051 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/i18n/ps.js
+-rw-r--r--   0        0        0      878 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/i18n/pt-BR.js
+-rw-r--r--   0        0        0      880 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/i18n/pt.js
+-rw-r--r--   0        0        0      940 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/i18n/ro.js
+-rw-r--r--   0        0        0     1173 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/i18n/ru.js
+-rw-r--r--   0        0        0     1308 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/i18n/sk.js
+-rw-r--r--   0        0        0      927 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/i18n/sl.js
+-rw-r--r--   0        0        0      905 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/i18n/sq.js
+-rw-r--r--   0        0        0     1111 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/i18n/sr-Cyrl.js
+-rw-r--r--   0        0        0      982 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/i18n/sr.js
+-rw-r--r--   0        0        0      788 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/i18n/sv.js
+-rw-r--r--   0        0        0     1076 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/i18n/th.js
+-rw-r--r--   0        0        0      773 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/i18n/tk.js
+-rw-r--r--   0        0        0      777 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/i18n/tr.js
+-rw-r--r--   0        0        0     1158 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/i18n/uk.js
+-rw-r--r--   0        0        0      798 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/i18n/vi.js
+-rw-r--r--   0        0        0      770 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/i18n/zh-CN.js
+-rw-r--r--   0        0        0      709 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/i18n/zh-TW.js
+-rw-r--r--   0        0        0   180386 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/select2.full.js
+-rw-r--r--   0        0        0    79213 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/select2.full.min.js
+-rw-r--r--   0        0        0   159697 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/select2.js
+-rw-r--r--   0        0        0    70892 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/select2/js/select2.min.js
+-rw-r--r--   0        0        0     1106 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/sortablejs/LICENSE
+-rw-r--r--   0        0        0    43304 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/static/sortablejs/Sortable.min.js
+-rw-r--r--   0        0        0      356 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/templates/400.html
+-rw-r--r--   0        0        0      309 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/templates/403.html
+-rw-r--r--   0        0        0      297 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/templates/404.html
+-rw-r--r--   0        0        0      372 2021-03-27 14:26:48.977753 ephios-0.9.3/ephios/templates/500.html
+-rw-r--r--   0        0        0     9178 2021-08-03 16:16:25.859939 ephios-0.9.3/ephios/templates/base.html
+-rw-r--r--   0        0        0      250 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/templates/email_base.html
+-rw-r--r--   0        0        0      288 2021-05-04 20:28:57.970408 ephios-0.9.3/ephios/templates/offline.html
+-rw-r--r--   0        0        0      290 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/templates/registration/logged_out.html
+-rw-r--r--   0        0        0      536 2021-07-03 12:30:08.206321 ephios-0.9.3/ephios/templates/registration/login.html
+-rw-r--r--   0        0        0      323 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/templates/registration/password_change_done.html
+-rw-r--r--   0        0        0      412 2021-03-21 23:27:39.868499 ephios-0.9.3/ephios/templates/registration/password_change_form.html
+-rw-r--r--   0        0        0      385 2021-03-21 23:27:39.884125 ephios-0.9.3/ephios/templates/registration/password_reset_complete.html
+-rw-r--r--   0        0        0      805 2021-03-21 23:27:39.884125 ephios-0.9.3/ephios/templates/registration/password_reset_confirm.html
+-rw-r--r--   0        0        0      388 2021-03-21 23:27:39.884125 ephios-0.9.3/ephios/templates/registration/password_reset_done.html
+-rw-r--r--   0        0        0      419 2021-03-21 23:27:39.884125 ephios-0.9.3/ephios/templates/registration/password_reset_form.html
+-rw-r--r--   0        0        0     1639 2021-05-04 20:28:57.970408 ephios-0.9.3/ephios/urls.py
+-rw-r--r--   0        0        0      405 2021-03-21 23:27:39.884125 ephios-0.9.3/ephios/wsgi.py
+-rw-r--r--   0        0        0     1088 2021-03-21 23:27:39.730437 ephios-0.9.3/LICENSE
+-rw-r--r--   0        0        0     2733 2021-10-10 21:33:22.919324 ephios-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     1936 2021-03-21 23:27:39.730437 ephios-0.9.3/README.md
+-rw-r--r--   0        0        0     5791 2021-10-10 21:33:55.226117 ephios-0.9.3/setup.py
+-rw-r--r--   0        0        0     3732 2021-10-10 21:33:55.226117 ephios-0.9.3/PKG-INFO
```

### Comparing `ephios-0.9.2/ephios/__main__.py` & `ephios-0.9.3/ephios/__main__.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/admin.py` & `ephios-0.9.3/ephios/core/admin.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/calendar.py` & `ephios-0.9.3/ephios/core/calendar.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/consequences.py` & `ephios-0.9.3/ephios/core/consequences.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/context.py` & `ephios-0.9.3/ephios/core/context.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/dynamic_preferences_registry.py` & `ephios-0.9.3/ephios/core/dynamic_preferences_registry.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/forms/events.py` & `ephios-0.9.3/ephios/core/forms/events.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/forms/users.py` & `ephios-0.9.3/ephios/core/forms/users.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/ical.py` & `ephios-0.9.3/ephios/core/ical.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/migrations/0001_initial.py` & `ephios-0.9.3/ephios/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/migrations/0001_squashed_0008_auto_20210207_1309.py` & `ephios-0.9.3/ephios/core/migrations/0001_squashed_0008_auto_20210207_1309.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/migrations/0001_squashed_event_management_0007_auto_20210207_1309.py` & `ephios-0.9.3/ephios/core/migrations/0001_squashed_event_management_0007_auto_20210207_1309.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/migrations/0002_initial_permissions.py` & `ephios-0.9.3/ephios/core/migrations/0002_initial_permissions.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/migrations/0002_merge_content_type_20210208_0020.py` & `ephios-0.9.3/ephios/core/migrations/0002_merge_content_type_20210208_0020.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/migrations/0003_migrate_content_type_to_core_20210219_1642.py` & `ephios-0.9.3/ephios/core/migrations/0003_migrate_content_type_to_core_20210219_1642.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/migrations/0003_userprofile_calendar_token_squashed_0008_auto_20200925_1640.py` & `ephios-0.9.3/ephios/core/migrations/0003_userprofile_calendar_token_squashed_0008_auto_20200925_1640.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/migrations/0004_auto_20201014_1648.py` & `ephios-0.9.3/ephios/core/migrations/0004_auto_20201014_1648.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/migrations/0004_auto_20210305_1855.py` & `ephios-0.9.3/ephios/core/migrations/0004_auto_20210305_1855.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/migrations/0005_auto_20210106_2219.py` & `ephios-0.9.3/ephios/core/migrations/0005_auto_20210106_2219.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/migrations/0006_auto_20210109_2230.py` & `ephios-0.9.3/ephios/core/migrations/0006_auto_20210109_2230.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/migrations/0006_notification.py` & `ephios-0.9.3/ephios/core/migrations/0006_notification.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/migrations/0007_auto_20210110_0050.py` & `ephios-0.9.3/ephios/core/migrations/0007_auto_20210110_0050.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/migrations/0007_auto_20210324_2101.py` & `ephios-0.9.3/ephios/core/migrations/0007_auto_20210324_2101.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/migrations/0008_auto_20210207_1309.py` & `ephios-0.9.3/ephios/core/migrations/0008_auto_20210207_1309.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/migrations/0008_auto_20210403_2348.py` & `ephios-0.9.3/ephios/core/migrations/0008_auto_20210403_2348.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/migrations/0009_auto_20210528_2230.py` & `ephios-0.9.3/ephios/core/migrations/0009_auto_20210528_2230.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/migrations/0010_placeholderparticipation.py` & `ephios-0.9.3/ephios/core/migrations/0010_placeholderparticipation.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/migrations/0011_auto_20210903_1258.py` & `ephios-0.9.3/ephios/core/migrations/0011_auto_20210903_1258.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/models/events.py` & `ephios-0.9.3/ephios/core/models/events.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/models/users.py` & `ephios-0.9.3/ephios/core/models/users.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import functools
 import secrets
 import uuid
 from datetime import date
 from itertools import chain
 
 import guardian.mixins
@@ -147,35 +148,35 @@
             state__in=with_participation_state_in
         ).values_list("shift", flat=True)
         return Shift.objects.filter(pk__in=shift_ids).select_related("event")
 
     def get_workhour_items(self):
         from ephios.core.models import AbstractParticipation
 
-        participation = (
+        participations = (
             self.localparticipation_set.filter(state=AbstractParticipation.States.CONFIRMED)
             .annotate(
-                hours=ExpressionWrapper(
-                    (
-                        F("shift__end_time") - F("shift__start_time")
-                    ),  # calculate length of shift in μs
-                    output_field=models.IntegerField(),
-                )
-                / 1000000
-                / 3600,  # convert microseconds to seconds to hours
+                duration=ExpressionWrapper(
+                    (F("shift__end_time") - F("shift__start_time")),
+                    output_field=models.DurationField(),
+                ),
                 date=ExpressionWrapper(TruncDate(F("shift__start_time")), output_field=DateField()),
                 reason=F("shift__event__title"),
             )
-            .values("hours", "date", "reason")
+            .values("duration", "date", "reason")
         )
-        workinghours = self.workinghours_set.all().values("hours", "date", "reason")
-        hour_sum = (participation.aggregate(Sum("hours"))["hours__sum"] or 0) + (
-            workinghours.aggregate(Sum("hours"))["hours__sum"] or 0
+        workinghours = self.workinghours_set.annotate(duration=F("hours")).values(
+            "duration", "date", "reason"
         )
-        return hour_sum, list(sorted(chain(participation, workinghours), key=lambda k: k["date"]))
+        hour_sum = (
+            participations.aggregate(Sum("duration"))["duration__sum"] or datetime.timedelta()
+        ) + datetime.timedelta(
+            hours=float(workinghours.aggregate(Sum("duration"))["duration__sum"] or 0)
+        )
+        return hour_sum, list(sorted(chain(participations, workinghours), key=lambda k: k["date"]))
 
 
 register_model_for_logging(
     UserProfile,
     ModelFieldsLogConfig(
         unlogged_fields={"id", "password", "calendar_token", "last_login"},
     ),
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ephios-0.9.2/ephios/core/pdf.py` & `ephios-0.9.3/ephios/core/pdf.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/plugins.py` & `ephios-0.9.3/ephios/core/plugins.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/services/notifications/backends.py` & `ephios-0.9.3/ephios/core/services/notifications/backends.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/services/notifications/types.py` & `ephios-0.9.3/ephios/core/services/notifications/types.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/services/participation.py` & `ephios-0.9.3/ephios/core/services/participation.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/services/password_reset.py` & `ephios-0.9.3/ephios/core/services/password_reset.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/signals.py` & `ephios-0.9.3/ephios/core/signals.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/signup/disposition.py` & `ephios-0.9.3/ephios/core/signup/disposition.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/signup/methods.py` & `ephios-0.9.3/ephios/core/signup/methods.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/disposition/disposition.html` & `ephios-0.9.3/ephios/core/templates/core/disposition/disposition.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/disposition/fragment_participation.html` & `ephios-0.9.3/ephios/core/templates/core/disposition/fragment_participation.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/event_archive.html` & `ephios-0.9.3/ephios/core/templates/core/event_archive.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/event_bulk_delete.html` & `ephios-0.9.3/ephios/core/templates/core/event_bulk_delete.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/event_calendar.html` & `ephios-0.9.3/ephios/core/templates/core/event_calendar.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/event_confirm_delete.html` & `ephios-0.9.3/ephios/core/templates/core/event_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/event_copy.html` & `ephios-0.9.3/ephios/core/templates/core/event_copy.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/event_detail.html` & `ephios-0.9.3/ephios/core/templates/core/event_detail.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/event_form.html` & `ephios-0.9.3/ephios/core/templates/core/event_form.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/event_list.html` & `ephios-0.9.3/ephios/core/templates/core/event_list.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/event_notification.html` & `ephios-0.9.3/ephios/core/templates/core/event_notification.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/eventtype_confirm_delete.html` & `ephios-0.9.3/ephios/core/templates/core/eventtype_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/eventtype_form.html` & `ephios-0.9.3/ephios/core/templates/core/eventtype_form.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/eventtype_list.html` & `ephios-0.9.3/ephios/core/templates/core/eventtype_list.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/fragments/approve_consequences.html` & `ephios-0.9.3/ephios/core/templates/core/fragments/approve_consequences.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/fragments/pending_consequences.html` & `ephios-0.9.3/ephios/core/templates/core/fragments/pending_consequences.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/fragments/shift_box_big.html` & `ephios-0.9.3/ephios/core/templates/core/fragments/shift_box_big.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/fragments/shift_box_small.html` & `ephios-0.9.3/ephios/core/templates/core/fragments/shift_box_small.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/fragments/signup_stats_indicator.html` & `ephios-0.9.3/ephios/core/templates/core/fragments/signup_stats_indicator.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/group_confirm_delete.html` & `ephios-0.9.3/ephios/core/templates/core/group_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/group_form.html` & `ephios-0.9.3/ephios/core/templates/core/group_form.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/group_list.html` & `ephios-0.9.3/ephios/core/templates/core/group_list.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/home.html` & `ephios-0.9.3/ephios/core/templates/core/home.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/logentry_list.html` & `ephios-0.9.3/ephios/core/templates/core/logentry_list.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/mails/new_event.html` & `ephios-0.9.3/ephios/core/templates/core/mails/new_event.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/pagination.html` & `ephios-0.9.3/ephios/core/templates/core/pagination.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/settings/settings_base.html` & `ephios-0.9.3/ephios/core/templates/core/settings/settings_base.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/shift_confirm_delete.html` & `ephios-0.9.3/ephios/core/templates/core/shift_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/shift_form.html` & `ephios-0.9.3/ephios/core/templates/core/shift_form.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/userprofile_confirm_delete.html` & `ephios-0.9.3/ephios/core/templates/core/userprofile_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/userprofile_confirm_password_reset.html` & `ephios-0.9.3/ephios/core/templates/core/userprofile_confirm_password_reset.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/userprofile_detail.html` & `ephios-0.9.3/ephios/core/templates/core/userprofile_detail.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% extends "base.html" %}
+{% load utils %}
 {% load user_extras %}
 {% load static %}
 {% load i18n %}
 
 {% block title %}
     {% trans "Profile" %}
 {% endblock %}
@@ -73,22 +74,22 @@
         <ul class="list-group list-group-flush">
             {% with userprofile|workhour_items as workhour_items %}
                 {% for item in workhour_items.1 %}
                     <li class="list-group-item flex-column">
                         <div class="d-flex w-100 justify-content-between align-items-start">
                             <span class="me-1">{{ item.date|date:"SHORT_DATE_FORMAT" }}</span>
                             <span class="flex-grow-1 me-2 break-word">{{ item.reason }}</span>
-                            <span class="text-nowrap">{{ item.hours|floatformat:2 }} {% translate "hours" %}</span>
+                            <span class="text-nowrap">{{ item.duration|timedelta_in_hours }} {% translate "hours" %}</span>
                         </div>
                     </li>
                 {% endfor %}
                 <li class="list-group-item flex-column">
                     <div class="d-flex w-100 justify-content-between align-items-center">
                         <b>{% translate "Total" %}</b>
-                        <span>{{ workhour_items.0|floatformat:2 }} {% translate "hours" %}</span>
+                        <span>{{ workhour_items.0|timedelta_in_hours }} {% translate "hours" %}</span>
                     </div>
                 </li>
             {% endwith %}
         </ul>
     </div>
 {% endblock %}
```

### Comparing `ephios-0.9.2/ephios/core/templates/core/userprofile_form.html` & `ephios-0.9.3/ephios/core/templates/core/userprofile_form.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/userprofile_list.html` & `ephios-0.9.3/ephios/core/templates/core/userprofile_list.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templates/core/userprofile_notifications.html` & `ephios-0.9.3/ephios/core/templates/core/userprofile_notifications.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templatetags/event_extras.py` & `ephios-0.9.3/ephios/core/templatetags/event_extras.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/templatetags/user_extras.py` & `ephios-0.9.3/ephios/core/templatetags/user_extras.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/urls.py` & `ephios-0.9.3/ephios/core/urls.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/views/accounts.py` & `ephios-0.9.3/ephios/core/views/accounts.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/views/bulk.py` & `ephios-0.9.3/ephios/core/views/bulk.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/views/consequences.py` & `ephios-0.9.3/ephios/core/views/consequences.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/views/event.py` & `ephios-0.9.3/ephios/core/views/event.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/views/eventtype.py` & `ephios-0.9.3/ephios/core/views/eventtype.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/views/log.py` & `ephios-0.9.3/ephios/core/views/log.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/views/pwa.py` & `ephios-0.9.3/ephios/core/views/pwa.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/views/settings.py` & `ephios-0.9.3/ephios/core/views/settings.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/views/shift.py` & `ephios-0.9.3/ephios/core/views/shift.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/views/signup.py` & `ephios-0.9.3/ephios/core/views/signup.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/core/widgets.py` & `ephios-0.9.3/ephios/core/widgets.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/extra/bootstrap.py` & `ephios-0.9.3/ephios/extra/bootstrap.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/extra/colors.py` & `ephios-0.9.3/ephios/extra/colors.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/extra/crispy.py` & `ephios-0.9.3/ephios/extra/crispy.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/extra/fields.py` & `ephios-0.9.3/ephios/extra/fields.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/extra/json.py` & `ephios-0.9.3/ephios/extra/json.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/extra/management/commands/devdata.py` & `ephios-0.9.3/ephios/extra/management/commands/devdata.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/extra/mixins.py` & `ephios-0.9.3/ephios/extra/mixins.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/extra/permissions.py` & `ephios-0.9.3/ephios/extra/permissions.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/extra/preferences.py` & `ephios-0.9.3/ephios/extra/preferences.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/extra/templatetags/rich_text.py` & `ephios-0.9.3/ephios/extra/templatetags/rich_text.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/extra/widgets.py` & `ephios-0.9.3/ephios/extra/widgets.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/locale/de/LC_MESSAGES/django.po` & `ephios-0.9.3/ephios/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/modellogging/json.py` & `ephios-0.9.3/ephios/modellogging/json.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/modellogging/log.py` & `ephios-0.9.3/ephios/modellogging/log.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/modellogging/middleware.py` & `ephios-0.9.3/ephios/modellogging/middleware.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/modellogging/migrations/0001_initial.py` & `ephios-0.9.3/ephios/modellogging/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/modellogging/migrations/0002_auto_20210403_2348.py` & `ephios-0.9.3/ephios/modellogging/migrations/0002_auto_20210403_2348.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/modellogging/migrations/0004_alter_logentry_user.py` & `ephios-0.9.3/ephios/modellogging/migrations/0004_alter_logentry_user.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/modellogging/models.py` & `ephios-0.9.3/ephios/modellogging/models.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/modellogging/recorders.py` & `ephios-0.9.3/ephios/modellogging/recorders.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/modellogging/templates/modellogging/logentry.html` & `ephios-0.9.3/ephios/modellogging/templates/modellogging/logentry.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/modellogging/templates/modellogging/logentry_grouped_list.html` & `ephios-0.9.3/ephios/modellogging/templates/modellogging/logentry_grouped_list.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/modellogging/templates/modellogging/statement.html` & `ephios-0.9.3/ephios/modellogging/templates/modellogging/statement.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/modellogging/templatetags/logentries.py` & `ephios-0.9.3/ephios/modellogging/templatetags/logentries.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/basesignup/signals.py` & `ephios-0.9.3/ephios/plugins/basesignup/signals.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/basesignup/signup/common.py` & `ephios-0.9.3/ephios/plugins/basesignup/signup/common.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/basesignup/signup/coupled_signup.py` & `ephios-0.9.3/ephios/plugins/basesignup/signup/coupled_signup.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/basesignup/signup/instant.py` & `ephios-0.9.3/ephios/plugins/basesignup/signup/instant.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/basesignup/signup/no_selfservice.py` & `ephios-0.9.3/ephios/plugins/basesignup/signup/no_selfservice.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/basesignup/signup/request_confirm.py` & `ephios-0.9.3/ephios/plugins/basesignup/signup/request_confirm.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/basesignup/signup/section_based.py` & `ephios-0.9.3/ephios/plugins/basesignup/signup/section_based.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/basesignup/templates/basesignup/fragment_state_common.html` & `ephios-0.9.3/ephios/plugins/basesignup/templates/basesignup/fragment_state_common.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/basesignup/templates/basesignup/participation_card_inline.html` & `ephios-0.9.3/ephios/plugins/basesignup/templates/basesignup/participation_card_inline.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/basesignup/templates/basesignup/section_based/configuration_form.html` & `ephios-0.9.3/ephios/plugins/basesignup/templates/basesignup/section_based/configuration_form.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/basesignup/templates/basesignup/section_based/fragment_participant.html` & `ephios-0.9.3/ephios/plugins/basesignup/templates/basesignup/section_based/fragment_participant.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/basesignup/templates/basesignup/section_based/fragment_state.html` & `ephios-0.9.3/ephios/plugins/basesignup/templates/basesignup/section_based/fragment_state.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/basesignup/templates/basesignup/section_based/signup.html` & `ephios-0.9.3/ephios/plugins/basesignup/templates/basesignup/section_based/signup.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/eventautoqualification/apps.py` & `ephios-0.9.3/ephios/plugins/eventautoqualification/apps.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/eventautoqualification/consequences.py` & `ephios-0.9.3/ephios/plugins/eventautoqualification/consequences.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/eventautoqualification/forms.py` & `ephios-0.9.3/ephios/plugins/eventautoqualification/forms.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/eventautoqualification/migrations/0001_initial.py` & `ephios-0.9.3/ephios/plugins/eventautoqualification/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/eventautoqualification/migrations/0002_auto_20210403_2348.py` & `ephios-0.9.3/ephios/plugins/eventautoqualification/migrations/0002_auto_20210403_2348.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/eventautoqualification/migrations/0003_alter_eventautoqualificationconfiguration_id.py` & `ephios-0.9.3/ephios/plugins/eventautoqualification/migrations/0003_alter_eventautoqualificationconfiguration_id.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/eventautoqualification/models.py` & `ephios-0.9.3/ephios/plugins/eventautoqualification/models.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/eventautoqualification/signals.py` & `ephios-0.9.3/ephios/plugins/eventautoqualification/signals.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/guests/apps.py` & `ephios-0.9.3/ephios/plugins/guests/apps.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/guests/forms.py` & `ephios-0.9.3/ephios/plugins/guests/forms.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/guests/migrations/0001_initial.py` & `ephios-0.9.3/ephios/plugins/guests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/guests/migrations/0002_auto_20210403_2348.py` & `ephios-0.9.3/ephios/plugins/guests/migrations/0002_auto_20210403_2348.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/guests/migrations/0003_auto_20210528_2230.py` & `ephios-0.9.3/ephios/plugins/guests/migrations/0003_auto_20210528_2230.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/guests/models.py` & `ephios-0.9.3/ephios/plugins/guests/models.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/guests/signals.py` & `ephios-0.9.3/ephios/plugins/guests/signals.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/guests/templates/guests/guestuser_form.html` & `ephios-0.9.3/ephios/plugins/guests/templates/guests/guestuser_form.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/guests/urls.py` & `ephios-0.9.3/ephios/plugins/guests/urls.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/guests/views.py` & `ephios-0.9.3/ephios/plugins/guests/views.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/pages/apps.py` & `ephios-0.9.3/ephios/plugins/pages/apps.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/pages/migrations/0001_initial.py` & `ephios-0.9.3/ephios/plugins/pages/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/pages/signals.py` & `ephios-0.9.3/ephios/plugins/pages/signals.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/pages/templates/pages/page_confirm_delete.html` & `ephios-0.9.3/ephios/plugins/pages/templates/pages/page_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/pages/templates/pages/page_form.html` & `ephios-0.9.3/ephios/plugins/pages/templates/pages/page_form.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/pages/templates/pages/page_list.html` & `ephios-0.9.3/ephios/plugins/pages/templates/pages/page_list.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/pages/urls.py` & `ephios-0.9.3/ephios/plugins/pages/urls.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/pages/views.py` & `ephios-0.9.3/ephios/plugins/pages/views.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/qualification_management/dynamic_preferences_registry.py` & `ephios-0.9.3/ephios/plugins/qualification_management/dynamic_preferences_registry.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/qualification_management/forms.py` & `ephios-0.9.3/ephios/plugins/qualification_management/forms.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/qualification_management/importing.py` & `ephios-0.9.3/ephios/plugins/qualification_management/importing.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/qualification_management/serializers.py` & `ephios-0.9.3/ephios/plugins/qualification_management/serializers.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/qualification_management/signals.py` & `ephios-0.9.3/ephios/plugins/qualification_management/signals.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/qualification_management/templates/core/qualification_confirm_delete.html` & `ephios-0.9.3/ephios/plugins/qualification_management/templates/core/qualification_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/qualification_management/templates/core/qualification_form.html` & `ephios-0.9.3/ephios/plugins/qualification_management/templates/core/qualification_form.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/qualification_management/templates/core/qualification_list.html` & `ephios-0.9.3/ephios/plugins/qualification_management/templates/core/qualification_list.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/qualification_management/templates/core/qualificationcategories_form.html` & `ephios-0.9.3/ephios/plugins/qualification_management/templates/core/qualificationcategories_form.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/qualification_management/urls.py` & `ephios-0.9.3/ephios/plugins/qualification_management/urls.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/plugins/qualification_management/views.py` & `ephios-0.9.3/ephios/plugins/qualification_management/views.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/settings.py` & `ephios-0.9.3/ephios/settings.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.bundle.js` & `ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.bundle.js.map` & `ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.bundle.min.js` & `ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.bundle.min.js.map` & `ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.esm.js` & `ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.esm.js.map` & `ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.esm.min.js` & `ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.esm.min.js.map` & `ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.js` & `ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.js.map` & `ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.min.js` & `ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/js/bootstrap.min.js.map` & `ephios-0.9.3/ephios/static/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/LICENSE` & `ephios-0.9.3/ephios/static/bootstrap/LICENSE`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_accordion.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_accordion.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_alert.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_alert.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_badge.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_badge.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_breadcrumb.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_button-group.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_button-group.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_buttons.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_buttons.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_card.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_card.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_carousel.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_carousel.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_close.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_close.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_containers.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_containers.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_dropdown.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_functions.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_functions.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_images.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_images.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_list-group.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_list-group.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_mixins.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_modal.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_modal.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_nav.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_navbar.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_navbar.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_offcanvas.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_offcanvas.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_pagination.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_pagination.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_popover.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_popover.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_progress.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_progress.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_reboot.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_reboot.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_root.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_root.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_spinners.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_spinners.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_tables.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_tables.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_toasts.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_toasts.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_tooltip.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_type.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_type.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_utilities.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_utilities.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/_variables.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/bootstrap-grid.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/bootstrap-reboot.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/bootstrap-reboot.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/bootstrap.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/forms/_floating-labels.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/forms/_form-check.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/forms/_form-control.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/forms/_form-range.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/forms/_form-select.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/forms/_input-group.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/forms/_labels.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/helpers/_position.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/helpers/_position.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_border-radius.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_breakpoints.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_buttons.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_caret.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_deprecate.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_forms.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_gradients.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_grid.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_list-group.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_list-group.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_pagination.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_pagination.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_reset-text.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_reset-text.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_table-variants.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_transition.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_utilities.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/mixins/_visually-hidden.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/utilities/_api.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/bootstrap/scss/vendor/_rfs.scss` & `ephios-0.9.3/ephios/static/bootstrap/scss/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/clipboardjs/js/clipboard.min.js` & `ephios-0.9.3/ephios/static/clipboardjs/js/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/ephios/img/ephios-1024x.png` & `ephios-0.9.3/ephios/static/ephios/img/ephios-1024x.png`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/ephios/img/ephios-192x.png` & `ephios-0.9.3/ephios/static/ephios/img/ephios-192x.png`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/ephios/img/ephios-512x.png` & `ephios-0.9.3/ephios/static/ephios/img/ephios-512x.png`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/ephios/img/ephios-symbol-red.svg` & `ephios-0.9.3/ephios/static/ephios/img/ephios-symbol-red.svg`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/ephios/img/ephios-text-black.png` & `ephios-0.9.3/ephios/static/ephios/img/ephios-text-black.png`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/ephios/img/mannequin_confirmed.svg` & `ephios-0.9.3/ephios/static/ephios/img/mannequin_confirmed.svg`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/ephios/img/mannequin_denied.svg` & `ephios-0.9.3/ephios/static/ephios/img/mannequin_denied.svg`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/ephios/img/mannequin_neutral.svg` & `ephios-0.9.3/ephios/static/ephios/img/mannequin_neutral.svg`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/ephios/img/mannequin_requested.svg` & `ephios-0.9.3/ephios/static/ephios/img/mannequin_requested.svg`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/ephios/js/consequences.js` & `ephios-0.9.3/ephios/static/ephios/js/consequences.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/ephios/js/event_copy.js` & `ephios-0.9.3/ephios/static/ephios/js/event_copy.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/ephios/js/formset/formset.js` & `ephios-0.9.3/ephios/static/ephios/js/formset/formset.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/ephios/js/formset/LICENSE` & `ephios-0.9.3/ephios/static/ephios/js/formset/LICENSE`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/ephios/js/group_form.js` & `ephios-0.9.3/ephios/static/ephios/js/group_form.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/ephios/js/main.js` & `ephios-0.9.3/ephios/static/ephios/js/main.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/ephios/js/serviceworker.js` & `ephios-0.9.3/ephios/static/ephios/js/serviceworker.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/ephios/js/shift_form.js` & `ephios-0.9.3/ephios/static/ephios/js/shift_form.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/ephios/scss/ephios_bootstrap_variables.scss` & `ephios-0.9.3/ephios/static/ephios/scss/ephios_bootstrap_variables.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/ephios/scss/ephios_custom.scss` & `ephios-0.9.3/ephios/static/ephios/scss/ephios_custom.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/ephios/scss/main.scss` & `ephios-0.9.3/ephios/static/ephios/scss/main.scss`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/fontawesome/css/all.css` & `ephios-0.9.3/ephios/static/fontawesome/css/all.css`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-brands-400.eot` & `ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-brands-400.svg` & `ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-brands-400.ttf` & `ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-brands-400.woff` & `ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-brands-400.woff2` & `ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-regular-400.eot` & `ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-regular-400.svg` & `ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-regular-400.ttf` & `ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-regular-400.woff` & `ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-regular-400.woff2` & `ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-solid-900.eot` & `ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-solid-900.svg` & `ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-solid-900.ttf` & `ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-solid-900.woff` & `ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/fontawesome/webfonts/fa-solid-900.woff2` & `ephios-0.9.3/ephios/static/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/jquery/js/jquery-3.5.1.min.js` & `ephios-0.9.3/ephios/static/jquery/js/jquery-3.5.1.min.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/plugins/basesignup/js/disposition.js` & `ephios-0.9.3/ephios/static/plugins/basesignup/js/disposition.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/css/select2-bootstrap5.min.css` & `ephios-0.9.3/ephios/static/select2/css/select2-bootstrap5.min.css`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/css/select2.css` & `ephios-0.9.3/ephios/static/select2/css/select2.css`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/css/select2.min.css` & `ephios-0.9.3/ephios/static/select2/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/af.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/af.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/ar.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/ar.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/az.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/az.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/bg.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/bg.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/bn.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/bn.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/bs.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/bs.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/ca.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/ca.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/cs.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/cs.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/da.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/da.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/de.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/de.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/dsb.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/dsb.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/el.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/el.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/en.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/en.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/es.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/es.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/et.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/et.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/eu.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/eu.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/fa.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/fa.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/fi.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/fi.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/fr.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/fr.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/gl.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/gl.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/he.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/he.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/hi.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/hi.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/hr.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/hr.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/hsb.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/hsb.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/hu.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/hu.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/hy.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/hy.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/id.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/id.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/is.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/is.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/it.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/it.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/ja.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/ja.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/ka.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/ka.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/km.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/km.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/ko.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/ko.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/lt.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/lt.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/lv.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/lv.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/mk.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/mk.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/ms.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/ms.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/nb.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/nb.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/ne.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/ne.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/nl.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/nl.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/pl.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/pl.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/ps.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/ps.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/pt-BR.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/pt.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/pt.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/ro.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/ro.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/ru.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/ru.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/sk.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/sk.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/sl.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/sl.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/sq.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/sq.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/sr-Cyrl.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/sr.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/sr.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/sv.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/sv.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/th.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/th.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/tk.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/tk.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/tr.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/tr.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/uk.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/uk.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/vi.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/vi.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/zh-CN.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/zh-CN.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/i18n/zh-TW.js` & `ephios-0.9.3/ephios/static/select2/js/i18n/zh-TW.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/select2.full.js` & `ephios-0.9.3/ephios/static/select2/js/select2.full.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/select2.full.min.js` & `ephios-0.9.3/ephios/static/select2/js/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/select2.js` & `ephios-0.9.3/ephios/static/select2/js/select2.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/select2/js/select2.min.js` & `ephios-0.9.3/ephios/static/select2/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/sortablejs/LICENSE` & `ephios-0.9.3/ephios/static/sortablejs/LICENSE`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/static/sortablejs/Sortable.min.js` & `ephios-0.9.3/ephios/static/sortablejs/Sortable.min.js`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/templates/base.html` & `ephios-0.9.3/ephios/templates/base.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/templates/registration/login.html` & `ephios-0.9.3/ephios/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/templates/registration/password_reset_confirm.html` & `ephios-0.9.3/ephios/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/ephios/urls.py` & `ephios-0.9.3/ephios/urls.py`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/LICENSE` & `ephios-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/pyproject.toml` & `ephios-0.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ephios"
-version = "0.9.2"
+version = "0.9.3"
 description = "ephios is a tool to manage shifts for medical services."
 authors = ["Julian Baumann <julian@ephios.de>", "Felix Rindt <felix@ephios.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://ephios.de"
 repository = "https://github.com/ephios-dev/ephios"
 documentation = "https://docs.ephios.de/en/stable/"
```

### Comparing `ephios-0.9.2/README.md` & `ephios-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `ephios-0.9.2/setup.py` & `ephios-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 {':python_version < "3.9"': ['importlib-metadata>=3.7.3,<5.0.0'],
  'mysql': ['mysqlclient>=2.0.1,<3.0.0'],
  'pgsql': ['psycopg2>=2.8.6,<3.0.0'],
  'redis': ['django-redis>=4.12.1,<6.0.0']}
 
 setup_kwargs = {
     'name': 'ephios',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'ephios is a tool to manage shifts for medical services.',
     'long_description': '![tests](https://github.com/ephios-dev/ephios/workflows/tests/badge.svg)\n[![Documentation Status](https://readthedocs.org/projects/ephios/badge/?version=latest)](https://docs.ephios.de/en/latest/?badge=latest)\n[![PyPI](https://img.shields.io/pypi/v/ephios)](https://pypi.org/project/ephios/)\n[![Coverage Status](https://coveralls.io/repos/github/ephios-dev/ephios/badge.svg?branch=main)](https://coveralls.io/github/ephios-dev/ephios?branch=main)\n[![translated by Weblate](https://hosted.weblate.org/widgets/ephios/-/svg-badge.svg)](https://hosted.weblate.org/engage/ephios/)\n\n\n# ephios\n\nephios is a tool to manage shifts for medical services.\nPlanners can create events for which volunteer help is required (e.g. security/medical services, beach patrols, exercises).\nAn event can contain multiple shifts for which different processes can be applied for signup \n(e.g. a direct confirmation for an event or an "application" that has to be accepted first).\nThe volunteers can register for the respective shifts via a clearly arranged web interface.\nThe planners can then assign personnel and have an overview of the current status.\nAround this central feature there are further supporting functions like the management of the volunteers and their\nqualifications or an overview of the volunteer hours worked. A flexible group systems helps to support complex permission\nszenarios. The functionality can be extended using plugins.\n\n## Documentation\nYou can find the documentation for ephios at [Read the Docs](https://docs.ephios.de/en/latest). This includes\nthe user guide and installation instructions.\n\n## Contributing\nContributions to ephios are very welcome. You can find information about contributing at our [Contribution page](https://docs.ephios.de/en/latest/development/contributing.html)\nWe are using Weblate for translations, you can also contribute [there](https://hosted.weblate.org/engage/ephios/).\n',
     'author': 'Julian Baumann',
     'author_email': 'julian@ephios.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://ephios.de',
```

### Comparing `ephios-0.9.2/PKG-INFO` & `ephios-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephios
-Version: 0.9.2
+Version: 0.9.3
 Summary: ephios is a tool to manage shifts for medical services.
 Home-page: https://ephios.de
 License: MIT
 Author: Julian Baumann
 Author-email: julian@ephios.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

