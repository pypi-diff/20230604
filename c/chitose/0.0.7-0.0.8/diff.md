# Comparing `tmp/chitose-0.0.7.tar.gz` & `tmp/chitose-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chitose-0.0.7.tar", max compression
+gzip compressed data, was "chitose-0.0.8.tar", max compression
```

## Comparing `chitose-0.0.7.tar` & `chitose-0.0.8.tar`

### file list

```diff
@@ -1,144 +1,145 @@
--rw-r--r--   0        0        0     1073 2023-05-27 13:16:49.683080 chitose-0.0.7/LICENSE
--rw-r--r--   0        0        0     3483 2023-05-27 13:16:49.683080 chitose-0.0.7/README.md
--rw-r--r--   0        0        0      221 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/__init__.py
--rw-r--r--   0        0        0     8972 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/agent.py
--rw-r--r--   0        0        0      443 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/__init__.py
--rw-r--r--   0        0        0     1070 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/__init__.py
--rw-r--r--   0        0        0     2061 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/actor/__init__.py
--rw-r--r--   0        0        0     5314 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/actor/defs.py
--rw-r--r--   0        0        0      276 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/actor/get_preferences.py
--rw-r--r--   0        0        0      248 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/actor/get_profile.py
--rw-r--r--   0        0        0      259 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/actor/get_profiles.py
--rw-r--r--   0        0        0      415 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/actor/get_suggestions.py
--rw-r--r--   0        0        0      682 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/actor/profile.py
--rw-r--r--   0        0        0      428 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/actor/put_preferences.py
--rw-r--r--   0        0        0      429 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/actor/search_actors.py
--rw-r--r--   0        0        0      397 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/actor/search_actors_typeahead.py
--rw-r--r--   0        0        0      354 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/embed/__init__.py
--rw-r--r--   0        0        0     1717 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/embed/external.py
--rw-r--r--   0        0        0     1343 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/embed/images.py
--rw-r--r--   0        0        0     2511 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/embed/record.py
--rw-r--r--   0        0        0     1145 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/embed/record_with_media.py
--rw-r--r--   0        0        0     3583 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/__init__.py
--rw-r--r--   0        0        0     6930 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/defs.py
--rw-r--r--   0        0        0      999 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/describe_feed_generator.py
--rw-r--r--   0        0        0      926 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/generator.py
--rw-r--r--   0        0        0      424 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/get_actor_feeds.py
--rw-r--r--   0        0        0      401 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/get_author_feed.py
--rw-r--r--   0        0        0      423 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/get_feed.py
--rw-r--r--   0        0        0      349 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/get_feed_generator.py
--rw-r--r--   0        0        0      315 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/get_feed_generators.py
--rw-r--r--   0        0        0      425 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/get_feed_skeleton.py
--rw-r--r--   0        0        0      864 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/get_likes.py
--rw-r--r--   0        0        0      389 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/get_post_thread.py
--rw-r--r--   0        0        0      272 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/get_posts.py
--rw-r--r--   0        0        0      415 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/get_reposted_by.py
--rw-r--r--   0        0        0      439 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/get_timeline.py
--rw-r--r--   0        0        0      480 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/like.py
--rw-r--r--   0        0        0     2470 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/post.py
--rw-r--r--   0        0        0      484 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/feed/repost.py
--rw-r--r--   0        0        0     2889 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/__init__.py
--rw-r--r--   0        0        0      398 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/block.py
--rw-r--r--   0        0        0     2642 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/defs.py
--rw-r--r--   0        0        0      400 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/follow.py
--rw-r--r--   0        0        0      377 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/get_blocks.py
--rw-r--r--   0        0        0      399 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/get_followers.py
--rw-r--r--   0        0        0      395 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/get_follows.py
--rw-r--r--   0        0        0      382 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/get_list.py
--rw-r--r--   0        0        0      390 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/get_list_mutes.py
--rw-r--r--   0        0        0      410 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/get_lists.py
--rw-r--r--   0        0        0      360 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/get_mutes.py
--rw-r--r--   0        0        0      969 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/list.py
--rw-r--r--   0        0        0      459 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/listitem.py
--rw-r--r--   0        0        0      307 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/mute_actor.py
--rw-r--r--   0        0        0      304 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/mute_actor_list.py
--rw-r--r--   0        0        0      313 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/unmute_actor.py
--rw-r--r--   0        0        0      310 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/graph/unmute_actor_list.py
--rw-r--r--   0        0        0     1131 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/notification/__init__.py
--rw-r--r--   0        0        0      305 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/notification/get_unread_count.py
--rw-r--r--   0        0        0     1603 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/notification/list_notifications.py
--rw-r--r--   0        0        0      341 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/notification/update_seen.py
--rw-r--r--   0        0        0      357 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/richtext/__init__.py
--rw-r--r--   0        0        0     1327 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/richtext/facet.py
--rw-r--r--   0        0        0      930 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/unspecced/__init__.py
--rw-r--r--   0        0        0      459 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/unspecced/get_popular.py
--rw-r--r--   0        0        0      307 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/app/bsky/unspecced/get_popular_feed_generators.py
--rw-r--r--   0        0        0      373 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/blob.py
--rw-r--r--   0        0        0      455 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/__init__.py
--rw-r--r--   0        0        0     1049 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/__init__.py
--rw-r--r--   0        0        0     5659 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/__init__.py
--rw-r--r--   0        0        0    13162 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/defs.py
--rw-r--r--   0        0        0      400 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/disable_account_invites.py
--rw-r--r--   0        0        0      478 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/disable_invite_codes.py
--rw-r--r--   0        0        0      361 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/enable_account_invites.py
--rw-r--r--   0        0        0      456 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/get_invite_codes.py
--rw-r--r--   0        0        0      300 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/get_moderation_action.py
--rw-r--r--   0        0        0      466 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/get_moderation_actions.py
--rw-r--r--   0        0        0      300 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/get_moderation_report.py
--rw-r--r--   0        0        0      747 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/get_moderation_reports.py
--rw-r--r--   0        0        0      331 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/get_record.py
--rw-r--r--   0        0        0      271 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/get_repo.py
--rw-r--r--   0        0        0      451 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/resolve_moderation_reports.py
--rw-r--r--   0        0        0      400 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/reverse_moderation_action.py
--rw-r--r--   0        0        0      500 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/search_repos.py
--rw-r--r--   0        0        0     1023 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/take_moderation_action.py
--rw-r--r--   0        0        0      440 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/update_account_email.py
--rw-r--r--   0        0        0      376 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/admin/update_account_handle.py
--rw-r--r--   0        0        0      794 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/identity/__init__.py
--rw-r--r--   0        0        0      339 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/identity/resolve_handle.py
--rw-r--r--   0        0        0      324 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/identity/update_handle.py
--rw-r--r--   0        0        0      995 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/label/__init__.py
--rw-r--r--   0        0        0     1096 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/label/defs.py
--rw-r--r--   0        0        0      772 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/label/query_labels.py
--rw-r--r--   0        0        0      820 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/label/subscribe_labels.py
--rw-r--r--   0        0        0      896 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/moderation/__init__.py
--rw-r--r--   0        0        0      697 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/moderation/create_report.py
--rw-r--r--   0        0        0      740 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/moderation/defs.py
--rw-r--r--   0        0        0     5516 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/repo/__init__.py
--rw-r--r--   0        0        0     1896 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/repo/apply_writes.py
--rw-r--r--   0        0        0      885 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/repo/create_record.py
--rw-r--r--   0        0        0      846 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/repo/delete_record.py
--rw-r--r--   0        0        0      372 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/repo/describe_repo.py
--rw-r--r--   0        0        0      655 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/repo/get_record.py
--rw-r--r--   0        0        0     1380 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/repo/list_records.py
--rw-r--r--   0        0        0     1028 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/repo/put_record.py
--rw-r--r--   0        0        0      530 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/repo/rebase_repo.py
--rw-r--r--   0        0        0      392 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/repo/strong_ref.py
--rw-r--r--   0        0        0      317 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/repo/upload_blob.py
--rw-r--r--   0        0        0     4261 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/server/__init__.py
--rw-r--r--   0        0        0      569 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/server/create_account.py
--rw-r--r--   0        0        0      729 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/server/create_app_password.py
--rw-r--r--   0        0        0      409 2023-05-27 13:16:49.683080 chitose-0.0.7/chitose/com/atproto/server/create_invite_code.py
--rw-r--r--   0        0        0      789 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/create_invite_codes.py
--rw-r--r--   0        0        0      483 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/create_session.py
--rw-r--r--   0        0        0     1191 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/defs.py
--rw-r--r--   0        0        0      395 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/delete_account.py
--rw-r--r--   0        0        0      255 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/delete_session.py
--rw-r--r--   0        0        0      744 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/describe_server.py
--rw-r--r--   0        0        0      458 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/get_account_invite_codes.py
--rw-r--r--   0        0        0      266 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/get_session.py
--rw-r--r--   0        0        0      596 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/list_app_passwords.py
--rw-r--r--   0        0        0      264 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/refresh_session.py
--rw-r--r--   0        0        0      286 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/request_account_delete.py
--rw-r--r--   0        0        0      352 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/request_password_reset.py
--rw-r--r--   0        0        0      369 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/reset_password.py
--rw-r--r--   0        0        0      334 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/server/revoke_app_password.py
--rw-r--r--   0        0        0     4145 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/__init__.py
--rw-r--r--   0        0        0      392 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/get_blob.py
--rw-r--r--   0        0        0      349 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/get_blocks.py
--rw-r--r--   0        0        0      462 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/get_checkout.py
--rw-r--r--   0        0        0      553 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/get_commit_path.py
--rw-r--r--   0        0        0      318 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/get_head.py
--rw-r--r--   0        0        0      536 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/get_record.py
--rw-r--r--   0        0        0      580 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/get_repo.py
--rw-r--r--   0        0        0      555 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/list_blobs.py
--rw-r--r--   0        0        0      648 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/list_repos.py
--rw-r--r--   0        0        0      492 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/notify_of_update.py
--rw-r--r--   0        0        0      402 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/request_crawl.py
--rw-r--r--   0        0        0     2945 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/com/atproto/sync/subscribe_repos.py
--rw-r--r--   0        0        0      170 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/link.py
--rw-r--r--   0        0        0      136 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/object.py
--rw-r--r--   0        0        0      136 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/record.py
--rw-r--r--   0        0        0     1642 2023-05-27 13:16:49.687080 chitose-0.0.7/chitose/xrpc.py
--rw-r--r--   0        0        0      801 2023-05-27 13:16:49.687080 chitose-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4286 1970-01-01 00:00:00.000000 chitose-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-04 10:04:22.655807 chitose-0.0.8/LICENSE
+-rw-r--r--   0        0        0     3643 2023-06-04 10:04:22.655807 chitose-0.0.8/README.md
+-rw-r--r--   0        0        0      221 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/__init__.py
+-rw-r--r--   0        0        0     9519 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/agent.py
+-rw-r--r--   0        0        0      551 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/__init__.py
+-rw-r--r--   0        0        0     1274 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/__init__.py
+-rw-r--r--   0        0        0     2153 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/actor/__init__.py
+-rw-r--r--   0        0        0     5314 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/actor/defs.py
+-rw-r--r--   0        0        0      272 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/actor/get_preferences.py
+-rw-r--r--   0        0        0      244 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/actor/get_profile.py
+-rw-r--r--   0        0        0      255 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/actor/get_profiles.py
+-rw-r--r--   0        0        0      411 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/actor/get_suggestions.py
+-rw-r--r--   0        0        0      682 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/actor/profile.py
+-rw-r--r--   0        0        0      424 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/actor/put_preferences.py
+-rw-r--r--   0        0        0      425 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/actor/search_actors.py
+-rw-r--r--   0        0        0      393 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/actor/search_actors_typeahead.py
+-rw-r--r--   0        0        0      446 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/embed/__init__.py
+-rw-r--r--   0        0        0     1717 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/embed/external.py
+-rw-r--r--   0        0        0     1343 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/embed/images.py
+-rw-r--r--   0        0        0     2511 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/embed/record.py
+-rw-r--r--   0        0        0     1145 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/embed/record_with_media.py
+-rw-r--r--   0        0        0     3640 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/__init__.py
+-rw-r--r--   0        0        0     6930 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/defs.py
+-rw-r--r--   0        0        0      995 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/describe_feed_generator.py
+-rw-r--r--   0        0        0      926 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/generator.py
+-rw-r--r--   0        0        0      420 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/get_actor_feeds.py
+-rw-r--r--   0        0        0      397 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/get_author_feed.py
+-rw-r--r--   0        0        0      419 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/get_feed.py
+-rw-r--r--   0        0        0      345 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/get_feed_generator.py
+-rw-r--r--   0        0        0      311 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/get_feed_generators.py
+-rw-r--r--   0        0        0      421 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/get_feed_skeleton.py
+-rw-r--r--   0        0        0      860 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/get_likes.py
+-rw-r--r--   0        0        0      385 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/get_post_thread.py
+-rw-r--r--   0        0        0      268 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/get_posts.py
+-rw-r--r--   0        0        0      411 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/get_reposted_by.py
+-rw-r--r--   0        0        0      435 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/get_timeline.py
+-rw-r--r--   0        0        0      480 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/like.py
+-rw-r--r--   0        0        0     2470 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/post.py
+-rw-r--r--   0        0        0      484 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/repost.py
+-rw-r--r--   0        0        0     2981 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/__init__.py
+-rw-r--r--   0        0        0      398 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/block.py
+-rw-r--r--   0        0        0     2642 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/defs.py
+-rw-r--r--   0        0        0      400 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/follow.py
+-rw-r--r--   0        0        0      373 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/get_blocks.py
+-rw-r--r--   0        0        0      395 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/get_followers.py
+-rw-r--r--   0        0        0      391 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/get_follows.py
+-rw-r--r--   0        0        0      378 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/get_list.py
+-rw-r--r--   0        0        0      386 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/get_list_mutes.py
+-rw-r--r--   0        0        0      406 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/get_lists.py
+-rw-r--r--   0        0        0      356 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/get_mutes.py
+-rw-r--r--   0        0        0      969 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/list.py
+-rw-r--r--   0        0        0      459 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/listitem.py
+-rw-r--r--   0        0        0      303 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/mute_actor.py
+-rw-r--r--   0        0        0      300 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/mute_actor_list.py
+-rw-r--r--   0        0        0      309 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/unmute_actor.py
+-rw-r--r--   0        0        0      306 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/unmute_actor_list.py
+-rw-r--r--   0        0        0     1150 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/notification/__init__.py
+-rw-r--r--   0        0        0      301 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/notification/get_unread_count.py
+-rw-r--r--   0        0        0     1599 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/notification/list_notifications.py
+-rw-r--r--   0        0        0      337 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/notification/update_seen.py
+-rw-r--r--   0        0        0      449 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/richtext/__init__.py
+-rw-r--r--   0        0        0     1327 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/richtext/facet.py
+-rw-r--r--   0        0        0     1022 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/unspecced/__init__.py
+-rw-r--r--   0        0        0      455 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/unspecced/get_popular.py
+-rw-r--r--   0        0        0      303 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/unspecced/get_popular_feed_generators.py
+-rw-r--r--   0        0        0      373 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/blob.py
+-rw-r--r--   0        0        0      563 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/__init__.py
+-rw-r--r--   0        0        0     1253 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/__init__.py
+-rw-r--r--   0        0        0     6382 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/__init__.py
+-rw-r--r--   0        0        0    13162 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/defs.py
+-rw-r--r--   0        0        0      396 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/disable_account_invites.py
+-rw-r--r--   0        0        0      474 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/disable_invite_codes.py
+-rw-r--r--   0        0        0      357 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/enable_account_invites.py
+-rw-r--r--   0        0        0      452 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/get_invite_codes.py
+-rw-r--r--   0        0        0      296 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/get_moderation_action.py
+-rw-r--r--   0        0        0      462 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/get_moderation_actions.py
+-rw-r--r--   0        0        0      296 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/get_moderation_report.py
+-rw-r--r--   0        0        0     1009 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/get_moderation_reports.py
+-rw-r--r--   0        0        0      327 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/get_record.py
+-rw-r--r--   0        0        0      267 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/get_repo.py
+-rw-r--r--   0        0        0      534 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/rebase_repo.py
+-rw-r--r--   0        0        0      447 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/resolve_moderation_reports.py
+-rw-r--r--   0        0        0      396 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/reverse_moderation_action.py
+-rw-r--r--   0        0        0      496 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/search_repos.py
+-rw-r--r--   0        0        0     1019 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/take_moderation_action.py
+-rw-r--r--   0        0        0      436 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/update_account_email.py
+-rw-r--r--   0        0        0      372 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/update_account_handle.py
+-rw-r--r--   0        0        0      886 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/identity/__init__.py
+-rw-r--r--   0        0        0      335 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/identity/resolve_handle.py
+-rw-r--r--   0        0        0      320 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/identity/update_handle.py
+-rw-r--r--   0        0        0     1434 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/label/__init__.py
+-rw-r--r--   0        0        0     1096 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/label/defs.py
+-rw-r--r--   0        0        0      768 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/label/query_labels.py
+-rw-r--r--   0        0        0     1145 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/label/subscribe_labels.py
+-rw-r--r--   0        0        0      988 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/moderation/__init__.py
+-rw-r--r--   0        0        0      693 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/moderation/create_report.py
+-rw-r--r--   0        0        0      740 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/moderation/defs.py
+-rw-r--r--   0        0        0     5608 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/repo/__init__.py
+-rw-r--r--   0        0        0     1892 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/repo/apply_writes.py
+-rw-r--r--   0        0        0      881 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/repo/create_record.py
+-rw-r--r--   0        0        0      842 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/repo/delete_record.py
+-rw-r--r--   0        0        0      368 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/repo/describe_repo.py
+-rw-r--r--   0        0        0      651 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/repo/get_record.py
+-rw-r--r--   0        0        0     1376 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/repo/list_records.py
+-rw-r--r--   0        0        0     1024 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/repo/put_record.py
+-rw-r--r--   0        0        0      526 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/repo/rebase_repo.py
+-rw-r--r--   0        0        0      392 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/repo/strong_ref.py
+-rw-r--r--   0        0        0      313 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/repo/upload_blob.py
+-rw-r--r--   0        0        0     4353 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/server/__init__.py
+-rw-r--r--   0        0        0      565 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/server/create_account.py
+-rw-r--r--   0        0        0      725 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/server/create_app_password.py
+-rw-r--r--   0        0        0      405 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/server/create_invite_code.py
+-rw-r--r--   0        0        0      785 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/server/create_invite_codes.py
+-rw-r--r--   0        0        0      479 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/server/create_session.py
+-rw-r--r--   0        0        0     1191 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/server/defs.py
+-rw-r--r--   0        0        0      391 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/server/delete_account.py
+-rw-r--r--   0        0        0      251 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/server/delete_session.py
+-rw-r--r--   0        0        0      740 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/server/describe_server.py
+-rw-r--r--   0        0        0      454 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/server/get_account_invite_codes.py
+-rw-r--r--   0        0        0      262 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/server/get_session.py
+-rw-r--r--   0        0        0      592 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/server/list_app_passwords.py
+-rw-r--r--   0        0        0      260 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/server/refresh_session.py
+-rw-r--r--   0        0        0      282 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/server/request_account_delete.py
+-rw-r--r--   0        0        0      348 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/server/request_password_reset.py
+-rw-r--r--   0        0        0      365 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/server/reset_password.py
+-rw-r--r--   0        0        0      330 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/server/revoke_app_password.py
+-rw-r--r--   0        0        0     4579 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/__init__.py
+-rw-r--r--   0        0        0      388 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/get_blob.py
+-rw-r--r--   0        0        0      345 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/get_blocks.py
+-rw-r--r--   0        0        0      458 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/get_checkout.py
+-rw-r--r--   0        0        0      549 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/get_commit_path.py
+-rw-r--r--   0        0        0      314 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/get_head.py
+-rw-r--r--   0        0        0      532 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/get_record.py
+-rw-r--r--   0        0        0      576 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/get_repo.py
+-rw-r--r--   0        0        0      551 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/list_blobs.py
+-rw-r--r--   0        0        0      644 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/list_repos.py
+-rw-r--r--   0        0        0      488 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/notify_of_update.py
+-rw-r--r--   0        0        0      398 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/request_crawl.py
+-rw-r--r--   0        0        0     3266 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/subscribe_repos.py
+-rw-r--r--   0        0        0      170 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/link.py
+-rw-r--r--   0        0        0      136 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/object.py
+-rw-r--r--   0        0        0      136 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/record.py
+-rw-r--r--   0        0        0     2206 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/xrpc.py
+-rw-r--r--   0        0        0      823 2023-06-04 10:04:22.659807 chitose-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4481 1970-01-01 00:00:00.000000 chitose-0.0.8/PKG-INFO
```

### Comparing `chitose-0.0.7/LICENSE` & `chitose-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chitose-0.0.7/README.md` & `chitose-0.0.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,27 +11,29 @@
 The API of Chitose is similar to [the ATP API](https://github.com/bluesky-social/atproto/blob/main/packages/api/README.md).
 
 For example, you can use `get_timeline()` in `BskyAgent` to get the timeline as shown below. Replace `YOUR_USERNAME` and `YOUR_PASSWORD` with your username and your password respectively:
 
 ```
 $ git clone https://github.com/mnogu/chitose.git
 $ cd chitose
+$ python3 -m pip install -r requirements.txt
 $ python3
 >>> from chitose import BskyAgent
 >>> agent = BskyAgent(service='https://bsky.social')
 >>> agent.login(identifier='YOUR_USERNAME', password='YOUR_PASSWORD')
 >>> agent.get_timeline(limit=1)
 ```
 For available methods in `BskyAgent`, refer to [the documentation of `BskyAgent`](https://chitose.readthedocs.io/en/latest/chitose.html#chitose.BskyAgent).
 
 Alternatively, you can use `app.bsky.feed.get_timeline()` as in [the advanced API calls](https://github.com/bluesky-social/atproto/blob/main/packages/api/README.md#advanced-api-calls):
 
 ```
 $ git clone https://github.com/mnogu/chitose.git
 $ cd chitose
+$ python3 -m pip install -r requirements.txt
 $ python3
 >>> from chitose import BskyAgent
 >>> agent = BskyAgent(service='https://bsky.social')
 >>> agent.login(identifier='YOUR_USERNAME', password='YOUR_PASSWORD')
 >>> agent.app.bsky.feed.get_timeline(limit=1)
 ```
 
@@ -64,14 +66,15 @@
 $ python3 -m pip install chitose
 ```
 
 Alternatively, you can build a Python package and install it:
 ```
 $ git clone https://github.com/mnogu/chitose.git
 $ cd chitose
+$ python3 -m pip install -r requirements.txt
 $ python3 -m pip install --upgrade build
 $ python3 -m build
 $ python3 -m pip install dist/chitose-*-py3-none-any.whl
 ```
 
 ## Generating Code
 
@@ -90,11 +93,11 @@
 
 You may want to add new Python code to the repository or update the documentation:
 ```
 $ git add chitose
 $ git commit
 ```
 ```
-$ python3 -m pip install sphinx
+$ python3 -m pip install -r docs/source/requirements.txt
 $ cd docs
 $ sphinx-apidoc -o ./source ../chitose -f
 ```
```

### Comparing `chitose-0.0.7/chitose/agent.py` & `chitose-0.0.8/chitose/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 from chitose.app.bsky.feed.repost import Repost
 from chitose.app.bsky.graph.follow import Follow
 from chitose.com.atproto.repo.strong_ref import StrongRef
 
 from .app import App_
 from .com import Com_
 from .xrpc import call
+from .xrpc import subscribe
 from .xrpc import XrpcParams
 from .xrpc import XrpcData
+from .xrpc import XrpcHandler
 from .xrpc import XrpcHeaders
 
 
 class BskyAgent:
     def __init__(self, service: str) -> None:
         self.service = service
         self.session: dict[str, str] = {}
@@ -29,18 +31,26 @@
             return headers | {
                 'authorization': f'Bearer {self.session["accessJwt"]}'
             }
 
         return headers
 
     def _refresh_session(self, e: urllib.error.HTTPError):
-        if 'refreshJwt' not in self.session:
+        if e.code != 400 or 'refreshJwt' not in self.session:
             raise e
 
-        error = json.loads(e.read().decode())['error']
+        try:
+            obj = json.loads(e.read())
+        except json.JSONDecodeError:
+            raise e
+
+        if 'error' not in obj:
+            return e
+
+        error = obj['error']
         if error != 'ExpiredToken':
             raise e
 
         self.session = json.loads(
             call('com.atproto.server.refreshSession',
                  [], {}, self.service,
                  {'authorization':
@@ -54,21 +64,28 @@
                         self._add_auth_header(headers))
         except urllib.error.HTTPError as e:
             self._refresh_session(e)
 
             return call(method, params, d, self.service,
                         self._add_auth_header(headers))
 
+    def _subscribe(self, method: str, params: XrpcParams,
+                   handler: XrpcHandler) -> None:
+        # https -> wss
+        scheme = urllib.parse.urlparse(self.service).scheme
+        service = self.service.replace(scheme, 'wss', 1)
+        subscribe(method, params, service, handler)
+
     @property
     def app(self):
-        return App_(self._call)
+        return App_(self._call, self._subscribe)
 
     @property
     def com(self):
-        return Com_(self._call)
+        return Com_(self._call, self._subscribe)
 
     def get_timeline(self, **kwargs: dict[str, typing.Any]) -> bytes:
         """See :doc:`chitose.app.bsky.feed` for available arguments."""
         return self.app.bsky.feed.get_timeline(**kwargs)
 
     def get_author_feed(self, **kwargs: dict[str, typing.Any]) -> bytes:
         """See :doc:`chitose.app.bsky.feed` for available arguments."""
```

### Comparing `chitose-0.0.7/chitose/app/bsky/__init__.py` & `chitose-0.0.8/chitose/app/bsky/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
-from chitose.xrpc import XrpcCallable
+from chitose.xrpc import XrpcCall
+from chitose.xrpc import XrpcSubscribe
 from .actor import Actor_
 from .embed import Embed_
 from .feed import Feed_
 from .graph import Graph_
 from .notification import Notification_
 from .richtext import Richtext_
 from .unspecced import Unspecced_
 
 class Bsky_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
-    def __init__(self, call: XrpcCallable) -> None:
+    def __init__(self, call: XrpcCall, subscribe: XrpcSubscribe) -> None:
         self.call = call
+        self.subscribe = subscribe
 
     @property
     def actor(self):
-        return Actor_(self.call)
+        return Actor_(self.call, self.subscribe)
 
     @property
     def embed(self):
-        return Embed_(self.call)
+        return Embed_(self.call, self.subscribe)
 
     @property
     def feed(self):
-        return Feed_(self.call)
+        return Feed_(self.call, self.subscribe)
 
     @property
     def graph(self):
-        return Graph_(self.call)
+        return Graph_(self.call, self.subscribe)
 
     @property
     def notification(self):
-        return Notification_(self.call)
+        return Notification_(self.call, self.subscribe)
 
     @property
     def richtext(self):
-        return Richtext_(self.call)
+        return Richtext_(self.call, self.subscribe)
 
     @property
     def unspecced(self):
-        return Unspecced_(self.call)
+        return Unspecced_(self.call, self.subscribe)
```

### Comparing `chitose-0.0.7/chitose/app/bsky/actor/__init__.py` & `chitose-0.0.8/chitose/app/bsky/actor/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
-from chitose.xrpc import XrpcCallable
+from chitose.xrpc import XrpcCall
+from chitose.xrpc import XrpcSubscribe
 from .get_preferences import _get_preferences
 from .get_profile import _get_profile
 from .get_profiles import _get_profiles
 from .get_suggestions import _get_suggestions
 from .put_preferences import _put_preferences
 from .search_actors import _search_actors
 from .search_actors_typeahead import _search_actors_typeahead
 import chitose.app.bsky.actor.defs
 import typing
 
 class Actor_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
-    def __init__(self, call: XrpcCallable) -> None:
+    def __init__(self, call: XrpcCall, subscribe: XrpcSubscribe) -> None:
         self.call = call
+        self.subscribe = subscribe
 
     def search_actors_typeahead(self, term: typing.Optional[str]=None, limit: typing.Optional[int]=None) -> bytes:
         """Find actor suggestions for a search term."""
         return _search_actors_typeahead(self.call, term, limit)
 
     def put_preferences(self, preferences: chitose.app.bsky.actor.defs.Preferences) -> bytes:
         """Sets the private preferences attached to the account."""
```

### Comparing `chitose-0.0.7/chitose/app/bsky/actor/defs.py` & `chitose-0.0.8/chitose/app/bsky/actor/defs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.7/chitose/app/bsky/actor/profile.py` & `chitose-0.0.8/chitose/app/bsky/actor/profile.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.7/chitose/app/bsky/embed/external.py` & `chitose-0.0.8/chitose/app/bsky/embed/external.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.7/chitose/app/bsky/embed/images.py` & `chitose-0.0.8/chitose/app/bsky/embed/images.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.7/chitose/app/bsky/embed/record.py` & `chitose-0.0.8/chitose/app/bsky/embed/record.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.7/chitose/app/bsky/embed/record_with_media.py` & `chitose-0.0.8/chitose/app/bsky/embed/record_with_media.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.7/chitose/app/bsky/feed/__init__.py` & `chitose-0.0.8/chitose/app/bsky/feed/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
-from chitose.xrpc import XrpcCallable
+from chitose.xrpc import XrpcCall
+from chitose.xrpc import XrpcSubscribe
 from .describe_feed_generator import _describe_feed_generator
 from .get_actor_feeds import _get_actor_feeds
 from .get_author_feed import _get_author_feed
 from .get_feed import _get_feed
 from .get_feed_generator import _get_feed_generator
 from .get_feed_generators import _get_feed_generators
 from .get_feed_skeleton import _get_feed_skeleton
 from .get_likes import _get_likes
 from .get_post_thread import _get_post_thread
 from .get_posts import _get_posts
 from .get_reposted_by import _get_reposted_by
 from .get_timeline import _get_timeline
-import chitose.app.bsky.actor.defs
 import typing
 
 class Feed_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
-    def __init__(self, call: XrpcCallable) -> None:
+    def __init__(self, call: XrpcCall, subscribe: XrpcSubscribe) -> None:
         self.call = call
+        self.subscribe = subscribe
 
     def get_feed_generators(self, feeds: list[str]) -> bytes:
         """Get information about a list of feed generators"""
         return _get_feed_generators(self.call, feeds)
 
     def get_timeline(self, algorithm: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """A view of the user's home timeline."""
```

### Comparing `chitose-0.0.7/chitose/app/bsky/feed/defs.py` & `chitose-0.0.8/chitose/app/bsky/feed/defs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.7/chitose/app/bsky/feed/describe_feed_generator.py` & `chitose-0.0.8/chitose/app/bsky/feed/describe_feed_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _describe_feed_generator(call: chitose.xrpc.XrpcCallable) -> bytes:
+def _describe_feed_generator(call: chitose.xrpc.XrpcCall) -> bytes:
     """Returns information about a given feed generator including TOS & offered feed URIs"""
     return call('app.bsky.feed.describeFeedGenerator', [], None, {})
 
 class Feed(chitose.Object):
     """"""
 
     def __init__(self, uri: str) -> None:
```

### Comparing `chitose-0.0.7/chitose/app/bsky/feed/generator.py` & `chitose-0.0.8/chitose/app/bsky/feed/generator.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.7/chitose/app/bsky/feed/get_likes.py` & `chitose-0.0.8/chitose/app/bsky/feed/get_likes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import chitose.app.bsky.actor.defs
 import typing
 
-def _get_likes(call: chitose.xrpc.XrpcCallable, uri: str, cid: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
+def _get_likes(call: chitose.xrpc.XrpcCall, uri: str, cid: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
     """"""
     return call('app.bsky.feed.getLikes', [('uri', uri), ('cid', cid), ('limit', limit), ('cursor', cursor)], None, {})
 
 class Like(chitose.Object):
     """"""
 
     def __init__(self, indexed_at: str, created_at: str, actor: chitose.app.bsky.actor.defs.ProfileView) -> None:
```

### Comparing `chitose-0.0.7/chitose/app/bsky/feed/post.py` & `chitose-0.0.8/chitose/app/bsky/feed/post.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.7/chitose/app/bsky/graph/__init__.py` & `chitose-0.0.8/chitose/app/bsky/graph/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
-from chitose.xrpc import XrpcCallable
+from chitose.xrpc import XrpcCall
+from chitose.xrpc import XrpcSubscribe
 from .get_blocks import _get_blocks
 from .get_followers import _get_followers
 from .get_follows import _get_follows
 from .get_list import _get_list
 from .get_list_mutes import _get_list_mutes
 from .get_lists import _get_lists
 from .get_mutes import _get_mutes
@@ -13,16 +14,17 @@
 from .unmute_actor import _unmute_actor
 from .unmute_actor_list import _unmute_actor_list
 import typing
 
 class Graph_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
-    def __init__(self, call: XrpcCallable) -> None:
+    def __init__(self, call: XrpcCall, subscribe: XrpcSubscribe) -> None:
         self.call = call
+        self.subscribe = subscribe
 
     def unmute_actor_list(self, list: str) -> bytes:
         """Unmute a list of actors."""
         return _unmute_actor_list(self.call, list)
 
     def mute_actor_list(self, list: str) -> bytes:
         """Mute a list of actors."""
```

### Comparing `chitose-0.0.7/chitose/app/bsky/graph/defs.py` & `chitose-0.0.8/chitose/app/bsky/graph/defs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.7/chitose/app/bsky/graph/list.py` & `chitose-0.0.8/chitose/app/bsky/graph/list.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.7/chitose/app/bsky/notification/__init__.py` & `chitose-0.0.8/chitose/app/bsky/notification/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
-from chitose.xrpc import XrpcCallable
+from chitose.xrpc import XrpcCall
+from chitose.xrpc import XrpcSubscribe
 from .get_unread_count import _get_unread_count
 from .list_notifications import _list_notifications
 from .update_seen import _update_seen
-import chitose.app.bsky.actor.defs
-import chitose.com.atproto.label.defs
 import typing
 
 class Notification_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
-    def __init__(self, call: XrpcCallable) -> None:
+    def __init__(self, call: XrpcCall, subscribe: XrpcSubscribe) -> None:
         self.call = call
+        self.subscribe = subscribe
 
     def update_seen(self, seen_at: str) -> bytes:
         """Notify server that the user has seen notifications."""
         return _update_seen(self.call, seen_at)
 
     def list_notifications(self, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, seen_at: typing.Optional[str]=None) -> bytes:
         """"""
```

### Comparing `chitose-0.0.7/chitose/app/bsky/notification/list_notifications.py` & `chitose-0.0.8/chitose/app/bsky/notification/list_notifications.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """"""
 from __future__ import annotations
 import chitose
 import chitose.app.bsky.actor.defs
 import chitose.com.atproto.label.defs
 import typing
 
-def _list_notifications(call: chitose.xrpc.XrpcCallable, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, seen_at: typing.Optional[str]=None) -> bytes:
+def _list_notifications(call: chitose.xrpc.XrpcCall, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, seen_at: typing.Optional[str]=None) -> bytes:
     """"""
     return call('app.bsky.notification.listNotifications', [('limit', limit), ('cursor', cursor), ('seenAt', seen_at)], None, {})
 
 class Notification(chitose.Object):
     """
```

### Comparing `chitose-0.0.7/chitose/app/bsky/richtext/facet.py` & `chitose-0.0.8/chitose/app/bsky/richtext/facet.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.7/chitose/com/atproto/admin/__init__.py` & `chitose-0.0.8/chitose/com/atproto/admin/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,73 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
-from chitose.xrpc import XrpcCallable
+from chitose.xrpc import XrpcCall
+from chitose.xrpc import XrpcSubscribe
 from .disable_account_invites import _disable_account_invites
 from .disable_invite_codes import _disable_invite_codes
 from .enable_account_invites import _enable_account_invites
 from .get_invite_codes import _get_invite_codes
 from .get_moderation_action import _get_moderation_action
 from .get_moderation_actions import _get_moderation_actions
 from .get_moderation_report import _get_moderation_report
 from .get_moderation_reports import _get_moderation_reports
 from .get_record import _get_record
 from .get_repo import _get_repo
+from .rebase_repo import _rebase_repo
 from .resolve_moderation_reports import _resolve_moderation_reports
 from .reverse_moderation_action import _reverse_moderation_action
 from .search_repos import _search_repos
 from .take_moderation_action import _take_moderation_action
 from .update_account_email import _update_account_email
 from .update_account_handle import _update_account_handle
 import chitose.com.atproto.admin.defs
 import chitose.com.atproto.repo.strong_ref
 import typing
 
 class Admin_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
-    def __init__(self, call: XrpcCallable) -> None:
+    def __init__(self, call: XrpcCall, subscribe: XrpcSubscribe) -> None:
         self.call = call
+        self.subscribe = subscribe
 
     def get_repo(self, did: str) -> bytes:
         """View details about a repository."""
         return _get_repo(self.call, did)
 
-    def get_moderation_reports(self, subject: typing.Optional[str]=None, resolved: typing.Optional[bool]=None, action_type: typing.Optional[typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge', 'com.atproto.admin.defs#escalate']]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
-        """List moderation reports related to a subject."""
-        return _get_moderation_reports(self.call, subject, resolved, action_type, limit, cursor)
+    def get_moderation_reports(self, subject: typing.Optional[str]=None, ignore_subjects: typing.Optional[list[str]]=None, resolved: typing.Optional[bool]=None, action_type: typing.Optional[typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge', 'com.atproto.admin.defs#escalate']]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, reverse: typing.Optional[bool]=None) -> bytes:
+        """List moderation reports related to a subject.
+
+
+        :param reverse: Reverse the order of the returned records? when true, returns reports in chronological order
+        """
+        return _get_moderation_reports(self.call, subject, ignore_subjects, resolved, action_type, limit, cursor, reverse)
 
     def take_moderation_action(self, action: typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge'], subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: str, created_by: str, subject_blob_cids: typing.Optional[list[str]]=None, create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None) -> bytes:
         """Take a moderation action on a repo."""
         return _take_moderation_action(self.call, action, subject, reason, created_by, subject_blob_cids, create_label_vals, negate_label_vals)
 
     def update_account_email(self, account: str, email: str) -> bytes:
         """Administrative action to update an account's email
 
 
         :param account: The handle or DID of the repo.
         """
         return _update_account_email(self.call, account, email)
 
+    def rebase_repo(self, repo: str, swap_commit: typing.Optional[str]=None) -> bytes:
+        """Administrative action to rebase an account's repo
+
+
+        :param repo: The handle or DID of the repo.
+
+        :param swap_commit: Compare and swap with the previous commit by cid.
+        """
+        return _rebase_repo(self.call, repo, swap_commit)
+
     def get_moderation_action(self, id: int) -> bytes:
         """View details about a moderation action."""
         return _get_moderation_action(self.call, id)
 
     def update_account_handle(self, did: str, handle: str) -> bytes:
         """Administrative action to update an account's handle"""
         return _update_account_handle(self.call, did, handle)
```

### Comparing `chitose-0.0.7/chitose/com/atproto/admin/defs.py` & `chitose-0.0.8/chitose/com/atproto/admin/defs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.7/chitose/com/atproto/admin/get_moderation_reports.py` & `chitose-0.0.8/chitose/com/atproto/admin/get_moderation_reports.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _get_moderation_reports(call: chitose.xrpc.XrpcCallable, subject: typing.Optional[str]=None, resolved: typing.Optional[bool]=None, action_type: typing.Optional[typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge', 'com.atproto.admin.defs#escalate']]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
-    """List moderation reports related to a subject."""
-    return call('com.atproto.admin.getModerationReports', [('subject', subject), ('resolved', resolved), ('actionType', action_type), ('limit', limit), ('cursor', cursor)], None, {})
+def _get_moderation_reports(call: chitose.xrpc.XrpcCall, subject: typing.Optional[str]=None, ignore_subjects: typing.Optional[list[str]]=None, resolved: typing.Optional[bool]=None, action_type: typing.Optional[typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge', 'com.atproto.admin.defs#escalate']]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, reverse: typing.Optional[bool]=None) -> bytes:
+    """List moderation reports related to a subject.
+
+
+    :param reverse: Reverse the order of the returned records? when true, returns reports in chronological order
+    """
+    return call('com.atproto.admin.getModerationReports', [('subject', subject), ('ignoreSubjects', ignore_subjects), ('resolved', resolved), ('actionType', action_type), ('limit', limit), ('cursor', cursor), ('reverse', reverse)], None, {})
```

### Comparing `chitose-0.0.7/chitose/com/atproto/admin/take_moderation_action.py` & `chitose-0.0.8/chitose/com/atproto/admin/take_moderation_action.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,10 +2,10 @@
 """"""
 from __future__ import annotations
 import chitose
 import chitose.com.atproto.admin.defs
 import chitose.com.atproto.repo.strong_ref
 import typing
 
-def _take_moderation_action(call: chitose.xrpc.XrpcCallable, action: typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge'], subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: str, created_by: str, subject_blob_cids: typing.Optional[list[str]]=None, create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None) -> bytes:
+def _take_moderation_action(call: chitose.xrpc.XrpcCall, action: typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge'], subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: str, created_by: str, subject_blob_cids: typing.Optional[list[str]]=None, create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None) -> bytes:
     """Take a moderation action on a repo."""
     return call('com.atproto.admin.takeModerationAction', [], {'action': action, 'subject': subject, 'subjectBlobCids': subject_blob_cids, 'createLabelVals': create_label_vals, 'negateLabelVals': negate_label_vals, 'reason': reason, 'createdBy': created_by}, {'Content-Type': 'application/json'})
```

### Comparing `chitose-0.0.7/chitose/com/atproto/identity/__init__.py` & `chitose-0.0.8/chitose/com/atproto/identity/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
-from chitose.xrpc import XrpcCallable
+from chitose.xrpc import XrpcCall
+from chitose.xrpc import XrpcSubscribe
 from .resolve_handle import _resolve_handle
 from .update_handle import _update_handle
 
 class Identity_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
-    def __init__(self, call: XrpcCallable) -> None:
+    def __init__(self, call: XrpcCall, subscribe: XrpcSubscribe) -> None:
         self.call = call
+        self.subscribe = subscribe
 
     def update_handle(self, handle: str) -> bytes:
         """Updates the handle of the account"""
         return _update_handle(self.call, handle)
 
     def resolve_handle(self, handle: str) -> bytes:
         """Provides the DID of a repo.
```

### Comparing `chitose-0.0.7/chitose/com/atproto/label/__init__.py` & `chitose-0.0.8/chitose/com/atproto/label/query_labels.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
-from chitose.xrpc import XrpcCallable
-from .query_labels import _query_labels
+import chitose
 import typing
 
-class Label_:
-    """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
+def _query_labels(call: chitose.xrpc.XrpcCall, uri_patterns: list[str], sources: typing.Optional[list[str]]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
+    """Find labels relevant to the provided URI patterns.
 
-    def __init__(self, call: XrpcCallable) -> None:
-        self.call = call
 
-    def query_labels(self, uri_patterns: list[str], sources: typing.Optional[list[str]]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
-        """Find labels relevant to the provided URI patterns.
+    :param uri_patterns: List of AT URI patterns to match (boolean 'OR'). Each may be a prefix (ending with '*'; will match inclusive of the string leading to '*'), or a full URI
 
-
-        :param uri_patterns: List of AT URI patterns to match (boolean 'OR'). Each may be a prefix (ending with '*'; will match inclusive of the string leading to '*'), or a full URI
-
-        :param sources: Optional list of label sources (DIDs) to filter on
-        """
-        return _query_labels(self.call, uri_patterns, sources, limit, cursor)
+    :param sources: Optional list of label sources (DIDs) to filter on
+    """
+    return call('com.atproto.label.queryLabels', [('uriPatterns', uri_patterns), ('sources', sources), ('limit', limit), ('cursor', cursor)], None, {})
```

### Comparing `chitose-0.0.7/chitose/com/atproto/label/defs.py` & `chitose-0.0.8/chitose/com/atproto/label/defs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.7/chitose/com/atproto/moderation/__init__.py` & `chitose-0.0.8/chitose/com/atproto/moderation/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
-from chitose.xrpc import XrpcCallable
+from chitose.xrpc import XrpcCall
+from chitose.xrpc import XrpcSubscribe
 from .create_report import _create_report
 import chitose.com.atproto.admin.defs
 import chitose.com.atproto.moderation.defs
 import chitose.com.atproto.repo.strong_ref
 import typing
 
 class Moderation_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
-    def __init__(self, call: XrpcCallable) -> None:
+    def __init__(self, call: XrpcCall, subscribe: XrpcSubscribe) -> None:
         self.call = call
+        self.subscribe = subscribe
 
     def create_report(self, reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: typing.Optional[str]=None) -> bytes:
         """Report a repo or a record."""
         return _create_report(self.call, reason_type, subject, reason)
```

### Comparing `chitose-0.0.7/chitose/com/atproto/moderation/create_report.py` & `chitose-0.0.8/chitose/com/atproto/moderation/create_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,10 +3,10 @@
 from __future__ import annotations
 import chitose
 import chitose.com.atproto.admin.defs
 import chitose.com.atproto.moderation.defs
 import chitose.com.atproto.repo.strong_ref
 import typing
 
-def _create_report(call: chitose.xrpc.XrpcCallable, reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: typing.Optional[str]=None) -> bytes:
+def _create_report(call: chitose.xrpc.XrpcCall, reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: typing.Optional[str]=None) -> bytes:
     """Report a repo or a record."""
     return call('com.atproto.moderation.createReport', [], {'reasonType': reason_type, 'reason': reason, 'subject': subject}, {'Content-Type': 'application/json'})
```

### Comparing `chitose-0.0.7/chitose/com/atproto/moderation/defs.py` & `chitose-0.0.8/chitose/com/atproto/moderation/defs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.7/chitose/com/atproto/repo/__init__.py` & `chitose-0.0.8/chitose/com/atproto/repo/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
-from chitose.xrpc import XrpcCallable
+from chitose.xrpc import XrpcCall
+from chitose.xrpc import XrpcSubscribe
 from .apply_writes import _apply_writes
 from .create_record import _create_record
 from .delete_record import _delete_record
 from .describe_repo import _describe_repo
 from .get_record import _get_record
 from .list_records import _list_records
 from .put_record import _put_record
@@ -12,16 +13,17 @@
 from .upload_blob import _upload_blob
 import chitose.com.atproto.repo.apply_writes
 import typing
 
 class Repo_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
-    def __init__(self, call: XrpcCallable) -> None:
+    def __init__(self, call: XrpcCall, subscribe: XrpcSubscribe) -> None:
         self.call = call
+        self.subscribe = subscribe
 
     def create_record(self, repo: str, collection: str, record: typing.Any, rkey: typing.Optional[str]=None, validate: typing.Optional[bool]=None, swap_commit: typing.Optional[str]=None) -> bytes:
         """Create a new record.
 
 
         :param repo: The handle or DID of the repo.
```

### Comparing `chitose-0.0.7/chitose/com/atproto/repo/apply_writes.py` & `chitose-0.0.8/chitose/com/atproto/repo/apply_writes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import chitose.com.atproto.repo.apply_writes
 import typing
 
-def _apply_writes(call: chitose.xrpc.XrpcCallable, repo: str, writes: list[typing.Union[chitose.com.atproto.repo.apply_writes.Create, chitose.com.atproto.repo.apply_writes.Update, chitose.com.atproto.repo.apply_writes.Delete]], validate: typing.Optional[bool]=None, swap_commit: typing.Optional[str]=None) -> bytes:
+def _apply_writes(call: chitose.xrpc.XrpcCall, repo: str, writes: list[typing.Union[chitose.com.atproto.repo.apply_writes.Create, chitose.com.atproto.repo.apply_writes.Update, chitose.com.atproto.repo.apply_writes.Delete]], validate: typing.Optional[bool]=None, swap_commit: typing.Optional[str]=None) -> bytes:
     """Apply a batch transaction of creates, updates, and deletes.
 
 
     :param repo: The handle or DID of the repo.
 
     :param validate: Validate the records?
     """
```

### Comparing `chitose-0.0.7/chitose/com/atproto/repo/create_record.py` & `chitose-0.0.8/chitose/com/atproto/repo/create_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _create_record(call: chitose.xrpc.XrpcCallable, repo: str, collection: str, record: typing.Any, rkey: typing.Optional[str]=None, validate: typing.Optional[bool]=None, swap_commit: typing.Optional[str]=None) -> bytes:
+def _create_record(call: chitose.xrpc.XrpcCall, repo: str, collection: str, record: typing.Any, rkey: typing.Optional[str]=None, validate: typing.Optional[bool]=None, swap_commit: typing.Optional[str]=None) -> bytes:
     """Create a new record.
 
 
     :param repo: The handle or DID of the repo.
 
     :param collection: The NSID of the record collection.
```

### Comparing `chitose-0.0.7/chitose/com/atproto/repo/delete_record.py` & `chitose-0.0.8/chitose/com/atproto/repo/delete_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _delete_record(call: chitose.xrpc.XrpcCallable, repo: str, collection: str, rkey: str, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
+def _delete_record(call: chitose.xrpc.XrpcCall, repo: str, collection: str, rkey: str, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
     """Delete a record, or ensure it doesn't exist.
 
 
     :param repo: The handle or DID of the repo.
 
     :param collection: The NSID of the record collection.
```

### Comparing `chitose-0.0.7/chitose/com/atproto/repo/get_record.py` & `chitose-0.0.8/chitose/com/atproto/repo/get_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _get_record(call: chitose.xrpc.XrpcCallable, repo: str, collection: str, rkey: str, cid: typing.Optional[str]=None) -> bytes:
+def _get_record(call: chitose.xrpc.XrpcCall, repo: str, collection: str, rkey: str, cid: typing.Optional[str]=None) -> bytes:
     """Get a record.
 
 
     :param repo: The handle or DID of the repo.
 
     :param collection: The NSID of the record collection.
```

### Comparing `chitose-0.0.7/chitose/com/atproto/repo/list_records.py` & `chitose-0.0.8/chitose/com/atproto/repo/list_records.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _list_records(call: chitose.xrpc.XrpcCallable, repo: str, collection: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, rkey_start: typing.Optional[str]=None, rkey_end: typing.Optional[str]=None, reverse: typing.Optional[bool]=None) -> bytes:
+def _list_records(call: chitose.xrpc.XrpcCall, repo: str, collection: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, rkey_start: typing.Optional[str]=None, rkey_end: typing.Optional[str]=None, reverse: typing.Optional[bool]=None) -> bytes:
     """List a range of records in a collection.
 
 
     :param repo: The handle or DID of the repo.
 
     :param collection: The NSID of the record type.
```

### Comparing `chitose-0.0.7/chitose/com/atproto/repo/put_record.py` & `chitose-0.0.8/chitose/com/atproto/repo/put_record.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _put_record(call: chitose.xrpc.XrpcCallable, repo: str, collection: str, rkey: str, record: typing.Any, validate: typing.Optional[bool]=None, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
+def _put_record(call: chitose.xrpc.XrpcCall, repo: str, collection: str, rkey: str, record: typing.Any, validate: typing.Optional[bool]=None, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
     """Write a record, creating or updating it as needed.
 
 
     :param repo: The handle or DID of the repo.
 
     :param collection: The NSID of the record collection.
```

### Comparing `chitose-0.0.7/chitose/com/atproto/repo/rebase_repo.py` & `chitose-0.0.8/chitose/com/atproto/repo/rebase_repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _rebase_repo(call: chitose.xrpc.XrpcCallable, repo: str, swap_commit: typing.Optional[str]=None) -> bytes:
+def _rebase_repo(call: chitose.xrpc.XrpcCall, repo: str, swap_commit: typing.Optional[str]=None) -> bytes:
     """Simple rebase of repo that deletes history
 
 
     :param repo: The handle or DID of the repo.
 
     :param swap_commit: Compare and swap with the previous commit by cid.
     """
```

### Comparing `chitose-0.0.7/chitose/com/atproto/server/__init__.py` & `chitose-0.0.8/chitose/com/atproto/server/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
-from chitose.xrpc import XrpcCallable
+from chitose.xrpc import XrpcCall
+from chitose.xrpc import XrpcSubscribe
 from .create_account import _create_account
 from .create_app_password import _create_app_password
 from .create_invite_code import _create_invite_code
 from .create_invite_codes import _create_invite_codes
 from .create_session import _create_session
 from .delete_account import _delete_account
 from .delete_session import _delete_session
@@ -18,16 +19,17 @@
 from .reset_password import _reset_password
 from .revoke_app_password import _revoke_app_password
 import typing
 
 class Server_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
-    def __init__(self, call: XrpcCallable) -> None:
+    def __init__(self, call: XrpcCall, subscribe: XrpcSubscribe) -> None:
         self.call = call
+        self.subscribe = subscribe
 
     def get_account_invite_codes(self, include_used: typing.Optional[bool]=None, create_available: typing.Optional[bool]=None) -> bytes:
         """Get all invite codes for a given account"""
         return _get_account_invite_codes(self.call, include_used, create_available)
 
     def create_session(self, identifier: str, password: str) -> bytes:
         """Create an authentication session.
```

### Comparing `chitose-0.0.7/chitose/com/atproto/server/create_account.py` & `chitose-0.0.8/chitose/com/atproto/server/create_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _create_account(call: chitose.xrpc.XrpcCallable, email: str, handle: str, password: str, did: typing.Optional[str]=None, invite_code: typing.Optional[str]=None, recovery_key: typing.Optional[str]=None) -> bytes:
+def _create_account(call: chitose.xrpc.XrpcCall, email: str, handle: str, password: str, did: typing.Optional[str]=None, invite_code: typing.Optional[str]=None, recovery_key: typing.Optional[str]=None) -> bytes:
     """Create an account."""
     return call('com.atproto.server.createAccount', [], {'email': email, 'handle': handle, 'did': did, 'inviteCode': invite_code, 'password': password, 'recoveryKey': recovery_key}, {'Content-Type': 'application/json'})
```

### Comparing `chitose-0.0.7/chitose/com/atproto/server/create_app_password.py` & `chitose-0.0.8/chitose/com/atproto/server/create_app_password.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 
-def _create_app_password(call: chitose.xrpc.XrpcCallable, name: str) -> bytes:
+def _create_app_password(call: chitose.xrpc.XrpcCall, name: str) -> bytes:
     """Create an app-specific password."""
     return call('com.atproto.server.createAppPassword', [], {'name': name}, {'Content-Type': 'application/json'})
 
 class AppPassword(chitose.Object):
     """"""
 
     def __init__(self, name: str, password: str, created_at: str) -> None:
```

### Comparing `chitose-0.0.7/chitose/com/atproto/server/create_invite_codes.py` & `chitose-0.0.8/chitose/com/atproto/server/create_invite_codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _create_invite_codes(call: chitose.xrpc.XrpcCallable, code_count: int, use_count: int, for_accounts: typing.Optional[list[str]]=None) -> bytes:
+def _create_invite_codes(call: chitose.xrpc.XrpcCall, code_count: int, use_count: int, for_accounts: typing.Optional[list[str]]=None) -> bytes:
     """Create an invite code."""
     return call('com.atproto.server.createInviteCodes', [], {'codeCount': code_count, 'useCount': use_count, 'forAccounts': for_accounts}, {'Content-Type': 'application/json'})
 
 class AccountCodes(chitose.Object):
     """"""
 
     def __init__(self, account: str, codes: list[str]) -> None:
```

### Comparing `chitose-0.0.7/chitose/com/atproto/server/defs.py` & `chitose-0.0.8/chitose/com/atproto/server/defs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.7/chitose/com/atproto/server/describe_server.py` & `chitose-0.0.8/chitose/com/atproto/server/describe_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _describe_server(call: chitose.xrpc.XrpcCallable) -> bytes:
+def _describe_server(call: chitose.xrpc.XrpcCall) -> bytes:
     """Get a document describing the service's accounts configuration."""
     return call('com.atproto.server.describeServer', [], None, {})
 
 class Links(chitose.Object):
     """"""
 
     def __init__(self, privacy_policy: typing.Optional[str]=None, terms_of_service: typing.Optional[str]=None) -> None:
```

### Comparing `chitose-0.0.7/chitose/com/atproto/server/list_app_passwords.py` & `chitose-0.0.8/chitose/com/atproto/server/list_app_passwords.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 
-def _list_app_passwords(call: chitose.xrpc.XrpcCallable) -> bytes:
+def _list_app_passwords(call: chitose.xrpc.XrpcCall) -> bytes:
     """List all app-specific passwords."""
     return call('com.atproto.server.listAppPasswords', [], None, {})
 
 class AppPassword(chitose.Object):
     """"""
 
     def __init__(self, name: str, created_at: str) -> None:
```

### Comparing `chitose-0.0.7/chitose/com/atproto/sync/__init__.py` & `chitose-0.0.8/chitose/com/atproto/sync/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
-from chitose.xrpc import XrpcCallable
+from chitose.xrpc import XrpcCall
+from chitose.xrpc import XrpcSubscribe
 from .get_blob import _get_blob
 from .get_blocks import _get_blocks
 from .get_checkout import _get_checkout
 from .get_commit_path import _get_commit_path
 from .get_head import _get_head
 from .get_record import _get_record
 from .get_repo import _get_repo
 from .list_blobs import _list_blobs
 from .list_repos import _list_repos
 from .notify_of_update import _notify_of_update
 from .request_crawl import _request_crawl
+from .subscribe_repos import _subscribe_repos
+import chitose
 import typing
 
 class Sync_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
-    def __init__(self, call: XrpcCallable) -> None:
+    def __init__(self, call: XrpcCall, subscribe: XrpcSubscribe) -> None:
         self.call = call
+        self.subscribe = subscribe
 
     def get_head(self, did: str) -> bytes:
         """Gets the current HEAD CID of a repo.
 
 
         :param did: The DID of the repo.
         """
@@ -74,14 +78,22 @@
 
         :param latest: The most recent commit
 
         :param earliest: The earliest commit to start from
         """
         return _list_blobs(self.call, did, latest, earliest)
 
+    def subscribe_repos(self, handler: chitose.xrpc.XrpcHandler, cursor: typing.Optional[int]=None) -> None:
+        """Subscribe to repo updates
+
+
+        :param cursor: The last known event to backfill from.
+        """
+        _subscribe_repos(self.subscribe, handler, cursor)
+
     def get_record(self, did: str, collection: str, rkey: str, commit: typing.Optional[str]=None) -> bytes:
         """Gets blocks needed for existence or non-existence of record.
 
 
         :param did: The DID of the repo.
 
         :param commit: An optional past commit CID.
```

### Comparing `chitose-0.0.7/chitose/com/atproto/sync/get_commit_path.py` & `chitose-0.0.8/chitose/com/atproto/sync/get_commit_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _get_commit_path(call: chitose.xrpc.XrpcCallable, did: str, latest: typing.Optional[str]=None, earliest: typing.Optional[str]=None) -> bytes:
+def _get_commit_path(call: chitose.xrpc.XrpcCall, did: str, latest: typing.Optional[str]=None, earliest: typing.Optional[str]=None) -> bytes:
     """Gets the path of repo commits
 
 
     :param did: The DID of the repo.
 
     :param latest: The most recent commit
```

### Comparing `chitose-0.0.7/chitose/com/atproto/sync/get_record.py` & `chitose-0.0.8/chitose/com/atproto/admin/rebase_repo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _get_record(call: chitose.xrpc.XrpcCallable, did: str, collection: str, rkey: str, commit: typing.Optional[str]=None) -> bytes:
-    """Gets blocks needed for existence or non-existence of record.
+def _rebase_repo(call: chitose.xrpc.XrpcCall, repo: str, swap_commit: typing.Optional[str]=None) -> bytes:
+    """Administrative action to rebase an account's repo
 
 
-    :param did: The DID of the repo.
+    :param repo: The handle or DID of the repo.
 
-    :param commit: An optional past commit CID.
+    :param swap_commit: Compare and swap with the previous commit by cid.
     """
-    return call('com.atproto.sync.getRecord', [('did', did), ('collection', collection), ('rkey', rkey), ('commit', commit)], None, {})
+    return call('com.atproto.admin.rebaseRepo', [], {'repo': repo, 'swapCommit': swap_commit}, {'Content-Type': 'application/json'})
```

### Comparing `chitose-0.0.7/chitose/com/atproto/sync/get_repo.py` & `chitose-0.0.8/chitose/com/atproto/sync/get_repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _get_repo(call: chitose.xrpc.XrpcCallable, did: str, earliest: typing.Optional[str]=None, latest: typing.Optional[str]=None) -> bytes:
+def _get_repo(call: chitose.xrpc.XrpcCall, did: str, earliest: typing.Optional[str]=None, latest: typing.Optional[str]=None) -> bytes:
     """Gets the repo state.
 
 
     :param did: The DID of the repo.
 
     :param earliest: The earliest commit in the commit range (not inclusive)
```

### Comparing `chitose-0.0.7/chitose/com/atproto/sync/list_blobs.py` & `chitose-0.0.8/chitose/com/atproto/sync/list_blobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _list_blobs(call: chitose.xrpc.XrpcCallable, did: str, latest: typing.Optional[str]=None, earliest: typing.Optional[str]=None) -> bytes:
+def _list_blobs(call: chitose.xrpc.XrpcCall, did: str, latest: typing.Optional[str]=None, earliest: typing.Optional[str]=None) -> bytes:
     """List blob cids for some range of commits
 
 
     :param did: The DID of the repo.
 
     :param latest: The most recent commit
```

### Comparing `chitose-0.0.7/chitose/com/atproto/sync/list_repos.py` & `chitose-0.0.8/chitose/com/atproto/sync/list_repos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _list_repos(call: chitose.xrpc.XrpcCallable, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
+def _list_repos(call: chitose.xrpc.XrpcCall, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
     """List dids and root cids of hosted repos"""
     return call('com.atproto.sync.listRepos', [('limit', limit), ('cursor', cursor)], None, {})
 
 class Repo(chitose.Object):
     """"""
 
     def __init__(self, did: str, head: str) -> None:
```

### Comparing `chitose-0.0.7/chitose/com/atproto/sync/subscribe_repos.py` & `chitose-0.0.8/chitose/com/atproto/sync/subscribe_repos.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import chitose.com.atproto.sync.subscribe_repos
 import typing
 
+def _subscribe_repos(subscribe: chitose.xrpc.XrpcSubscribe, handler: chitose.xrpc.XrpcHandler, cursor: typing.Optional[int]=None) -> None:
+    """Subscribe to repo updates
+
+
+    :param cursor: The last known event to backfill from.
+    """
+    subscribe('com.atproto.sync.subscribeRepos', [('cursor', cursor)], handler)
+
 class Commit(chitose.Object):
     """
 
 
     :param blocks: CAR file containing relevant blocks
     """
```

### Comparing `chitose-0.0.7/chitose/xrpc.py` & `chitose-0.0.8/chitose/xrpc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from typing import Callable
 from typing import Optional
 from typing import Union
 import json
 import urllib.parse
 import urllib.request
 
+from websockets.sync.client import connect
+
 XrpcParams = list[tuple[str, Union[str,
                                    Optional[str], Optional[int], list[str]]]]
 XrpcData = Union[bytes, Optional[dict]]
 XrpcHeaders = dict[str, str]
-XrpcCallable = Callable[[str, XrpcParams, XrpcData, XrpcHeaders], bytes]
+XrpcCall = Callable[[str, XrpcParams, XrpcData, XrpcHeaders], bytes]
 
+XrpcHandler = Callable[[Union[str, bytes]], None]
+XrpcSubscribe = Callable[[str, XrpcParams, XrpcHandler], None]
 
-def call(method: str, params: XrpcParams,
-         d: XrpcData, service: str, headers: XrpcHeaders) -> bytes:
+
+def _url(method: str, params: XrpcParams, service: str) -> str:
     url = f'{service}/xrpc/{method}'
 
     query: list[tuple[str, Union[str, int]]] = []
     for key, val in params:
         if val is None:
             continue
 
@@ -26,15 +30,22 @@
             continue
 
         query.append((key, val))
 
     if query:
         url = f'{url}?{urllib.parse.urlencode(query)}'
 
+    return url
+
+
+def call(method: str, params: XrpcParams,
+         d: XrpcData, service: str, headers: XrpcHeaders) -> bytes:
+    url = _url(method, params, service)
     req = urllib.request.Request(url)
+
     for key, val in headers.items():
         req.add_header(key, val)
 
     if d:
         # for com.atproto.repo.uploadBlob
         if isinstance(d, bytes):
             data = d
@@ -44,15 +55,24 @@
                 if val is not None
             }
             data = json.dumps(d, default=lambda obj: {
                               key: val for key, val in obj.to_dict().items()
                               if val is not None
                               }).encode()
     elif d is None:
+        # for GET requests
         # d = None => data = None
         data = None
     else:
+        # for POST requests
         # d = {} => data = b''
         data = b''
 
     r = urllib.request.urlopen(req, data)
     return r.read()
+
+
+def subscribe(method: str, params: XrpcParams, service: str,
+              handler: XrpcHandler) -> None:
+    with connect(_url(method, params, service)) as websocket:
+        for message in websocket:
+            handler(message)
```

### Comparing `chitose-0.0.7/pyproject.toml` & `chitose-0.0.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chitose"
-version = "0.0.7"
+version = "0.0.8"
 description = "A client library for the AT Protocol (Bluesky) "
 license = "MIT"
 authors = [
     "Muneyuki Noguchi <nogu.dev@gmail.com>",
 ]
 readme = "README.md"
 homepage = "https://github.com/mnogu/chitose"
@@ -16,14 +16,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Documentation :: Sphinx",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
+websockets = ">=11.0"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/mnogu/chitose/issues"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `chitose-0.0.7/PKG-INFO` & `chitose-0.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: chitose
-Version: 0.0.7
+Version: 0.0.8
 Summary: A client library for the AT Protocol (Bluesky) 
 Home-page: https://github.com/mnogu/chitose
 License: MIT
 Author: Muneyuki Noguchi
 Author-email: nogu.dev@gmail.com
 Requires-Python: >=3.9
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation :: Sphinx
+Requires-Dist: websockets (>=11.0)
 Project-URL: Documentation, https://chitose.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/mnogu/chitose
 Description-Content-Type: text/markdown
 
 # Chitose
 
 [![Python](https://img.shields.io/pypi/pyversions/chitose.svg)](https://badge.fury.io/py/chitose)
@@ -32,27 +33,29 @@
 The API of Chitose is similar to [the ATP API](https://github.com/bluesky-social/atproto/blob/main/packages/api/README.md).
 
 For example, you can use `get_timeline()` in `BskyAgent` to get the timeline as shown below. Replace `YOUR_USERNAME` and `YOUR_PASSWORD` with your username and your password respectively:
 
 ```
 $ git clone https://github.com/mnogu/chitose.git
 $ cd chitose
+$ python3 -m pip install -r requirements.txt
 $ python3
 >>> from chitose import BskyAgent
 >>> agent = BskyAgent(service='https://bsky.social')
 >>> agent.login(identifier='YOUR_USERNAME', password='YOUR_PASSWORD')
 >>> agent.get_timeline(limit=1)
 ```
 For available methods in `BskyAgent`, refer to [the documentation of `BskyAgent`](https://chitose.readthedocs.io/en/latest/chitose.html#chitose.BskyAgent).
 
 Alternatively, you can use `app.bsky.feed.get_timeline()` as in [the advanced API calls](https://github.com/bluesky-social/atproto/blob/main/packages/api/README.md#advanced-api-calls):
 
 ```
 $ git clone https://github.com/mnogu/chitose.git
 $ cd chitose
+$ python3 -m pip install -r requirements.txt
 $ python3
 >>> from chitose import BskyAgent
 >>> agent = BskyAgent(service='https://bsky.social')
 >>> agent.login(identifier='YOUR_USERNAME', password='YOUR_PASSWORD')
 >>> agent.app.bsky.feed.get_timeline(limit=1)
 ```
 
@@ -85,14 +88,15 @@
 $ python3 -m pip install chitose
 ```
 
 Alternatively, you can build a Python package and install it:
 ```
 $ git clone https://github.com/mnogu/chitose.git
 $ cd chitose
+$ python3 -m pip install -r requirements.txt
 $ python3 -m pip install --upgrade build
 $ python3 -m build
 $ python3 -m pip install dist/chitose-*-py3-none-any.whl
 ```
 
 ## Generating Code
 
@@ -111,11 +115,11 @@
 
 You may want to add new Python code to the repository or update the documentation:
 ```
 $ git add chitose
 $ git commit
 ```
 ```
-$ python3 -m pip install sphinx
+$ python3 -m pip install -r docs/source/requirements.txt
 $ cd docs
 $ sphinx-apidoc -o ./source ../chitose -f
 ```
```

