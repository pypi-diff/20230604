# Comparing `tmp/pubmed_types-0.1.1.tar.gz` & `tmp/pubmed_types-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pubmed_types-0.1.1.tar", max compression
+gzip compressed data, was "pubmed_types-0.1.2.tar", max compression
```

## Comparing `pubmed_types-0.1.1.tar` & `pubmed_types-0.1.2.tar`

### file list

```diff
@@ -1,673 +1,673 @@
--rw-r--r--   0        0        0     1072 2023-05-25 16:03:32.757838 pubmed_types-0.1.1/LICENSE
--rw-r--r--   0        0        0     3934 2023-06-04 13:47:52.792647 pubmed_types-0.1.1/README.md
--rw-r--r--   0        0        0     1444 2023-06-04 13:48:30.592052 pubmed_types-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      483 2023-06-04 13:47:52.792647 pubmed_types-0.1.1/src/pubmed_types/__init__.py
--rw-r--r--   0        0        0    24766 2023-06-03 02:43:58.380623 pubmed_types-0.1.1/src/pubmed_types/models/__init__.py
--rw-r--r--   0        0        0     7420 2023-06-03 02:44:01.924575 pubmed_types-0.1.1/src/pubmed_types/models/abbrev_journal_title.py
--rw-r--r--   0        0        0      610 2023-06-03 02:44:02.860562 pubmed_types-0.1.1/src/pubmed_types/models/abstract_1.py
--rw-r--r--   0        0        0     1645 2023-06-03 02:44:02.572566 pubmed_types-0.1.1/src/pubmed_types/models/abstract_text.py
--rw-r--r--   0        0        0      229 2023-06-03 02:44:02.832563 pubmed_types-0.1.1/src/pubmed_types/models/abstract_text_nlm_category.py
--rw-r--r--   0        0        0  1064015 2023-06-03 02:44:01.912575 pubmed_types-0.1.1/src/pubmed_types/models/access_date.py
--rw-r--r--   0        0        0      342 2023-06-03 02:44:02.576566 pubmed_types-0.1.1/src/pubmed_types/models/accession_number_list.py
--rw-r--r--   0        0        0      962 2023-06-03 02:44:02.576566 pubmed_types-0.1.1/src/pubmed_types/models/affiliation.py
--rw-r--r--   0        0        0      588 2023-06-03 02:44:02.576566 pubmed_types-0.1.1/src/pubmed_types/models/affiliation_info.py
--rw-r--r--   0        0        0     1373 2023-06-03 02:44:01.924575 pubmed_types-0.1.1/src/pubmed_types/models/alt_text.py
--rw-r--r--   0        0        0     8831 2023-06-03 02:44:01.944575 pubmed_types-0.1.1/src/pubmed_types/models/app.py
--rw-r--r--   0        0        0     8786 2023-06-03 02:44:01.960574 pubmed_types-0.1.1/src/pubmed_types/models/app_group.py
--rw-r--r--   0        0        0      419 2023-06-03 02:18:03.813928 pubmed_types-0.1.1/src/pubmed_types/models/archive_copy_source.py
--rw-r--r--   0        0        0      108 2023-06-03 02:44:02.776564 pubmed_types-0.1.1/src/pubmed_types/models/array_orientation.py
--rw-r--r--   0        0        0     3079 2023-06-03 02:44:02.864562 pubmed_types-0.1.1/src/pubmed_types/models/article_1.py
--rw-r--r--   0        0        0     2649 2023-06-03 02:44:02.876562 pubmed_types-0.1.1/src/pubmed_types/models/article_2.py
--rw-r--r--   0        0        0     1202 2023-06-03 02:44:01.960574 pubmed_types-0.1.1/src/pubmed_types/models/article_categories.py
--rw-r--r--   0        0        0      878 2023-06-03 02:44:02.576566 pubmed_types-0.1.1/src/pubmed_types/models/article_date.py
--rw-r--r--   0        0        0      369 2023-06-03 02:44:02.824563 pubmed_types-0.1.1/src/pubmed_types/models/article_dtd_version.py
--rw-r--r--   0        0        0     1423 2023-06-03 02:44:01.964574 pubmed_types-0.1.1/src/pubmed_types/models/article_id.py
--rw-r--r--   0        0        0      511 2023-06-03 02:44:02.876562 pubmed_types-0.1.1/src/pubmed_types/models/article_id_1.py
--rw-r--r--   0        0        0      303 2023-06-03 02:44:02.848563 pubmed_types-0.1.1/src/pubmed_types/models/article_id_id_type.py
--rw-r--r--   0        0        0      368 2023-06-03 02:44:02.580566 pubmed_types-0.1.1/src/pubmed_types/models/article_id_list.py
--rw-r--r--   0        0        0     9515 2023-06-03 02:44:01.980574 pubmed_types-0.1.1/src/pubmed_types/models/article_meta.py
--rw-r--r--   0        0        0      242 2023-06-03 02:44:02.828563 pubmed_types-0.1.1/src/pubmed_types/models/article_pub_model.py
--rw-r--r--   0        0        0      353 2023-06-03 02:18:03.769929 pubmed_types-0.1.1/src/pubmed_types/models/article_set.py
--rw-r--r--   0        0        0     1495 2023-06-03 02:44:02.880562 pubmed_types-0.1.1/src/pubmed_types/models/article_title_1.py
--rw-r--r--   0        0        0     3823 2023-06-03 02:44:01.988574 pubmed_types-0.1.1/src/pubmed_types/models/article_version.py
--rw-r--r--   0        0        0      827 2023-06-03 02:44:01.992574 pubmed_types-0.1.1/src/pubmed_types/models/article_version_alternatives.py
--rw-r--r--   0        0        0     1938 2023-06-03 02:44:02.580566 pubmed_types-0.1.1/src/pubmed_types/models/author.py
--rw-r--r--   0        0        0       80 2023-06-03 02:44:02.836563 pubmed_types-0.1.1/src/pubmed_types/models/author_equal_contrib.py
--rw-r--r--   0        0        0      838 2023-06-03 02:44:02.584566 pubmed_types-0.1.1/src/pubmed_types/models/author_list.py
--rw-r--r--   0        0        0       82 2023-06-03 02:44:02.832563 pubmed_types-0.1.1/src/pubmed_types/models/author_list_complete_yn.py
--rw-r--r--   0        0        0      100 2023-06-03 02:44:02.832563 pubmed_types-0.1.1/src/pubmed_types/models/author_list_type.py
--rw-r--r--   0        0        0     1720 2023-06-03 02:44:02.000574 pubmed_types-0.1.1/src/pubmed_types/models/author_notes.py
--rw-r--r--   0        0        0       75 2023-06-03 02:44:02.836563 pubmed_types-0.1.1/src/pubmed_types/models/author_valid_yn.py
--rw-r--r--   0        0        0     2449 2023-06-03 02:44:02.004574 pubmed_types-0.1.1/src/pubmed_types/models/award_desc.py
--rw-r--r--   0        0        0     4315 2023-06-03 02:44:02.012574 pubmed_types-0.1.1/src/pubmed_types/models/award_group.py
--rw-r--r--   0        0        0     2442 2023-06-03 02:44:02.016574 pubmed_types-0.1.1/src/pubmed_types/models/award_name.py
--rw-r--r--   0        0        0     2079 2023-06-03 02:44:02.020574 pubmed_types-0.1.1/src/pubmed_types/models/back.py
--rw-r--r--   0        0        0      765 2023-06-03 02:44:02.584566 pubmed_types-0.1.1/src/pubmed_types/models/beginning_date.py
--rw-r--r--   0        0        0     7356 2023-06-03 02:44:02.032574 pubmed_types-0.1.1/src/pubmed_types/models/body.py
--rw-r--r--   0        0        0       78 2023-06-03 02:44:02.768564 pubmed_types-0.1.1/src/pubmed_types/models/bold_toggle.py
--rw-r--r--   0        0        0     3125 2023-06-03 02:44:02.588566 pubmed_types-0.1.1/src/pubmed_types/models/book.py
--rw-r--r--   0        0        0     4185 2023-06-03 02:44:02.560566 pubmed_types-0.1.1/src/pubmed_types/models/book_document.py
--rw-r--r--   0        0        0      587 2023-06-03 02:44:02.556566 pubmed_types-0.1.1/src/pubmed_types/models/book_document_set.py
--rw-r--r--   0        0        0     1444 2023-06-03 02:44:02.592566 pubmed_types-0.1.1/src/pubmed_types/models/book_title.py
--rw-r--r--   0        0        0      112 2023-06-03 02:44:02.784563 pubmed_types-0.1.1/src/pubmed_types/models/boxed_text_orientation.py
--rw-r--r--   0        0        0      149 2023-06-03 02:44:02.788563 pubmed_types-0.1.1/src/pubmed_types/models/boxed_text_position.py
--rw-r--r--   0        0        0      529 2023-06-03 02:44:02.032574 pubmed_types-0.1.1/src/pubmed_types/models/break_mod.py
--rw-r--r--   0        0        0      117 2023-06-03 02:44:02.788563 pubmed_types-0.1.1/src/pubmed_types/models/chem_struct_wrap_orientation.py
--rw-r--r--   0        0        0      154 2023-06-03 02:44:02.788563 pubmed_types-0.1.1/src/pubmed_types/models/chem_struct_wrap_position.py
--rw-r--r--   0        0        0      592 2023-06-03 02:44:02.592566 pubmed_types-0.1.1/src/pubmed_types/models/chemical.py
--rw-r--r--   0        0        0      356 2023-06-03 02:44:02.592566 pubmed_types-0.1.1/src/pubmed_types/models/chemical_list.py
--rw-r--r--   0        0        0     1065 2023-06-03 02:44:02.592566 pubmed_types-0.1.1/src/pubmed_types/models/citation.py
--rw-r--r--   0        0        0     1344 2023-06-03 02:44:02.036574 pubmed_types-0.1.1/src/pubmed_types/models/city.py
--rw-r--r--   0        0        0       82 2023-06-03 02:44:02.788563 pubmed_types-0.1.1/src/pubmed_types/models/code_executable.py
--rw-r--r--   0        0        0      107 2023-06-03 02:44:02.788563 pubmed_types-0.1.1/src/pubmed_types/models/code_orientation.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.788563 pubmed_types-0.1.1/src/pubmed_types/models/code_position.py
--rw-r--r--   0        0        0      963 2023-06-03 02:44:02.596566 pubmed_types-0.1.1/src/pubmed_types/models/coi_statement.py
--rw-r--r--   0        0        0     1574 2023-06-03 02:44:02.036574 pubmed_types-0.1.1/src/pubmed_types/models/col.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.804563 pubmed_types-0.1.1/src/pubmed_types/models/col_align.py
--rw-r--r--   0        0        0      133 2023-06-03 02:44:02.804563 pubmed_types-0.1.1/src/pubmed_types/models/col_valign.py
--rw-r--r--   0        0        0     1765 2023-06-03 02:44:02.040573 pubmed_types-0.1.1/src/pubmed_types/models/colgroup.py
--rw-r--r--   0        0        0      153 2023-06-03 02:44:02.808563 pubmed_types-0.1.1/src/pubmed_types/models/colgroup_align.py
--rw-r--r--   0        0        0      138 2023-06-03 02:44:02.808563 pubmed_types-0.1.1/src/pubmed_types/models/colgroup_valign.py
--rw-r--r--   0        0        0     1450 2023-06-03 02:44:02.596566 pubmed_types-0.1.1/src/pubmed_types/models/collection_title.py
--rw-r--r--   0        0        0      965 2023-06-03 02:44:02.600566 pubmed_types-0.1.1/src/pubmed_types/models/collective_name.py
--rw-r--r--   0        0        0      934 2023-06-03 02:44:02.600566 pubmed_types-0.1.1/src/pubmed_types/models/comments_corrections.py
--rw-r--r--   0        0        0      424 2023-06-03 02:44:02.600566 pubmed_types-0.1.1/src/pubmed_types/models/comments_corrections_list.py
--rw-r--r--   0        0        0     1025 2023-06-03 02:44:02.840563 pubmed_types-0.1.1/src/pubmed_types/models/comments_corrections_ref_type.py
--rw-r--r--   0        0        0     7391 2023-06-03 02:44:02.052573 pubmed_types-0.1.1/src/pubmed_types/models/conf_num.py
--rw-r--r--   0        0        0     7394 2023-06-03 02:44:02.064573 pubmed_types-0.1.1/src/pubmed_types/models/conf_theme.py
--rw-r--r--   0        0        0     4292 2023-06-03 02:44:02.068573 pubmed_types-0.1.1/src/pubmed_types/models/conference.py
--rw-r--r--   0        0        0       82 2023-06-03 02:44:02.780563 pubmed_types-0.1.1/src/pubmed_types/models/contrib_corresp.py
--rw-r--r--   0        0        0       83 2023-06-03 02:44:02.784563 pubmed_types-0.1.1/src/pubmed_types/models/contrib_deceased.py
--rw-r--r--   0        0        0       87 2023-06-03 02:44:02.784563 pubmed_types-0.1.1/src/pubmed_types/models/contrib_equal_contrib.py
--rw-r--r--   0        0        0     1940 2023-06-03 02:44:02.072573 pubmed_types-0.1.1/src/pubmed_types/models/contrib_id.py
--rw-r--r--   0        0        0       98 2023-06-03 02:44:02.784563 pubmed_types-0.1.1/src/pubmed_types/models/contrib_id_authenticated.py
--rw-r--r--   0        0        0     1889 2023-06-03 02:44:02.076573 pubmed_types-0.1.1/src/pubmed_types/models/contributed_resource_group.py
--rw-r--r--   0        0        0      768 2023-06-03 02:44:02.600566 pubmed_types-0.1.1/src/pubmed_types/models/contribution_date.py
--rw-r--r--   0        0        0     1083 2023-06-03 02:44:02.080573 pubmed_types-0.1.1/src/pubmed_types/models/copyright_year.py
--rw-r--r--   0        0        0     8856 2023-06-03 02:44:02.092573 pubmed_types-0.1.1/src/pubmed_types/models/corresp.py
--rw-r--r--   0        0        0      871 2023-06-03 02:44:02.096573 pubmed_types-0.1.1/src/pubmed_types/models/count.py
--rw-r--r--   0        0        0     1907 2023-06-03 02:44:02.100573 pubmed_types-0.1.1/src/pubmed_types/models/counts.py
--rw-r--r--   0        0        0     3702 2023-06-03 02:44:02.104573 pubmed_types-0.1.1/src/pubmed_types/models/custom_meta.py
--rw-r--r--   0        0        0     1389 2023-06-03 02:44:02.108573 pubmed_types-0.1.1/src/pubmed_types/models/custom_meta_group.py
--rw-r--r--   0        0        0      579 2023-06-03 02:44:02.604566 pubmed_types-0.1.1/src/pubmed_types/models/data_bank.py
--rw-r--r--   0        0        0      644 2023-06-03 02:44:02.604566 pubmed_types-0.1.1/src/pubmed_types/models/data_bank_list.py
--rw-r--r--   0        0        0       84 2023-06-03 02:44:02.836563 pubmed_types-0.1.1/src/pubmed_types/models/data_bank_list_complete_yn.py
--rw-r--r--   0        0        0      672 2023-06-03 02:44:02.604566 pubmed_types-0.1.1/src/pubmed_types/models/date_completed.py
--rw-r--r--   0        0        0      670 2023-06-03 02:44:02.604566 pubmed_types-0.1.1/src/pubmed_types/models/date_revised.py
--rw-r--r--   0        0        0     1328 2023-06-03 02:44:02.108573 pubmed_types-0.1.1/src/pubmed_types/models/day.py
--rw-r--r--   0        0        0      338 2023-06-03 02:44:02.564566 pubmed_types-0.1.1/src/pubmed_types/models/delete_citation.py
--rw-r--r--   0        0        0      309 2023-06-03 02:44:02.564566 pubmed_types-0.1.1/src/pubmed_types/models/delete_document.py
--rw-r--r--   0        0        0      948 2023-06-03 02:44:02.608566 pubmed_types-0.1.1/src/pubmed_types/models/descriptor_name.py
--rw-r--r--   0        0        0       88 2023-06-03 02:44:02.840563 pubmed_types-0.1.1/src/pubmed_types/models/descriptor_name_major_topic_yn.py
--rw-r--r--   0        0        0       86 2023-06-03 02:44:02.840563 pubmed_types-0.1.1/src/pubmed_types/models/descriptor_name_type.py
--rw-r--r--   0        0        0      331 2023-06-03 02:44:02.884562 pubmed_types-0.1.1/src/pubmed_types/models/disp_formula_1.py
--rw-r--r--   0        0        0     1217 2023-06-03 02:44:02.112573 pubmed_types-0.1.1/src/pubmed_types/models/elocation_id.py
--rw-r--r--   0        0        0      809 2023-06-03 02:44:02.884562 pubmed_types-0.1.1/src/pubmed_types/models/elocation_id_1.py
--rw-r--r--   0        0        0       88 2023-06-03 02:44:02.832563 pubmed_types-0.1.1/src/pubmed_types/models/elocation_id_eid_type.py
--rw-r--r--   0        0        0       80 2023-06-03 02:44:02.832563 pubmed_types-0.1.1/src/pubmed_types/models/elocation_id_valid_yn.py
--rw-r--r--   0        0        0      762 2023-06-03 02:44:02.608566 pubmed_types-0.1.1/src/pubmed_types/models/ending_date.py
--rw-r--r--   0        0        0      704 2023-06-03 02:44:02.116572 pubmed_types-0.1.1/src/pubmed_types/models/equation_count.py
--rw-r--r--   0        0        0     1328 2023-06-03 02:44:02.116572 pubmed_types-0.1.1/src/pubmed_types/models/era.py
--rw-r--r--   0        0        0     3816 2023-06-03 02:44:02.124572 pubmed_types-0.1.1/src/pubmed_types/models/event.py
--rw-r--r--   0        0        0     3116 2023-06-03 02:44:02.132572 pubmed_types-0.1.1/src/pubmed_types/models/event_desc.py
--rw-r--r--   0        0        0     3131 2023-06-03 02:44:02.136572 pubmed_types-0.1.1/src/pubmed_types/models/extended_by.py
--rw-r--r--   0        0        0      692 2023-06-03 02:44:02.140572 pubmed_types-0.1.1/src/pubmed_types/models/fig_count.py
--rw-r--r--   0        0        0      111 2023-06-03 02:44:02.796563 pubmed_types-0.1.1/src/pubmed_types/models/fig_group_orientation.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.796563 pubmed_types-0.1.1/src/pubmed_types/models/fig_group_position.py
--rw-r--r--   0        0        0      106 2023-06-03 02:44:02.792563 pubmed_types-0.1.1/src/pubmed_types/models/fig_orientation.py
--rw-r--r--   0        0        0      143 2023-06-03 02:44:02.792563 pubmed_types-0.1.1/src/pubmed_types/models/fig_position.py
--rw-r--r--   0        0        0      467 2023-06-03 02:18:03.781929 pubmed_types-0.1.1/src/pubmed_types/models/first_name.py
--rw-r--r--   0        0        0       78 2023-06-03 02:18:04.049925 pubmed_types-0.1.1/src/pubmed_types/models/first_name_empty_yn.py
--rw-r--r--   0        0        0      458 2023-06-03 02:18:03.777929 pubmed_types-0.1.1/src/pubmed_types/models/first_page.py
--rw-r--r--   0        0        0      112 2023-06-03 02:18:04.045925 pubmed_types-0.1.1/src/pubmed_types/models/first_page_lzero.py
--rw-r--r--   0        0        0     2865 2023-06-03 02:44:02.144572 pubmed_types-0.1.1/src/pubmed_types/models/floats_group.py
--rw-r--r--   0        0        0     1461 2023-06-03 02:44:02.148572 pubmed_types-0.1.1/src/pubmed_types/models/fpage.py
--rw-r--r--   0        0        0     2105 2023-06-03 02:44:02.156572 pubmed_types-0.1.1/src/pubmed_types/models/front.py
--rw-r--r--   0        0        0     9514 2023-06-03 02:44:02.168572 pubmed_types-0.1.1/src/pubmed_types/models/front_stub.py
--rw-r--r--   0        0        0     1657 2023-06-03 02:44:02.168572 pubmed_types-0.1.1/src/pubmed_types/models/funding_group.py
--rw-r--r--   0        0        0     9232 2023-06-03 02:44:02.184572 pubmed_types-0.1.1/src/pubmed_types/models/funding_statement.py
--rw-r--r--   0        0        0      327 2023-06-03 02:44:02.608566 pubmed_types-0.1.1/src/pubmed_types/models/gene_symbol_list.py
--rw-r--r--   0        0        0      465 2023-06-03 02:44:02.612566 pubmed_types-0.1.1/src/pubmed_types/models/general_note.py
--rw-r--r--   0        0        0      152 2023-06-03 02:44:02.844563 pubmed_types-0.1.1/src/pubmed_types/models/general_note_owner.py
--rw-r--r--   0        0        0     1866 2023-06-03 02:44:02.184572 pubmed_types-0.1.1/src/pubmed_types/models/glyph_data.py
--rw-r--r--   0        0        0      728 2023-06-03 02:44:02.188572 pubmed_types-0.1.1/src/pubmed_types/models/glyph_ref.py
--rw-r--r--   0        0        0      806 2023-06-03 02:44:02.612566 pubmed_types-0.1.1/src/pubmed_types/models/grant.py
--rw-r--r--   0        0        0      611 2023-06-03 02:44:02.612566 pubmed_types-0.1.1/src/pubmed_types/models/grant_list.py
--rw-r--r--   0        0        0       81 2023-06-03 02:44:02.836563 pubmed_types-0.1.1/src/pubmed_types/models/grant_list_complete_yn.py
--rw-r--r--   0        0        0      110 2023-06-03 02:44:02.792563 pubmed_types-0.1.1/src/pubmed_types/models/graphic_orientation.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.792563 pubmed_types-0.1.1/src/pubmed_types/models/graphic_position.py
--rw-r--r--   0        0        0      551 2023-06-03 02:18:03.805928 pubmed_types-0.1.1/src/pubmed_types/models/group.py
--rw-r--r--   0        0        0      338 2023-06-03 02:18:03.805928 pubmed_types-0.1.1/src/pubmed_types/models/group_list.py
--rw-r--r--   0        0        0      425 2023-06-03 02:44:02.888562 pubmed_types-0.1.1/src/pubmed_types/models/history_1.py
--rw-r--r--   0        0        0     7177 2023-06-03 02:44:02.908562 pubmed_types-0.1.1/src/pubmed_types/models/history_2.py
--rw-r--r--   0        0        0      528 2023-06-03 02:44:02.192571 pubmed_types-0.1.1/src/pubmed_types/models/hr.py
--rw-r--r--   0        0        0     3870 2023-06-03 02:18:03.805928 pubmed_types-0.1.1/src/pubmed_types/models/i.py
--rw-r--r--   0        0        0      426 2023-06-03 02:44:02.616566 pubmed_types-0.1.1/src/pubmed_types/models/identifier.py
--rw-r--r--   0        0        0      718 2023-06-03 02:44:02.192571 pubmed_types-0.1.1/src/pubmed_types/models/index_term_range_end.py
--rw-r--r--   0        0        0     1475 2023-06-03 02:18:03.809928 pubmed_types-0.1.1/src/pubmed_types/models/individual_name.py
--rw-r--r--   0        0        0     2029 2023-06-03 02:44:02.200571 pubmed_types-0.1.1/src/pubmed_types/models/institution_id.py
--rw-r--r--   0        0        0     1537 2023-06-03 02:44:02.616566 pubmed_types-0.1.1/src/pubmed_types/models/investigator.py
--rw-r--r--   0        0        0      380 2023-06-03 02:44:02.616566 pubmed_types-0.1.1/src/pubmed_types/models/investigator_list.py
--rw-r--r--   0        0        0       81 2023-06-03 02:44:02.844563 pubmed_types-0.1.1/src/pubmed_types/models/investigator_valid_yn.py
--rw-r--r--   0        0        0      515 2023-06-03 02:44:02.908562 pubmed_types-0.1.1/src/pubmed_types/models/issn_1.py
--rw-r--r--   0        0        0      100 2023-06-03 02:44:02.828563 pubmed_types-0.1.1/src/pubmed_types/models/issn_issn_type.py
--rw-r--r--   0        0        0     3124 2023-06-03 02:44:02.204571 pubmed_types-0.1.1/src/pubmed_types/models/issue_id.py
--rw-r--r--   0        0        0     7395 2023-06-03 02:44:02.216571 pubmed_types-0.1.1/src/pubmed_types/models/issue_sponsor.py
--rw-r--r--   0        0        0     7400 2023-06-03 02:44:02.228571 pubmed_types-0.1.1/src/pubmed_types/models/issue_subtitle.py
--rw-r--r--   0        0        0     1874 2023-06-03 02:44:02.228571 pubmed_types-0.1.1/src/pubmed_types/models/issue_title_group.py
--rw-r--r--   0        0        0       80 2023-06-03 02:44:02.768564 pubmed_types-0.1.1/src/pubmed_types/models/italic_toggle.py
--rw-r--r--   0        0        0      508 2023-06-03 02:44:02.620566 pubmed_types-0.1.1/src/pubmed_types/models/item_list.py
--rw-r--r--   0        0        0      873 2023-06-03 02:44:02.620566 pubmed_types-0.1.1/src/pubmed_types/models/journal.py
--rw-r--r--   0        0        0     1543 2023-06-03 02:44:02.232571 pubmed_types-0.1.1/src/pubmed_types/models/journal_id.py
--rw-r--r--   0        0        0      942 2023-06-03 02:44:02.620566 pubmed_types-0.1.1/src/pubmed_types/models/journal_issue.py
--rw-r--r--   0        0        0      107 2023-06-03 02:44:02.832563 pubmed_types-0.1.1/src/pubmed_types/models/journal_issue_cited_medium.py
--rw-r--r--   0        0        0     2752 2023-06-03 02:44:02.236571 pubmed_types-0.1.1/src/pubmed_types/models/journal_meta.py
--rw-r--r--   0        0        0     7406 2023-06-03 02:44:02.252570 pubmed_types-0.1.1/src/pubmed_types/models/journal_subtitle.py
--rw-r--r--   0        0        0     7404 2023-06-03 02:44:02.264570 pubmed_types-0.1.1/src/pubmed_types/models/journal_title.py
--rw-r--r--   0        0        0     1683 2023-06-03 02:44:02.268570 pubmed_types-0.1.1/src/pubmed_types/models/journal_title_group.py
--rw-r--r--   0        0        0     1342 2023-06-03 02:44:02.624565 pubmed_types-0.1.1/src/pubmed_types/models/keyword.py
--rw-r--r--   0        0        0      601 2023-06-03 02:44:02.624565 pubmed_types-0.1.1/src/pubmed_types/models/keyword_list.py
--rw-r--r--   0        0        0      184 2023-06-03 02:44:02.844563 pubmed_types-0.1.1/src/pubmed_types/models/keyword_list_owner.py
--rw-r--r--   0        0        0       81 2023-06-03 02:44:02.844563 pubmed_types-0.1.1/src/pubmed_types/models/keyword_major_topic_yn.py
--rw-r--r--   0        0        0      460 2023-06-03 02:44:02.624565 pubmed_types-0.1.1/src/pubmed_types/models/location_label.py
--rw-r--r--   0        0        0      205 2023-06-03 02:44:02.852563 pubmed_types-0.1.1/src/pubmed_types/models/location_label_type.py
--rw-r--r--   0        0        0     1338 2023-06-03 02:44:02.272570 pubmed_types-0.1.1/src/pubmed_types/models/lpage.py
--rw-r--r--   0        0        0      108 2023-06-03 02:44:02.792563 pubmed_types-0.1.1/src/pubmed_types/models/media_orientation.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.796563 pubmed_types-0.1.1/src/pubmed_types/models/media_position.py
--rw-r--r--   0        0        0     5578 2023-06-03 02:44:02.568566 pubmed_types-0.1.1/src/pubmed_types/models/medline_citation.py
--rw-r--r--   0        0        0      178 2023-06-03 02:44:02.828563 pubmed_types-0.1.1/src/pubmed_types/models/medline_citation_owner.py
--rw-r--r--   0        0        0      284 2023-06-03 02:44:02.828563 pubmed_types-0.1.1/src/pubmed_types/models/medline_citation_status.py
--rw-r--r--   0        0        0      813 2023-06-03 02:44:02.624565 pubmed_types-0.1.1/src/pubmed_types/models/medline_journal_info.py
--rw-r--r--   0        0        0      618 2023-06-03 02:44:02.628565 pubmed_types-0.1.1/src/pubmed_types/models/mesh_heading.py
--rw-r--r--   0        0        0      376 2023-06-03 02:44:02.628565 pubmed_types-0.1.1/src/pubmed_types/models/mesh_heading_list.py
--rw-r--r--   0        0        0     6803 2023-06-03 02:44:02.284570 pubmed_types-0.1.1/src/pubmed_types/models/meta_name.py
--rw-r--r--   0        0        0     6806 2023-06-03 02:44:02.296570 pubmed_types-0.1.1/src/pubmed_types/models/meta_value.py
--rw-r--r--   0        0        0     1408 2023-06-03 02:44:02.300570 pubmed_types-0.1.1/src/pubmed_types/models/milestone_end.py
--rw-r--r--   0        0        0     1414 2023-06-03 02:44:02.304570 pubmed_types-0.1.1/src/pubmed_types/models/milestone_start.py
--rw-r--r--   0        0        0       83 2023-06-03 02:44:02.772564 pubmed_types-0.1.1/src/pubmed_types/models/monospace_toggle.py
--rw-r--r--   0        0        0     1334 2023-06-03 02:44:02.304570 pubmed_types-0.1.1/src/pubmed_types/models/month.py
--rw-r--r--   0        0        0      153 2023-06-03 02:44:02.784563 pubmed_types-0.1.1/src/pubmed_types/models/name_name_style.py
--rw-r--r--   0        0        0      423 2023-06-03 02:44:02.628565 pubmed_types-0.1.1/src/pubmed_types/models/name_of_substance.py
--rw-r--r--   0        0        0     1422 2023-06-03 02:44:02.308570 pubmed_types-0.1.1/src/pubmed_types/models/object_id.py
--rw-r--r--   0        0        0      354 2023-06-03 02:44:02.632565 pubmed_types-0.1.1/src/pubmed_types/models/object_list.py
--rw-r--r--   0        0        0      497 2023-06-03 02:44:02.632565 pubmed_types-0.1.1/src/pubmed_types/models/object_mod.py
--rw-r--r--   0        0        0       81 2023-06-03 02:44:02.820563 pubmed_types-0.1.1/src/pubmed_types/models/option_correct.py
--rw-r--r--   0        0        0       15 2023-06-03 02:17:59.961981 pubmed_types-0.1.1/src/pubmed_types/models/org/__init__.py
--rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.1/src/pubmed_types/models/org/niso/__init__.py
--rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.1/src/pubmed_types/models/org/niso/schemas/__init__.py
--rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.1/src/pubmed_types/models/org/niso/schemas/ali/__init__.py
--rw-r--r--   0        0        0      124 2023-06-03 02:43:58.380623 pubmed_types-0.1.1/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/__init__.py
--rw-r--r--   0        0        0      631 2023-06-03 02:44:02.552566 pubmed_types-0.1.1/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/free_to_read.py
--rw-r--r--   0        0        0      578 2023-06-03 02:44:02.552566 pubmed_types-0.1.1/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/license_ref.py
--rw-r--r--   0        0        0       15 2023-06-03 02:17:59.961981 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/__init__.py
--rw-r--r--   0        0        0       15 2023-06-03 02:17:59.989981 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/__init__.py
--rw-r--r--   0        0        0       15 2023-06-03 02:17:59.989981 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/__init__.py
--rw-r--r--   0        0        0    18558 2023-06-03 02:43:58.344624 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/__init__.py
--rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.116600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/abs.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.132599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/and_mod.py
--rw-r--r--   0        0        0     2149 2023-06-03 02:44:00.364596 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/annotation.py
--rw-r--r--   0        0        0     1582 2023-06-03 02:44:00.148599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/approx.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.184599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccos.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.184599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccosh.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.184599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccot.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.188599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccoth.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.188599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccsc.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.188599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccsch.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.188599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arcsec.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.188599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arcsech.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.180599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arcsin.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.192599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arcsinh.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.184599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arctan.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.192599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arctanh.py
--rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.120600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arg.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.164599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/card.py
--rw-r--r--   0        0        0      466 2023-06-03 02:44:00.160599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cartesianproduct.py
--rw-r--r--   0        0        0     1737 2023-06-03 02:44:00.092600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cbytes.py
--rw-r--r--   0        0        0     1584 2023-06-03 02:44:00.128600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ceiling.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.096600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/codomain.py
--rw-r--r--   0        0        0      168 2023-06-03 02:44:00.224598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/columnalignstyle.py
--rw-r--r--   0        0        0      452 2023-06-03 02:44:00.208598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/complexes.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.104600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/compose.py
--rw-r--r--   0        0        0  1555308 2023-06-03 02:44:00.088600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/condition.py
--rw-r--r--   0        0        0     1588 2023-06-03 02:44:00.120600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/conjugate.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cos.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.176599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cosh.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.176599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cot.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.180599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/coth.py
--rw-r--r--   0        0        0     1767 2023-06-03 02:44:00.092600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cs.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/csc.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.180599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/csch.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.156599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/curl.py
--rw-r--r--   0        0        0      189 2023-06-03 02:44:02.664565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/declare_occurrence.py
--rw-r--r--   0        0        0      456 2023-06-03 02:44:00.196599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/determinant.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.152599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/diff.py
--rw-r--r--   0        0        0      454 2023-06-03 02:44:00.156599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/divergence.py
--rw-r--r--   0        0        0     1582 2023-06-03 02:44:00.108600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/divide.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.096600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/domain.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.208598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/emptyset.py
--rw-r--r--   0        0        0      438 2023-06-03 02:44:00.140599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/eq.py
--rw-r--r--   0        0        0      454 2023-06-03 02:44:00.140599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/equivalent.py
--rw-r--r--   0        0        0      454 2023-06-03 02:44:00.216598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/eulergamma.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.140599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/exists.py
--rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.128600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/exp.py
--rw-r--r--   0        0        0      458 2023-06-03 02:44:00.208598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/exponentiale.py
--rw-r--r--   0        0        0     1588 2023-06-03 02:44:00.116600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/factorial.py
--rw-r--r--   0        0        0     1586 2023-06-03 02:44:00.148599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/factorof.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.212598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/false.py
--rw-r--r--   0        0        0     1580 2023-06-03 02:44:00.124600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/floor.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.140599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/forall.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.132599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/gcd.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.144599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/geq.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.156599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/grad.py
--rw-r--r--   0        0        0      438 2023-06-03 02:44:00.140599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/gt.py
--rw-r--r--   0        0        0      444 2023-06-03 02:44:00.096600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ident.py
--rw-r--r--   0        0        0      444 2023-06-03 02:44:00.100600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/image.py
--rw-r--r--   0        0        0     1588 2023-06-03 02:44:00.124600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/imaginary.py
--rw-r--r--   0        0        0      454 2023-06-03 02:44:00.212598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/imaginaryi.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.136599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/implies.py
--rw-r--r--   0        0        0      438 2023-06-03 02:44:00.160599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/in_mod.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.216598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/infinity.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.152599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/int_mod.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.204599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/integers.py
--rw-r--r--   0        0        0      452 2023-06-03 02:44:00.160599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/intersect.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.096600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/interval.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.096600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/inverse.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.100600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/lambda_mod.py
--rw-r--r--   0        0        0      452 2023-06-03 02:44:00.156599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/laplacian.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.132599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/lcm.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.144599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/leq.py
--rw-r--r--   0        0        0      444 2023-06-03 02:44:00.168599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/limit.py
--rw-r--r--   0        0        0      161 2023-06-03 02:44:00.224598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/linestyle.py
--rw-r--r--   0        0        0      161 2023-06-03 02:44:02.664565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/list_order.py
--rw-r--r--   0        0        0      438 2023-06-03 02:44:00.100600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ln.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.100600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/log.py
--rw-r--r--   0        0        0      438 2023-06-03 02:44:00.140599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/lt.py
--rw-r--r--   0        0        0      136 2023-06-03 02:44:02.664565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maction_value.py
--rw-r--r--   0        0        0     2637 2023-06-03 02:44:00.268597 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maligngroup.py
--rw-r--r--   0        0        0      207 2023-06-03 02:44:02.708564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maligngroup_groupalign.py
--rw-r--r--   0        0        0      140 2023-06-03 02:44:02.708564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maligngroup_value.py
--rw-r--r--   0        0        0     2605 2023-06-03 02:44:00.264598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/malignmark.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.708564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/malignmark_edge.py
--rw-r--r--   0        0        0      139 2023-06-03 02:44:02.708564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/malignmark_value.py
--rw-r--r--   0        0        0    74524 2023-06-03 02:44:00.364596 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math.py
--rw-r--r--   0        0        0      140 2023-06-03 02:44:02.744564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_accent.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.744564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_accentunder.py
--rw-r--r--   0        0        0      161 2023-06-03 02:44:02.744564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_align.py
--rw-r--r--   0        0        0      142 2023-06-03 02:44:02.744564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_bevelled.py
--rw-r--r--   0        0        0      165 2023-06-03 02:44:02.744564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_charalign.py
--rw-r--r--   0        0        0      166 2023-06-03 02:44:02.744564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_denomalign.py
--rw-r--r--   0        0        0      131 2023-06-03 02:44:02.748564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_dir.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.768564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_display.py
--rw-r--r--   0        0        0      146 2023-06-03 02:44:02.744564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_displaystyle.py
--rw-r--r--   0        0        0      138 2023-06-03 02:44:02.748564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_edge.py
--rw-r--r--   0        0        0      146 2023-06-03 02:44:02.748564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_equalcolumns.py
--rw-r--r--   0        0        0      143 2023-06-03 02:44:02.748564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_equalrows.py
--rw-r--r--   0        0        0      139 2023-06-03 02:44:02.748564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_fence.py
--rw-r--r--   0        0        0      166 2023-06-03 02:44:02.748564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_form.py
--rw-r--r--   0        0        0      199 2023-06-03 02:44:02.752564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_indentalign.py
--rw-r--r--   0        0        0      236 2023-06-03 02:44:02.752564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_indentalignfirst.py
--rw-r--r--   0        0        0      235 2023-06-03 02:44:02.752564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_indentalignlast.py
--rw-r--r--   0        0        0      185 2023-06-03 02:44:02.744564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_infixlinebreakstyle.py
--rw-r--r--   0        0        0      141 2023-06-03 02:44:02.752564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_largeop.py
--rw-r--r--   0        0        0      225 2023-06-03 02:44:02.752564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_linebreak.py
--rw-r--r--   0        0        0      228 2023-06-03 02:44:02.756564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_linebreakstyle.py
--rw-r--r--   0        0        0      208 2023-06-03 02:44:02.756564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_location.py
--rw-r--r--   0        0        0      495 2023-06-03 02:44:02.756564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_longdivstyle.py
--rw-r--r--   0        0        0      641 2023-06-03 02:44:02.760564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_mathvariant.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.760564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_movablelimits.py
--rw-r--r--   0        0        0      164 2023-06-03 02:44:02.760564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_numalign.py
--rw-r--r--   0        0        0      220 2023-06-03 02:44:02.768564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_overflow.py
--rw-r--r--   0        0        0      143 2023-06-03 02:44:02.760564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_separator.py
--rw-r--r--   0        0        0      204 2023-06-03 02:44:02.760564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_side.py
--rw-r--r--   0        0        0      200 2023-06-03 02:44:02.764564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_stackalign.py
--rw-r--r--   0        0        0      142 2023-06-03 02:44:02.764564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_stretchy.py
--rw-r--r--   0        0        0      143 2023-06-03 02:44:02.764564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_symmetric.py
--rw-r--r--   0        0        0      117 2023-06-03 02:44:02.740564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_value.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.196599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/matrix.py
--rw-r--r--   0        0        0      452 2023-06-03 02:44:00.196599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/matrixrow.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.128600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/max.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.192599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mean.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.192599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/median.py
--rw-r--r--   0        0        0      137 2023-06-03 02:44:02.680565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/menclose_value.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.680565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/merror_value.py
--rw-r--r--   0        0        0      136 2023-06-03 02:44:02.680565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfenced_value.py
--rw-r--r--   0        0        0      143 2023-06-03 02:44:02.704564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfrac_bevelled.py
--rw-r--r--   0        0        0      167 2023-06-03 02:44:02.704564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfrac_denomalign.py
--rw-r--r--   0        0        0      165 2023-06-03 02:44:02.704564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfrac_numalign.py
--rw-r--r--   0        0        0      120 2023-06-03 02:44:02.704564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfrac_value.py
--rw-r--r--   0        0        0     5862 2023-06-03 02:44:00.256598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph.py
--rw-r--r--   0        0        0      151 2023-06-03 02:44:02.660565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_fontstyle.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.660565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_fontweight.py
--rw-r--r--   0        0        0      643 2023-06-03 02:44:02.660565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_mathvariant.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.660565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_value.py
--rw-r--r--   0        0        0     5329 2023-06-03 02:44:00.228598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi.py
--rw-r--r--   0        0        0      129 2023-06-03 02:44:02.732564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_dir.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.736564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_fontstyle.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.732564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_fontweight.py
--rw-r--r--   0        0        0      639 2023-06-03 02:44:02.732564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_mathvariant.py
--rw-r--r--   0        0        0      131 2023-06-03 02:44:02.732564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_value.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.132599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/min.py
--rw-r--r--   0        0        0     1580 2023-06-03 02:44:00.108600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/minus.py
--rw-r--r--   0        0        0     3231 2023-06-03 02:44:00.276597 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlabeledtr.py
--rw-r--r--   0        0        0      214 2023-06-03 02:44:02.736564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlabeledtr_rowalign.py
--rw-r--r--   0        0        0      139 2023-06-03 02:44:02.736564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlabeledtr_value.py
--rw-r--r--   0        0        0      499 2023-06-03 02:44:02.664565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlongdiv_longdivstyle.py
--rw-r--r--   0        0        0      137 2023-06-03 02:44:02.664565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlongdiv_value.py
--rw-r--r--   0        0        0      142 2023-06-03 02:44:02.672565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mmultiscripts_value.py
--rw-r--r--   0        0        0     5329 2023-06-03 02:44:00.232598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn.py
--rw-r--r--   0        0        0      129 2023-06-03 02:44:02.732564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_dir.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.732564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_fontstyle.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.732564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_fontweight.py
--rw-r--r--   0        0        0      639 2023-06-03 02:44:02.732564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_mathvariant.py
--rw-r--r--   0        0        0      131 2023-06-03 02:44:02.728564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_value.py
--rw-r--r--   0        0        0    10043 2023-06-03 02:44:00.240598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo.py
--rw-r--r--   0        0        0      138 2023-06-03 02:44:02.724564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_accent.py
--rw-r--r--   0        0        0      129 2023-06-03 02:44:02.720564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_dir.py
--rw-r--r--   0        0        0      137 2023-06-03 02:44:02.724564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_fence.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.720564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_fontstyle.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.720564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_fontweight.py
--rw-r--r--   0        0        0      164 2023-06-03 02:44:02.724564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_form.py
--rw-r--r--   0        0        0      197 2023-06-03 02:44:02.728564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_indentalign.py
--rw-r--r--   0        0        0      234 2023-06-03 02:44:02.728564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_indentalignfirst.py
--rw-r--r--   0        0        0      233 2023-06-03 02:44:02.728564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_indentalignlast.py
--rw-r--r--   0        0        0      139 2023-06-03 02:44:02.724564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_largeop.py
--rw-r--r--   0        0        0      223 2023-06-03 02:44:02.728564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_linebreak.py
--rw-r--r--   0        0        0      226 2023-06-03 02:44:02.728564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_linebreakstyle.py
--rw-r--r--   0        0        0      639 2023-06-03 02:44:02.720564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_mathvariant.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.724564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_movablelimits.py
--rw-r--r--   0        0        0      141 2023-06-03 02:44:02.724564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_separator.py
--rw-r--r--   0        0        0      140 2023-06-03 02:44:02.724564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_stretchy.py
--rw-r--r--   0        0        0      141 2023-06-03 02:44:02.724564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_symmetric.py
--rw-r--r--   0        0        0      125 2023-06-03 02:44:02.720564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_value.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.196599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mode.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.100600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/moment.py
--rw-r--r--   0        0        0      141 2023-06-03 02:44:02.676565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mover_accent.py
--rw-r--r--   0        0        0      162 2023-06-03 02:44:02.676565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mover_align.py
--rw-r--r--   0        0        0      134 2023-06-03 02:44:02.676565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mover_value.py
--rw-r--r--   0        0        0      136 2023-06-03 02:44:02.680565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mpadded_value.py
--rw-r--r--   0        0        0      137 2023-06-03 02:44:02.680565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mphantom_value.py
--rw-r--r--   0        0        0     2432 2023-06-03 02:44:00.264598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mprescripts.py
--rw-r--r--   0        0        0      140 2023-06-03 02:44:02.736564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mprescripts_value.py
--rw-r--r--   0        0        0      134 2023-06-03 02:44:02.700564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mroot_value.py
--rw-r--r--   0        0        0      131 2023-06-03 02:44:02.708564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mrow_dir.py
--rw-r--r--   0        0        0      133 2023-06-03 02:44:02.704564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mrow_value.py
--rw-r--r--   0        0        0     5585 2023-06-03 02:44:00.252598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms.py
--rw-r--r--   0        0        0      129 2023-06-03 02:44:02.712564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_dir.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.712564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_fontstyle.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.712564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_fontweight.py
--rw-r--r--   0        0        0      639 2023-06-03 02:44:02.708564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_mathvariant.py
--rw-r--r--   0        0        0      131 2023-06-03 02:44:02.708564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_value.py
--rw-r--r--   0        0        0      213 2023-06-03 02:44:02.740564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mscarries_location.py
--rw-r--r--   0        0        0      292 2023-06-03 02:44:02.740564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mscarries_value.py
--rw-r--r--   0        0        0      211 2023-06-03 02:44:02.740564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mscarry_location.py
--rw-r--r--   0        0        0      290 2023-06-03 02:44:02.740564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mscarry_value.py
--rw-r--r--   0        0        0      136 2023-06-03 02:44:02.740564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msgroup_value.py
--rw-r--r--   0        0        0     3475 2023-06-03 02:44:00.260598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msline.py
--rw-r--r--   0        0        0      121 2023-06-03 02:44:02.740564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msline_value.py
--rw-r--r--   0        0        0     5838 2023-06-03 02:44:00.248598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace.py
--rw-r--r--   0        0        0      133 2023-06-03 02:44:02.712564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_dir.py
--rw-r--r--   0        0        0      151 2023-06-03 02:44:02.716564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_fontstyle.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.716564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_fontweight.py
--rw-r--r--   0        0        0      269 2023-06-03 02:44:02.716564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_linebreak.py
--rw-r--r--   0        0        0      643 2023-06-03 02:44:02.712564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_mathvariant.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.712564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_value.py
--rw-r--r--   0        0        0      134 2023-06-03 02:44:02.700564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msqrt_value.py
--rw-r--r--   0        0        0      134 2023-06-03 02:44:02.740564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msrow_value.py
--rw-r--r--   0        0        0      167 2023-06-03 02:44:02.664565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstack_charalign.py
--rw-r--r--   0        0        0      202 2023-06-03 02:44:02.664565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstack_stackalign.py
--rw-r--r--   0        0        0      123 2023-06-03 02:44:02.664565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstack_value.py
--rw-r--r--   0        0        0      142 2023-06-03 02:44:02.684565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_accent.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.684565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_accentunder.py
--rw-r--r--   0        0        0      163 2023-06-03 02:44:02.684565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_align.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.684565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_bevelled.py
--rw-r--r--   0        0        0      167 2023-06-03 02:44:02.684565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_charalign.py
--rw-r--r--   0        0        0      168 2023-06-03 02:44:02.684565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_denomalign.py
--rw-r--r--   0        0        0      133 2023-06-03 02:44:02.688565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_dir.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.680565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_displaystyle.py
--rw-r--r--   0        0        0      140 2023-06-03 02:44:02.688565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_edge.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.688565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_equalcolumns.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.688565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_equalrows.py
--rw-r--r--   0        0        0      141 2023-06-03 02:44:02.688565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_fence.py
--rw-r--r--   0        0        0      151 2023-06-03 02:44:02.700564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_fontstyle.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.700564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_fontweight.py
--rw-r--r--   0        0        0      168 2023-06-03 02:44:02.688565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_form.py
--rw-r--r--   0        0        0      201 2023-06-03 02:44:02.692565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_indentalign.py
--rw-r--r--   0        0        0      238 2023-06-03 02:44:02.692565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_indentalignfirst.py
--rw-r--r--   0        0        0      237 2023-06-03 02:44:02.692565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_indentalignlast.py
--rw-r--r--   0        0        0      187 2023-06-03 02:44:02.684565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_infixlinebreakstyle.py
--rw-r--r--   0        0        0      143 2023-06-03 02:44:02.692565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_largeop.py
--rw-r--r--   0        0        0      227 2023-06-03 02:44:02.692565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_linebreak.py
--rw-r--r--   0        0        0      230 2023-06-03 02:44:02.692565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_linebreakstyle.py
--rw-r--r--   0        0        0      210 2023-06-03 02:44:02.692565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_location.py
--rw-r--r--   0        0        0      497 2023-06-03 02:44:02.696565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_longdivstyle.py
--rw-r--r--   0        0        0      643 2023-06-03 02:44:02.696565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_mathvariant.py
--rw-r--r--   0        0        0      149 2023-06-03 02:44:02.696565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_movablelimits.py
--rw-r--r--   0        0        0      166 2023-06-03 02:44:02.696565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_numalign.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.696565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_separator.py
--rw-r--r--   0        0        0      206 2023-06-03 02:44:02.700564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_side.py
--rw-r--r--   0        0        0      202 2023-06-03 02:44:02.700564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_stackalign.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.700564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_stretchy.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.700564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_symmetric.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.680565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_value.py
--rw-r--r--   0        0        0      133 2023-06-03 02:44:02.680565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msub_value.py
--rw-r--r--   0        0        0      136 2023-06-03 02:44:02.676565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msubsup_value.py
--rw-r--r--   0        0        0      133 2023-06-03 02:44:02.676565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msup_value.py
--rw-r--r--   0        0        0     6510 2023-06-03 02:44:00.272597 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.668565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_displaystyle.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.668565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_equalcolumns.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.668565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_equalrows.py
--rw-r--r--   0        0        0      206 2023-06-03 02:44:02.668565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_side.py
--rw-r--r--   0        0        0      141 2023-06-03 02:44:02.668565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_value.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.280597 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtd.py
--rw-r--r--   0        0        0     5386 2023-06-03 02:44:00.244598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext.py
--rw-r--r--   0        0        0      132 2023-06-03 02:44:02.716564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_dir.py
--rw-r--r--   0        0        0      150 2023-06-03 02:44:02.716564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_fontstyle.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.716564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_fontweight.py
--rw-r--r--   0        0        0      642 2023-06-03 02:44:02.716564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_mathvariant.py
--rw-r--r--   0        0        0      134 2023-06-03 02:44:02.716564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_value.py
--rw-r--r--   0        0        0     3175 2023-06-03 02:44:00.280597 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtr.py
--rw-r--r--   0        0        0      207 2023-06-03 02:44:02.672565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtr_rowalign.py
--rw-r--r--   0        0        0      132 2023-06-03 02:44:02.668565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtr_value.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.676565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munder_accentunder.py
--rw-r--r--   0        0        0      163 2023-06-03 02:44:02.676565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munder_align.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.676565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munder_value.py
--rw-r--r--   0        0        0      146 2023-06-03 02:44:02.672565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munderover_accent.py
--rw-r--r--   0        0        0      151 2023-06-03 02:44:02.672565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munderover_accentunder.py
--rw-r--r--   0        0        0      167 2023-06-03 02:44:02.672565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munderover_align.py
--rw-r--r--   0        0        0      139 2023-06-03 02:44:02.672565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munderover_value.py
--rw-r--r--   0        0        0      462 2023-06-03 02:44:00.204599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/naturalnumbers.py
--rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.144599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/neq.py
--rw-r--r--   0        0        0     2401 2023-06-03 02:44:00.260598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/none.py
--rw-r--r--   0        0        0      133 2023-06-03 02:44:02.736564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/none_value.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.136599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/not_mod.py
--rw-r--r--   0        0        0      454 2023-06-03 02:44:00.212598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/notanumber.py
--rw-r--r--   0        0        0      444 2023-06-03 02:44:00.160599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/notin.py
--rw-r--r--   0        0        0      456 2023-06-03 02:44:00.164599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/notprsubset.py
--rw-r--r--   0        0        0      452 2023-06-03 02:44:00.164599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/notsubset.py
--rw-r--r--   0        0        0      438 2023-06-03 02:44:00.136599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/or_mod.py
--rw-r--r--   0        0        0      458 2023-06-03 02:44:00.204599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/outerproduct.py
--rw-r--r--   0        0        0      456 2023-06-03 02:44:00.156599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/partialdiff.py
--rw-r--r--   0        0        0      438 2023-06-03 02:44:00.216598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/pi.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.132599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/plus.py
--rw-r--r--   0        0        0     1580 2023-06-03 02:44:00.108600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/power.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.208598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/primes.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.168599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/product.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.164599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/prsubset.py
--rw-r--r--   0        0        0     1586 2023-06-03 02:44:00.104600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/quotient.py
--rw-r--r--   0        0        0      452 2023-06-03 02:44:00.204599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/rationals.py
--rw-r--r--   0        0        0     1578 2023-06-03 02:44:00.124600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/real.py
--rw-r--r--   0        0        0      444 2023-06-03 02:44:00.204599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/reals.py
--rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.112600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/rem.py
--rw-r--r--   0        0        0     1578 2023-06-03 02:44:00.112600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/root.py
--rw-r--r--   0        0        0      460 2023-06-03 02:44:00.200599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/scalarproduct.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.192599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sdev.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sec.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.180599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sech.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.200599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/selector.py
--rw-r--r--   0        0        0      215 2023-06-03 02:44:00.092600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sep.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.164599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/setdiff.py
--rw-r--r--   0        0        0     1405 2023-06-03 02:44:00.088600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/share.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sin.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.176599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sinh.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.164599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/subset.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.168599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sum.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/tan.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.176599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/tanh.py
--rw-r--r--   0        0        0     1710 2023-06-03 02:44:00.152599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/tendsto.py
--rw-r--r--   0        0        0      444 2023-06-03 02:44:00.132599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/times.py
--rw-r--r--   0        0        0      452 2023-06-03 02:44:00.200599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/transpose.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.212598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/true.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.160599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/union.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.192599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/variance.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.196599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/vector.py
--rw-r--r--   0        0        0      460 2023-06-03 02:44:00.200599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/vectorproduct.py
--rw-r--r--   0        0        0      209 2023-06-03 02:44:00.224598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/verticalalign.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.136599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/xor.py
--rw-r--r--   0        0        0       15 2023-06-03 02:17:59.961981 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/__init__.py
--rw-r--r--   0        0        0      488 2023-06-03 02:43:58.316624 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/__init__.py
--rw-r--r--   0        0        0      188 2023-06-03 02:44:02.660565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/actuate_value.py
--rw-r--r--   0        0        0     1893 2023-06-03 02:43:58.428623 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/arc_type.py
--rw-r--r--   0        0        0     1169 2023-06-03 02:43:58.420623 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/extended.py
--rw-r--r--   0        0        0     1453 2023-06-03 02:43:58.428623 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/locator_type.py
--rw-r--r--   0        0        0     1244 2023-06-03 02:43:58.424623 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/resource_type.py
--rw-r--r--   0        0        0      193 2023-06-03 02:44:02.660565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/show_value.py
--rw-r--r--   0        0        0     1940 2023-06-03 02:43:58.416623 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/simple.py
--rw-r--r--   0        0        0     1203 2023-06-03 02:43:58.424623 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/title_elt_type.py
--rw-r--r--   0        0        0      247 2023-06-03 02:44:02.660565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/type_value.py
--rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/xml/__init__.py
--rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/xml/pkg_1998/__init__.py
--rw-r--r--   0        0        0      120 2023-06-03 02:43:58.380623 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/xml/pkg_1998/namespace/__init__.py
--rw-r--r--   0        0        0      118 2023-06-03 02:44:02.656565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/xml/pkg_1998/namespace/lang_value.py
--rw-r--r--   0        0        0      154 2023-06-03 02:44:02.656565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/xml/pkg_1998/namespace/space_value.py
--rw-r--r--   0        0        0      997 2023-06-03 02:44:02.632565 pubmed_types-0.1.1/src/pubmed_types/models/other_abstract.py
--rw-r--r--   0        0        0      223 2023-06-03 02:44:02.844563 pubmed_types-0.1.1/src/pubmed_types/models/other_abstract_type.py
--rw-r--r--   0        0        0      518 2023-06-03 02:44:02.632565 pubmed_types-0.1.1/src/pubmed_types/models/other_id.py
--rw-r--r--   0        0        0      257 2023-06-03 02:44:02.840563 pubmed_types-0.1.1/src/pubmed_types/models/other_id_source.py
--rw-r--r--   0        0        0      863 2023-06-03 02:44:02.312570 pubmed_types-0.1.1/src/pubmed_types/models/overline_end.py
--rw-r--r--   0        0        0      747 2023-06-03 02:44:02.312570 pubmed_types-0.1.1/src/pubmed_types/models/overline_start.py
--rw-r--r--   0        0        0       82 2023-06-03 02:44:02.772564 pubmed_types-0.1.1/src/pubmed_types/models/overline_toggle.py
--rw-r--r--   0        0        0      692 2023-06-03 02:44:02.316570 pubmed_types-0.1.1/src/pubmed_types/models/page_count.py
--rw-r--r--   0        0        0     1349 2023-06-03 02:44:02.320570 pubmed_types-0.1.1/src/pubmed_types/models/page_range.py
--rw-r--r--   0        0        0      649 2023-06-03 02:44:02.636565 pubmed_types-0.1.1/src/pubmed_types/models/pagination.py
--rw-r--r--   0        0        0     1147 2023-06-03 02:44:02.636565 pubmed_types-0.1.1/src/pubmed_types/models/param.py
--rw-r--r--   0        0        0      831 2023-06-03 02:44:02.640565 pubmed_types-0.1.1/src/pubmed_types/models/personal_name_subject.py
--rw-r--r--   0        0        0      426 2023-06-03 02:44:02.640565 pubmed_types-0.1.1/src/pubmed_types/models/personal_name_subject_list.py
--rw-r--r--   0        0        0      461 2023-06-03 02:44:02.632565 pubmed_types-0.1.1/src/pubmed_types/models/pmid.py
--rw-r--r--   0        0        0     1366 2023-06-03 02:44:02.320570 pubmed_types-0.1.1/src/pubmed_types/models/postal_code.py
--rw-r--r--   0        0        0      112 2023-06-03 02:44:02.796563 pubmed_types-0.1.1/src/pubmed_types/models/preformat_orientation.py
--rw-r--r--   0        0        0      149 2023-06-03 02:44:02.796563 pubmed_types-0.1.1/src/pubmed_types/models/preformat_position.py
--rw-r--r--   0        0        0     2142 2023-06-03 02:44:02.324570 pubmed_types-0.1.1/src/pubmed_types/models/principal_award_recipient.py
--rw-r--r--   0        0        0     1855 2023-06-03 02:44:02.328570 pubmed_types-0.1.1/src/pubmed_types/models/principal_investigator.py
--rw-r--r--   0        0        0     2483 2023-06-03 02:44:02.332569 pubmed_types-0.1.1/src/pubmed_types/models/processing_meta.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.824563 pubmed_types-0.1.1/src/pubmed_types/models/processing_meta_base_tagset.py
--rw-r--r--   0        0        0      109 2023-06-03 02:44:02.824563 pubmed_types-0.1.1/src/pubmed_types/models/processing_meta_mathml_version.py
--rw-r--r--   0        0        0      138 2023-06-03 02:44:02.824563 pubmed_types-0.1.1/src/pubmed_types/models/processing_meta_table_model.py
--rw-r--r--   0        0        0      116 2023-06-03 02:44:02.828563 pubmed_types-0.1.1/src/pubmed_types/models/processing_meta_tagset_family.py
--rw-r--r--   0        0        0      936 2023-06-03 02:44:02.912562 pubmed_types-0.1.1/src/pubmed_types/models/pub_date_1.py
--rw-r--r--   0        0        0     2895 2023-06-03 02:44:02.916561 pubmed_types-0.1.1/src/pubmed_types/models/pub_date_2.py
--rw-r--r--   0        0        0      740 2023-06-03 02:44:02.332569 pubmed_types-0.1.1/src/pubmed_types/models/pub_date_not_available.py
--rw-r--r--   0        0        0      408 2023-06-03 02:18:04.041925 pubmed_types-0.1.1/src/pubmed_types/models/pub_date_pub_status.py
--rw-r--r--   0        0        0      708 2023-06-03 02:44:02.336569 pubmed_types-0.1.1/src/pubmed_types/models/pub_history.py
--rw-r--r--   0        0        0     2871 2023-06-03 02:44:02.340569 pubmed_types-0.1.1/src/pubmed_types/models/pub_id.py
--rw-r--r--   0        0        0     1462 2023-06-03 02:44:02.644565 pubmed_types-0.1.1/src/pubmed_types/models/pub_med_pub_date.py
--rw-r--r--   0        0        0      496 2023-06-03 02:44:02.848563 pubmed_types-0.1.1/src/pubmed_types/models/pub_med_pub_date_pub_status.py
--rw-r--r--   0        0        0      423 2023-06-03 02:44:02.640565 pubmed_types-0.1.1/src/pubmed_types/models/publication_type.py
--rw-r--r--   0        0        0      400 2023-06-03 02:44:02.640565 pubmed_types-0.1.1/src/pubmed_types/models/publication_type_list.py
--rw-r--r--   0        0        0     1192 2023-06-03 02:18:03.561932 pubmed_types-0.1.1/src/pubmed_types/models/publisher.py
--rw-r--r--   0        0        0      606 2023-06-03 02:44:02.920561 pubmed_types-0.1.1/src/pubmed_types/models/publisher_1.py
--rw-r--r--   0        0        0     1193 2023-06-03 02:44:02.920561 pubmed_types-0.1.1/src/pubmed_types/models/publisher_2.py
--rw-r--r--   0        0        0     1013 2023-06-03 02:44:02.924561 pubmed_types-0.1.1/src/pubmed_types/models/publisher_name_1.py
--rw-r--r--   0        0        0      600 2023-06-03 02:44:02.556566 pubmed_types-0.1.1/src/pubmed_types/models/pubmed_article.py
--rw-r--r--   0        0        0      839 2023-06-03 02:44:02.552566 pubmed_types-0.1.1/src/pubmed_types/models/pubmed_article_set.py
--rw-r--r--   0        0        0      611 2023-06-03 02:44:02.556566 pubmed_types-0.1.1/src/pubmed_types/models/pubmed_book_article.py
--rw-r--r--   0        0        0      384 2023-06-03 02:44:02.556566 pubmed_types-0.1.1/src/pubmed_types/models/pubmed_book_article_set.py
--rw-r--r--   0        0        0      991 2023-06-03 02:44:02.572566 pubmed_types-0.1.1/src/pubmed_types/models/pubmed_book_data.py
--rw-r--r--   0        0        0     1217 2023-06-03 02:44:02.572566 pubmed_types-0.1.1/src/pubmed_types/models/pubmed_data.py
--rw-r--r--   0        0        0      724 2023-06-03 02:44:02.644565 pubmed_types-0.1.1/src/pubmed_types/models/qualifier_name.py
--rw-r--r--   0        0        0       87 2023-06-03 02:44:02.840563 pubmed_types-0.1.1/src/pubmed_types/models/qualifier_name_major_topic_yn.py
--rw-r--r--   0        0        0      268 2023-06-03 02:44:02.800563 pubmed_types-0.1.1/src/pubmed_types/models/question_question_response_type.py
--rw-r--r--   0        0        0      695 2023-06-03 02:44:02.344569 pubmed_types-0.1.1/src/pubmed_types/models/ref_count.py
--rw-r--r--   0        0        0      576 2023-06-03 02:44:02.644565 pubmed_types-0.1.1/src/pubmed_types/models/reference.py
--rw-r--r--   0        0        0      678 2023-06-03 02:44:02.644565 pubmed_types-0.1.1/src/pubmed_types/models/reference_list.py
--rw-r--r--   0        0        0      460 2023-06-03 02:18:03.773929 pubmed_types-0.1.1/src/pubmed_types/models/replaces.py
--rw-r--r--   0        0        0      192 2023-06-03 02:18:04.045925 pubmed_types-0.1.1/src/pubmed_types/models/replaces_id_type.py
--rw-r--r--   0        0        0     1440 2023-06-03 02:44:02.348569 pubmed_types-0.1.1/src/pubmed_types/models/resource_group.py
--rw-r--r--   0        0        0     2014 2023-06-03 02:44:02.348569 pubmed_types-0.1.1/src/pubmed_types/models/resource_id.py
--rw-r--r--   0        0        0     4999 2023-06-03 02:44:02.356569 pubmed_types-0.1.1/src/pubmed_types/models/resource_name.py
--rw-r--r--   0        0        0     1009 2023-06-03 02:44:02.360569 pubmed_types-0.1.1/src/pubmed_types/models/resource_wrap.py
--rw-r--r--   0        0        0     2223 2023-06-03 02:44:02.364569 pubmed_types-0.1.1/src/pubmed_types/models/response.py
--rw-r--r--   0        0        0     3137 2023-06-03 02:44:02.368569 pubmed_types-0.1.1/src/pubmed_types/models/restricted_by.py
--rw-r--r--   0        0        0       79 2023-06-03 02:44:02.772564 pubmed_types-0.1.1/src/pubmed_types/models/roman_toggle.py
--rw-r--r--   0        0        0      728 2023-06-03 02:44:02.368569 pubmed_types-0.1.1/src/pubmed_types/models/rp.py
--rw-r--r--   0        0        0     1346 2023-06-03 02:44:02.372569 pubmed_types-0.1.1/src/pubmed_types/models/rt.py
--rw-r--r--   0        0        0       83 2023-06-03 02:44:02.772564 pubmed_types-0.1.1/src/pubmed_types/models/sans_serif_toggle.py
--rw-r--r--   0        0        0       76 2023-06-03 02:44:02.776564 pubmed_types-0.1.1/src/pubmed_types/models/sc_toggle.py
--rw-r--r--   0        0        0     1337 2023-06-03 02:44:02.376569 pubmed_types-0.1.1/src/pubmed_types/models/season.py
--rw-r--r--   0        0        0      765 2023-06-03 02:44:02.648565 pubmed_types-0.1.1/src/pubmed_types/models/section.py
--rw-r--r--   0        0        0     1341 2023-06-03 02:44:02.648565 pubmed_types-0.1.1/src/pubmed_types/models/section_title.py
--rw-r--r--   0        0        0      347 2023-06-03 02:44:02.648565 pubmed_types-0.1.1/src/pubmed_types/models/sections.py
--rw-r--r--   0        0        0     9015 2023-06-03 02:44:02.388569 pubmed_types-0.1.1/src/pubmed_types/models/self_uri.py
--rw-r--r--   0        0        0     7416 2023-06-03 02:44:02.400569 pubmed_types-0.1.1/src/pubmed_types/models/series_text.py
--rw-r--r--   0        0        0     7394 2023-06-03 02:44:02.412568 pubmed_types-0.1.1/src/pubmed_types/models/series_title.py
--rw-r--r--   0        0        0     7912 2023-06-03 02:44:02.424568 pubmed_types-0.1.1/src/pubmed_types/models/sig.py
--rw-r--r--   0        0        0     8403 2023-06-03 02:44:02.440568 pubmed_types-0.1.1/src/pubmed_types/models/sig_block.py
--rw-r--r--   0        0        0     1361 2023-06-03 02:44:02.444568 pubmed_types-0.1.1/src/pubmed_types/models/state.py
--rw-r--r--   0        0        0       80 2023-06-03 02:44:02.776564 pubmed_types-0.1.1/src/pubmed_types/models/strike_toggle.py
--rw-r--r--   0        0        0     8497 2023-06-03 02:44:02.460568 pubmed_types-0.1.1/src/pubmed_types/models/string_conf.py
--rw-r--r--   0        0        0      159 2023-06-03 02:44:02.784563 pubmed_types-0.1.1/src/pubmed_types/models/string_name_name_style.py
--rw-r--r--   0        0        0       87 2023-06-03 02:44:02.780563 pubmed_types-0.1.1/src/pubmed_types/models/styled_content_toggle.py
--rw-r--r--   0        0        0      993 2023-06-03 02:44:02.924561 pubmed_types-0.1.1/src/pubmed_types/models/sub_1.py
--rw-r--r--   0        0        0       92 2023-06-03 02:44:02.780563 pubmed_types-0.1.1/src/pubmed_types/models/sub_arrange.py
--rw-r--r--   0        0        0     2576 2023-06-03 02:44:02.468568 pubmed_types-0.1.1/src/pubmed_types/models/sub_article.py
--rw-r--r--   0        0        0      999 2023-06-03 02:44:02.924561 pubmed_types-0.1.1/src/pubmed_types/models/suffix_1.py
--rw-r--r--   0        0        0      993 2023-06-03 02:44:02.928561 pubmed_types-0.1.1/src/pubmed_types/models/sup_1.py
--rw-r--r--   0        0        0       92 2023-06-03 02:44:02.780563 pubmed_types-0.1.1/src/pubmed_types/models/sup_arrange.py
--rw-r--r--   0        0        0      386 2023-06-03 02:44:02.648565 pubmed_types-0.1.1/src/pubmed_types/models/suppl_mesh_list.py
--rw-r--r--   0        0        0      668 2023-06-03 02:44:02.652565 pubmed_types-0.1.1/src/pubmed_types/models/suppl_mesh_name.py
--rw-r--r--   0        0        0      185 2023-06-03 02:44:02.836563 pubmed_types-0.1.1/src/pubmed_types/models/suppl_mesh_name_type.py
--rw-r--r--   0        0        0      124 2023-06-03 02:44:02.800563 pubmed_types-0.1.1/src/pubmed_types/models/supplementary_material_orientation.py
--rw-r--r--   0        0        0      161 2023-06-03 02:44:02.800563 pubmed_types-0.1.1/src/pubmed_types/models/supplementary_material_position.py
--rw-r--r--   0        0        0     1316 2023-06-03 02:44:02.472568 pubmed_types-0.1.1/src/pubmed_types/models/support_description.py
--rw-r--r--   0        0        0     1500 2023-06-03 02:44:02.476568 pubmed_types-0.1.1/src/pubmed_types/models/support_group.py
--rw-r--r--   0        0        0     9397 2023-06-03 02:44:02.500567 pubmed_types-0.1.1/src/pubmed_types/models/support_source.py
--rw-r--r--   0        0        0      695 2023-06-03 02:44:02.500567 pubmed_types-0.1.1/src/pubmed_types/models/table_count.py
--rw-r--r--   0        0        0      220 2023-06-03 02:44:02.804563 pubmed_types-0.1.1/src/pubmed_types/models/table_frame.py
--rw-r--r--   0        0        0      140 2023-06-03 02:44:02.804563 pubmed_types-0.1.1/src/pubmed_types/models/table_rules.py
--rw-r--r--   0        0        0      117 2023-06-03 02:44:02.820563 pubmed_types-0.1.1/src/pubmed_types/models/table_wrap_group_orientation.py
--rw-r--r--   0        0        0      154 2023-06-03 02:44:02.820563 pubmed_types-0.1.1/src/pubmed_types/models/table_wrap_group_position.py
--rw-r--r--   0        0        0      112 2023-06-03 02:44:02.800563 pubmed_types-0.1.1/src/pubmed_types/models/table_wrap_orientation.py
--rw-r--r--   0        0        0      149 2023-06-03 02:44:02.800563 pubmed_types-0.1.1/src/pubmed_types/models/table_wrap_position.py
--rw-r--r--   0        0        0      150 2023-06-03 02:44:02.816563 pubmed_types-0.1.1/src/pubmed_types/models/tbody_align.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.820563 pubmed_types-0.1.1/src/pubmed_types/models/tbody_valign.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.812563 pubmed_types-0.1.1/src/pubmed_types/models/td_align.py
--rw-r--r--   0        0        0      129 2023-06-03 02:44:02.812563 pubmed_types-0.1.1/src/pubmed_types/models/td_scope.py
--rw-r--r--   0        0        0      132 2023-06-03 02:44:02.816563 pubmed_types-0.1.1/src/pubmed_types/models/td_valign.py
--rw-r--r--   0        0        0     1386 2023-06-03 02:44:02.504567 pubmed_types-0.1.1/src/pubmed_types/models/tex_math.py
--rw-r--r--   0        0        0      128 2023-06-03 02:44:02.780563 pubmed_types-0.1.1/src/pubmed_types/models/tex_math_notation.py
--rw-r--r--   0        0        0      150 2023-06-03 02:44:02.816563 pubmed_types-0.1.1/src/pubmed_types/models/tfoot_align.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.816563 pubmed_types-0.1.1/src/pubmed_types/models/tfoot_valign.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.812563 pubmed_types-0.1.1/src/pubmed_types/models/th_align.py
--rw-r--r--   0        0        0      129 2023-06-03 02:44:02.812563 pubmed_types-0.1.1/src/pubmed_types/models/th_scope.py
--rw-r--r--   0        0        0      132 2023-06-03 02:44:02.812563 pubmed_types-0.1.1/src/pubmed_types/models/th_valign.py
--rw-r--r--   0        0        0      150 2023-06-03 02:44:02.808563 pubmed_types-0.1.1/src/pubmed_types/models/thead_align.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.808563 pubmed_types-0.1.1/src/pubmed_types/models/thead_valign.py
--rw-r--r--   0        0        0     1542 2023-06-03 02:44:02.508567 pubmed_types-0.1.1/src/pubmed_types/models/title_group.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.808563 pubmed_types-0.1.1/src/pubmed_types/models/tr_align.py
--rw-r--r--   0        0        0      132 2023-06-03 02:44:02.808563 pubmed_types-0.1.1/src/pubmed_types/models/tr_valign.py
--rw-r--r--   0        0        0     8912 2023-06-03 02:44:02.520567 pubmed_types-0.1.1/src/pubmed_types/models/trans_abstract.py
--rw-r--r--   0        0        0     7376 2023-06-03 02:44:02.532567 pubmed_types-0.1.1/src/pubmed_types/models/trans_subtitle.py
--rw-r--r--   0        0        0     1641 2023-06-03 02:44:02.536567 pubmed_types-0.1.1/src/pubmed_types/models/trans_title_group.py
--rw-r--r--   0        0        0     2610 2023-06-03 02:44:02.584566 pubmed_types-0.1.1/src/pubmed_types/models/u.py
--rw-r--r--   0        0        0      866 2023-06-03 02:44:02.536567 pubmed_types-0.1.1/src/pubmed_types/models/underline_end.py
--rw-r--r--   0        0        0      750 2023-06-03 02:44:02.540567 pubmed_types-0.1.1/src/pubmed_types/models/underline_start.py
--rw-r--r--   0        0        0       83 2023-06-03 02:44:02.776564 pubmed_types-0.1.1/src/pubmed_types/models/underline_toggle.py
--rw-r--r--   0        0        0      614 2023-06-03 02:44:02.652565 pubmed_types-0.1.1/src/pubmed_types/models/url.py
--rw-r--r--   0        0        0      661 2023-06-03 02:44:02.856562 pubmed_types-0.1.1/src/pubmed_types/models/url_lang.py
--rw-r--r--   0        0        0      150 2023-06-03 02:44:02.856562 pubmed_types-0.1.1/src/pubmed_types/models/url_type.py
--rw-r--r--   0        0        0     1072 2023-06-03 02:44:02.656565 pubmed_types-0.1.1/src/pubmed_types/models/vernacular_title.py
--rw-r--r--   0        0        0     2893 2023-06-03 02:44:02.544567 pubmed_types-0.1.1/src/pubmed_types/models/volume_issue_group.py
--rw-r--r--   0        0        0      962 2023-06-03 02:44:02.656565 pubmed_types-0.1.1/src/pubmed_types/models/volume_title.py
--rw-r--r--   0        0        0      692 2023-06-03 02:44:02.548566 pubmed_types-0.1.1/src/pubmed_types/models/word_count.py
--rw-r--r--   0        0        0      330 2023-06-03 02:44:02.656565 pubmed_types-0.1.1/src/pubmed_types/models/xs_pattern.py
--rw-r--r--   0        0        0     1627 2023-06-03 02:44:02.552566 pubmed_types-0.1.1/src/pubmed_types/models/year.py
--rw-r--r--   0        0        0     5086 1970-01-01 00:00:00.000000 pubmed_types-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-25 16:03:32.757838 pubmed_types-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4359 2023-06-04 14:01:16.579993 pubmed_types-0.1.2/README.md
+-rw-r--r--   0        0        0     1444 2023-06-04 14:01:16.575993 pubmed_types-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      483 2023-06-04 14:01:16.579993 pubmed_types-0.1.2/src/pubmed_types/__init__.py
+-rw-r--r--   0        0        0    24766 2023-06-03 02:43:58.380623 pubmed_types-0.1.2/src/pubmed_types/models/__init__.py
+-rw-r--r--   0        0        0     7420 2023-06-03 02:44:01.924575 pubmed_types-0.1.2/src/pubmed_types/models/abbrev_journal_title.py
+-rw-r--r--   0        0        0      610 2023-06-03 02:44:02.860562 pubmed_types-0.1.2/src/pubmed_types/models/abstract_1.py
+-rw-r--r--   0        0        0     1645 2023-06-03 02:44:02.572566 pubmed_types-0.1.2/src/pubmed_types/models/abstract_text.py
+-rw-r--r--   0        0        0      229 2023-06-03 02:44:02.832563 pubmed_types-0.1.2/src/pubmed_types/models/abstract_text_nlm_category.py
+-rw-r--r--   0        0        0  1064015 2023-06-03 02:44:01.912575 pubmed_types-0.1.2/src/pubmed_types/models/access_date.py
+-rw-r--r--   0        0        0      342 2023-06-03 02:44:02.576566 pubmed_types-0.1.2/src/pubmed_types/models/accession_number_list.py
+-rw-r--r--   0        0        0      962 2023-06-03 02:44:02.576566 pubmed_types-0.1.2/src/pubmed_types/models/affiliation.py
+-rw-r--r--   0        0        0      588 2023-06-03 02:44:02.576566 pubmed_types-0.1.2/src/pubmed_types/models/affiliation_info.py
+-rw-r--r--   0        0        0     1373 2023-06-03 02:44:01.924575 pubmed_types-0.1.2/src/pubmed_types/models/alt_text.py
+-rw-r--r--   0        0        0     8831 2023-06-03 02:44:01.944575 pubmed_types-0.1.2/src/pubmed_types/models/app.py
+-rw-r--r--   0        0        0     8786 2023-06-03 02:44:01.960574 pubmed_types-0.1.2/src/pubmed_types/models/app_group.py
+-rw-r--r--   0        0        0      419 2023-06-03 02:18:03.813928 pubmed_types-0.1.2/src/pubmed_types/models/archive_copy_source.py
+-rw-r--r--   0        0        0      108 2023-06-03 02:44:02.776564 pubmed_types-0.1.2/src/pubmed_types/models/array_orientation.py
+-rw-r--r--   0        0        0     3079 2023-06-03 02:44:02.864562 pubmed_types-0.1.2/src/pubmed_types/models/article_1.py
+-rw-r--r--   0        0        0     2649 2023-06-03 02:44:02.876562 pubmed_types-0.1.2/src/pubmed_types/models/article_2.py
+-rw-r--r--   0        0        0     1202 2023-06-03 02:44:01.960574 pubmed_types-0.1.2/src/pubmed_types/models/article_categories.py
+-rw-r--r--   0        0        0      878 2023-06-03 02:44:02.576566 pubmed_types-0.1.2/src/pubmed_types/models/article_date.py
+-rw-r--r--   0        0        0      369 2023-06-03 02:44:02.824563 pubmed_types-0.1.2/src/pubmed_types/models/article_dtd_version.py
+-rw-r--r--   0        0        0     1423 2023-06-03 02:44:01.964574 pubmed_types-0.1.2/src/pubmed_types/models/article_id.py
+-rw-r--r--   0        0        0      511 2023-06-03 02:44:02.876562 pubmed_types-0.1.2/src/pubmed_types/models/article_id_1.py
+-rw-r--r--   0        0        0      303 2023-06-03 02:44:02.848563 pubmed_types-0.1.2/src/pubmed_types/models/article_id_id_type.py
+-rw-r--r--   0        0        0      368 2023-06-03 02:44:02.580566 pubmed_types-0.1.2/src/pubmed_types/models/article_id_list.py
+-rw-r--r--   0        0        0     9515 2023-06-03 02:44:01.980574 pubmed_types-0.1.2/src/pubmed_types/models/article_meta.py
+-rw-r--r--   0        0        0      242 2023-06-03 02:44:02.828563 pubmed_types-0.1.2/src/pubmed_types/models/article_pub_model.py
+-rw-r--r--   0        0        0      353 2023-06-03 02:18:03.769929 pubmed_types-0.1.2/src/pubmed_types/models/article_set.py
+-rw-r--r--   0        0        0     1495 2023-06-03 02:44:02.880562 pubmed_types-0.1.2/src/pubmed_types/models/article_title_1.py
+-rw-r--r--   0        0        0     3823 2023-06-03 02:44:01.988574 pubmed_types-0.1.2/src/pubmed_types/models/article_version.py
+-rw-r--r--   0        0        0      827 2023-06-03 02:44:01.992574 pubmed_types-0.1.2/src/pubmed_types/models/article_version_alternatives.py
+-rw-r--r--   0        0        0     1938 2023-06-03 02:44:02.580566 pubmed_types-0.1.2/src/pubmed_types/models/author.py
+-rw-r--r--   0        0        0       80 2023-06-03 02:44:02.836563 pubmed_types-0.1.2/src/pubmed_types/models/author_equal_contrib.py
+-rw-r--r--   0        0        0      838 2023-06-03 02:44:02.584566 pubmed_types-0.1.2/src/pubmed_types/models/author_list.py
+-rw-r--r--   0        0        0       82 2023-06-03 02:44:02.832563 pubmed_types-0.1.2/src/pubmed_types/models/author_list_complete_yn.py
+-rw-r--r--   0        0        0      100 2023-06-03 02:44:02.832563 pubmed_types-0.1.2/src/pubmed_types/models/author_list_type.py
+-rw-r--r--   0        0        0     1720 2023-06-03 02:44:02.000574 pubmed_types-0.1.2/src/pubmed_types/models/author_notes.py
+-rw-r--r--   0        0        0       75 2023-06-03 02:44:02.836563 pubmed_types-0.1.2/src/pubmed_types/models/author_valid_yn.py
+-rw-r--r--   0        0        0     2449 2023-06-03 02:44:02.004574 pubmed_types-0.1.2/src/pubmed_types/models/award_desc.py
+-rw-r--r--   0        0        0     4315 2023-06-03 02:44:02.012574 pubmed_types-0.1.2/src/pubmed_types/models/award_group.py
+-rw-r--r--   0        0        0     2442 2023-06-03 02:44:02.016574 pubmed_types-0.1.2/src/pubmed_types/models/award_name.py
+-rw-r--r--   0        0        0     2079 2023-06-03 02:44:02.020574 pubmed_types-0.1.2/src/pubmed_types/models/back.py
+-rw-r--r--   0        0        0      765 2023-06-03 02:44:02.584566 pubmed_types-0.1.2/src/pubmed_types/models/beginning_date.py
+-rw-r--r--   0        0        0     7356 2023-06-03 02:44:02.032574 pubmed_types-0.1.2/src/pubmed_types/models/body.py
+-rw-r--r--   0        0        0       78 2023-06-03 02:44:02.768564 pubmed_types-0.1.2/src/pubmed_types/models/bold_toggle.py
+-rw-r--r--   0        0        0     3125 2023-06-03 02:44:02.588566 pubmed_types-0.1.2/src/pubmed_types/models/book.py
+-rw-r--r--   0        0        0     4185 2023-06-03 02:44:02.560566 pubmed_types-0.1.2/src/pubmed_types/models/book_document.py
+-rw-r--r--   0        0        0      587 2023-06-03 02:44:02.556566 pubmed_types-0.1.2/src/pubmed_types/models/book_document_set.py
+-rw-r--r--   0        0        0     1444 2023-06-03 02:44:02.592566 pubmed_types-0.1.2/src/pubmed_types/models/book_title.py
+-rw-r--r--   0        0        0      112 2023-06-03 02:44:02.784563 pubmed_types-0.1.2/src/pubmed_types/models/boxed_text_orientation.py
+-rw-r--r--   0        0        0      149 2023-06-03 02:44:02.788563 pubmed_types-0.1.2/src/pubmed_types/models/boxed_text_position.py
+-rw-r--r--   0        0        0      529 2023-06-03 02:44:02.032574 pubmed_types-0.1.2/src/pubmed_types/models/break_mod.py
+-rw-r--r--   0        0        0      117 2023-06-03 02:44:02.788563 pubmed_types-0.1.2/src/pubmed_types/models/chem_struct_wrap_orientation.py
+-rw-r--r--   0        0        0      154 2023-06-03 02:44:02.788563 pubmed_types-0.1.2/src/pubmed_types/models/chem_struct_wrap_position.py
+-rw-r--r--   0        0        0      592 2023-06-03 02:44:02.592566 pubmed_types-0.1.2/src/pubmed_types/models/chemical.py
+-rw-r--r--   0        0        0      356 2023-06-03 02:44:02.592566 pubmed_types-0.1.2/src/pubmed_types/models/chemical_list.py
+-rw-r--r--   0        0        0     1065 2023-06-03 02:44:02.592566 pubmed_types-0.1.2/src/pubmed_types/models/citation.py
+-rw-r--r--   0        0        0     1344 2023-06-03 02:44:02.036574 pubmed_types-0.1.2/src/pubmed_types/models/city.py
+-rw-r--r--   0        0        0       82 2023-06-03 02:44:02.788563 pubmed_types-0.1.2/src/pubmed_types/models/code_executable.py
+-rw-r--r--   0        0        0      107 2023-06-03 02:44:02.788563 pubmed_types-0.1.2/src/pubmed_types/models/code_orientation.py
+-rw-r--r--   0        0        0      144 2023-06-03 02:44:02.788563 pubmed_types-0.1.2/src/pubmed_types/models/code_position.py
+-rw-r--r--   0        0        0      963 2023-06-03 02:44:02.596566 pubmed_types-0.1.2/src/pubmed_types/models/coi_statement.py
+-rw-r--r--   0        0        0     1574 2023-06-03 02:44:02.036574 pubmed_types-0.1.2/src/pubmed_types/models/col.py
+-rw-r--r--   0        0        0      148 2023-06-03 02:44:02.804563 pubmed_types-0.1.2/src/pubmed_types/models/col_align.py
+-rw-r--r--   0        0        0      133 2023-06-03 02:44:02.804563 pubmed_types-0.1.2/src/pubmed_types/models/col_valign.py
+-rw-r--r--   0        0        0     1765 2023-06-03 02:44:02.040573 pubmed_types-0.1.2/src/pubmed_types/models/colgroup.py
+-rw-r--r--   0        0        0      153 2023-06-03 02:44:02.808563 pubmed_types-0.1.2/src/pubmed_types/models/colgroup_align.py
+-rw-r--r--   0        0        0      138 2023-06-03 02:44:02.808563 pubmed_types-0.1.2/src/pubmed_types/models/colgroup_valign.py
+-rw-r--r--   0        0        0     1450 2023-06-03 02:44:02.596566 pubmed_types-0.1.2/src/pubmed_types/models/collection_title.py
+-rw-r--r--   0        0        0      965 2023-06-03 02:44:02.600566 pubmed_types-0.1.2/src/pubmed_types/models/collective_name.py
+-rw-r--r--   0        0        0      934 2023-06-03 02:44:02.600566 pubmed_types-0.1.2/src/pubmed_types/models/comments_corrections.py
+-rw-r--r--   0        0        0      424 2023-06-03 02:44:02.600566 pubmed_types-0.1.2/src/pubmed_types/models/comments_corrections_list.py
+-rw-r--r--   0        0        0     1025 2023-06-03 02:44:02.840563 pubmed_types-0.1.2/src/pubmed_types/models/comments_corrections_ref_type.py
+-rw-r--r--   0        0        0     7391 2023-06-03 02:44:02.052573 pubmed_types-0.1.2/src/pubmed_types/models/conf_num.py
+-rw-r--r--   0        0        0     7394 2023-06-03 02:44:02.064573 pubmed_types-0.1.2/src/pubmed_types/models/conf_theme.py
+-rw-r--r--   0        0        0     4292 2023-06-03 02:44:02.068573 pubmed_types-0.1.2/src/pubmed_types/models/conference.py
+-rw-r--r--   0        0        0       82 2023-06-03 02:44:02.780563 pubmed_types-0.1.2/src/pubmed_types/models/contrib_corresp.py
+-rw-r--r--   0        0        0       83 2023-06-03 02:44:02.784563 pubmed_types-0.1.2/src/pubmed_types/models/contrib_deceased.py
+-rw-r--r--   0        0        0       87 2023-06-03 02:44:02.784563 pubmed_types-0.1.2/src/pubmed_types/models/contrib_equal_contrib.py
+-rw-r--r--   0        0        0     1940 2023-06-03 02:44:02.072573 pubmed_types-0.1.2/src/pubmed_types/models/contrib_id.py
+-rw-r--r--   0        0        0       98 2023-06-03 02:44:02.784563 pubmed_types-0.1.2/src/pubmed_types/models/contrib_id_authenticated.py
+-rw-r--r--   0        0        0     1889 2023-06-03 02:44:02.076573 pubmed_types-0.1.2/src/pubmed_types/models/contributed_resource_group.py
+-rw-r--r--   0        0        0      768 2023-06-03 02:44:02.600566 pubmed_types-0.1.2/src/pubmed_types/models/contribution_date.py
+-rw-r--r--   0        0        0     1083 2023-06-03 02:44:02.080573 pubmed_types-0.1.2/src/pubmed_types/models/copyright_year.py
+-rw-r--r--   0        0        0     8856 2023-06-03 02:44:02.092573 pubmed_types-0.1.2/src/pubmed_types/models/corresp.py
+-rw-r--r--   0        0        0      871 2023-06-03 02:44:02.096573 pubmed_types-0.1.2/src/pubmed_types/models/count.py
+-rw-r--r--   0        0        0     1907 2023-06-03 02:44:02.100573 pubmed_types-0.1.2/src/pubmed_types/models/counts.py
+-rw-r--r--   0        0        0     3702 2023-06-03 02:44:02.104573 pubmed_types-0.1.2/src/pubmed_types/models/custom_meta.py
+-rw-r--r--   0        0        0     1389 2023-06-03 02:44:02.108573 pubmed_types-0.1.2/src/pubmed_types/models/custom_meta_group.py
+-rw-r--r--   0        0        0      579 2023-06-03 02:44:02.604566 pubmed_types-0.1.2/src/pubmed_types/models/data_bank.py
+-rw-r--r--   0        0        0      644 2023-06-03 02:44:02.604566 pubmed_types-0.1.2/src/pubmed_types/models/data_bank_list.py
+-rw-r--r--   0        0        0       84 2023-06-03 02:44:02.836563 pubmed_types-0.1.2/src/pubmed_types/models/data_bank_list_complete_yn.py
+-rw-r--r--   0        0        0      672 2023-06-03 02:44:02.604566 pubmed_types-0.1.2/src/pubmed_types/models/date_completed.py
+-rw-r--r--   0        0        0      670 2023-06-03 02:44:02.604566 pubmed_types-0.1.2/src/pubmed_types/models/date_revised.py
+-rw-r--r--   0        0        0     1328 2023-06-03 02:44:02.108573 pubmed_types-0.1.2/src/pubmed_types/models/day.py
+-rw-r--r--   0        0        0      338 2023-06-03 02:44:02.564566 pubmed_types-0.1.2/src/pubmed_types/models/delete_citation.py
+-rw-r--r--   0        0        0      309 2023-06-03 02:44:02.564566 pubmed_types-0.1.2/src/pubmed_types/models/delete_document.py
+-rw-r--r--   0        0        0      948 2023-06-03 02:44:02.608566 pubmed_types-0.1.2/src/pubmed_types/models/descriptor_name.py
+-rw-r--r--   0        0        0       88 2023-06-03 02:44:02.840563 pubmed_types-0.1.2/src/pubmed_types/models/descriptor_name_major_topic_yn.py
+-rw-r--r--   0        0        0       86 2023-06-03 02:44:02.840563 pubmed_types-0.1.2/src/pubmed_types/models/descriptor_name_type.py
+-rw-r--r--   0        0        0      331 2023-06-03 02:44:02.884562 pubmed_types-0.1.2/src/pubmed_types/models/disp_formula_1.py
+-rw-r--r--   0        0        0     1217 2023-06-03 02:44:02.112573 pubmed_types-0.1.2/src/pubmed_types/models/elocation_id.py
+-rw-r--r--   0        0        0      809 2023-06-03 02:44:02.884562 pubmed_types-0.1.2/src/pubmed_types/models/elocation_id_1.py
+-rw-r--r--   0        0        0       88 2023-06-03 02:44:02.832563 pubmed_types-0.1.2/src/pubmed_types/models/elocation_id_eid_type.py
+-rw-r--r--   0        0        0       80 2023-06-03 02:44:02.832563 pubmed_types-0.1.2/src/pubmed_types/models/elocation_id_valid_yn.py
+-rw-r--r--   0        0        0      762 2023-06-03 02:44:02.608566 pubmed_types-0.1.2/src/pubmed_types/models/ending_date.py
+-rw-r--r--   0        0        0      704 2023-06-03 02:44:02.116572 pubmed_types-0.1.2/src/pubmed_types/models/equation_count.py
+-rw-r--r--   0        0        0     1328 2023-06-03 02:44:02.116572 pubmed_types-0.1.2/src/pubmed_types/models/era.py
+-rw-r--r--   0        0        0     3816 2023-06-03 02:44:02.124572 pubmed_types-0.1.2/src/pubmed_types/models/event.py
+-rw-r--r--   0        0        0     3116 2023-06-03 02:44:02.132572 pubmed_types-0.1.2/src/pubmed_types/models/event_desc.py
+-rw-r--r--   0        0        0     3131 2023-06-03 02:44:02.136572 pubmed_types-0.1.2/src/pubmed_types/models/extended_by.py
+-rw-r--r--   0        0        0      692 2023-06-03 02:44:02.140572 pubmed_types-0.1.2/src/pubmed_types/models/fig_count.py
+-rw-r--r--   0        0        0      111 2023-06-03 02:44:02.796563 pubmed_types-0.1.2/src/pubmed_types/models/fig_group_orientation.py
+-rw-r--r--   0        0        0      148 2023-06-03 02:44:02.796563 pubmed_types-0.1.2/src/pubmed_types/models/fig_group_position.py
+-rw-r--r--   0        0        0      106 2023-06-03 02:44:02.792563 pubmed_types-0.1.2/src/pubmed_types/models/fig_orientation.py
+-rw-r--r--   0        0        0      143 2023-06-03 02:44:02.792563 pubmed_types-0.1.2/src/pubmed_types/models/fig_position.py
+-rw-r--r--   0        0        0      467 2023-06-03 02:18:03.781929 pubmed_types-0.1.2/src/pubmed_types/models/first_name.py
+-rw-r--r--   0        0        0       78 2023-06-03 02:18:04.049925 pubmed_types-0.1.2/src/pubmed_types/models/first_name_empty_yn.py
+-rw-r--r--   0        0        0      458 2023-06-03 02:18:03.777929 pubmed_types-0.1.2/src/pubmed_types/models/first_page.py
+-rw-r--r--   0        0        0      112 2023-06-03 02:18:04.045925 pubmed_types-0.1.2/src/pubmed_types/models/first_page_lzero.py
+-rw-r--r--   0        0        0     2865 2023-06-03 02:44:02.144572 pubmed_types-0.1.2/src/pubmed_types/models/floats_group.py
+-rw-r--r--   0        0        0     1461 2023-06-03 02:44:02.148572 pubmed_types-0.1.2/src/pubmed_types/models/fpage.py
+-rw-r--r--   0        0        0     2105 2023-06-03 02:44:02.156572 pubmed_types-0.1.2/src/pubmed_types/models/front.py
+-rw-r--r--   0        0        0     9514 2023-06-03 02:44:02.168572 pubmed_types-0.1.2/src/pubmed_types/models/front_stub.py
+-rw-r--r--   0        0        0     1657 2023-06-03 02:44:02.168572 pubmed_types-0.1.2/src/pubmed_types/models/funding_group.py
+-rw-r--r--   0        0        0     9232 2023-06-03 02:44:02.184572 pubmed_types-0.1.2/src/pubmed_types/models/funding_statement.py
+-rw-r--r--   0        0        0      327 2023-06-03 02:44:02.608566 pubmed_types-0.1.2/src/pubmed_types/models/gene_symbol_list.py
+-rw-r--r--   0        0        0      465 2023-06-03 02:44:02.612566 pubmed_types-0.1.2/src/pubmed_types/models/general_note.py
+-rw-r--r--   0        0        0      152 2023-06-03 02:44:02.844563 pubmed_types-0.1.2/src/pubmed_types/models/general_note_owner.py
+-rw-r--r--   0        0        0     1866 2023-06-03 02:44:02.184572 pubmed_types-0.1.2/src/pubmed_types/models/glyph_data.py
+-rw-r--r--   0        0        0      728 2023-06-03 02:44:02.188572 pubmed_types-0.1.2/src/pubmed_types/models/glyph_ref.py
+-rw-r--r--   0        0        0      806 2023-06-03 02:44:02.612566 pubmed_types-0.1.2/src/pubmed_types/models/grant.py
+-rw-r--r--   0        0        0      611 2023-06-03 02:44:02.612566 pubmed_types-0.1.2/src/pubmed_types/models/grant_list.py
+-rw-r--r--   0        0        0       81 2023-06-03 02:44:02.836563 pubmed_types-0.1.2/src/pubmed_types/models/grant_list_complete_yn.py
+-rw-r--r--   0        0        0      110 2023-06-03 02:44:02.792563 pubmed_types-0.1.2/src/pubmed_types/models/graphic_orientation.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.792563 pubmed_types-0.1.2/src/pubmed_types/models/graphic_position.py
+-rw-r--r--   0        0        0      551 2023-06-03 02:18:03.805928 pubmed_types-0.1.2/src/pubmed_types/models/group.py
+-rw-r--r--   0        0        0      338 2023-06-03 02:18:03.805928 pubmed_types-0.1.2/src/pubmed_types/models/group_list.py
+-rw-r--r--   0        0        0      425 2023-06-03 02:44:02.888562 pubmed_types-0.1.2/src/pubmed_types/models/history_1.py
+-rw-r--r--   0        0        0     7177 2023-06-03 02:44:02.908562 pubmed_types-0.1.2/src/pubmed_types/models/history_2.py
+-rw-r--r--   0        0        0      528 2023-06-03 02:44:02.192571 pubmed_types-0.1.2/src/pubmed_types/models/hr.py
+-rw-r--r--   0        0        0     3870 2023-06-03 02:18:03.805928 pubmed_types-0.1.2/src/pubmed_types/models/i.py
+-rw-r--r--   0        0        0      426 2023-06-03 02:44:02.616566 pubmed_types-0.1.2/src/pubmed_types/models/identifier.py
+-rw-r--r--   0        0        0      718 2023-06-03 02:44:02.192571 pubmed_types-0.1.2/src/pubmed_types/models/index_term_range_end.py
+-rw-r--r--   0        0        0     1475 2023-06-03 02:18:03.809928 pubmed_types-0.1.2/src/pubmed_types/models/individual_name.py
+-rw-r--r--   0        0        0     2029 2023-06-03 02:44:02.200571 pubmed_types-0.1.2/src/pubmed_types/models/institution_id.py
+-rw-r--r--   0        0        0     1537 2023-06-03 02:44:02.616566 pubmed_types-0.1.2/src/pubmed_types/models/investigator.py
+-rw-r--r--   0        0        0      380 2023-06-03 02:44:02.616566 pubmed_types-0.1.2/src/pubmed_types/models/investigator_list.py
+-rw-r--r--   0        0        0       81 2023-06-03 02:44:02.844563 pubmed_types-0.1.2/src/pubmed_types/models/investigator_valid_yn.py
+-rw-r--r--   0        0        0      515 2023-06-03 02:44:02.908562 pubmed_types-0.1.2/src/pubmed_types/models/issn_1.py
+-rw-r--r--   0        0        0      100 2023-06-03 02:44:02.828563 pubmed_types-0.1.2/src/pubmed_types/models/issn_issn_type.py
+-rw-r--r--   0        0        0     3124 2023-06-03 02:44:02.204571 pubmed_types-0.1.2/src/pubmed_types/models/issue_id.py
+-rw-r--r--   0        0        0     7395 2023-06-03 02:44:02.216571 pubmed_types-0.1.2/src/pubmed_types/models/issue_sponsor.py
+-rw-r--r--   0        0        0     7400 2023-06-03 02:44:02.228571 pubmed_types-0.1.2/src/pubmed_types/models/issue_subtitle.py
+-rw-r--r--   0        0        0     1874 2023-06-03 02:44:02.228571 pubmed_types-0.1.2/src/pubmed_types/models/issue_title_group.py
+-rw-r--r--   0        0        0       80 2023-06-03 02:44:02.768564 pubmed_types-0.1.2/src/pubmed_types/models/italic_toggle.py
+-rw-r--r--   0        0        0      508 2023-06-03 02:44:02.620566 pubmed_types-0.1.2/src/pubmed_types/models/item_list.py
+-rw-r--r--   0        0        0      873 2023-06-03 02:44:02.620566 pubmed_types-0.1.2/src/pubmed_types/models/journal.py
+-rw-r--r--   0        0        0     1543 2023-06-03 02:44:02.232571 pubmed_types-0.1.2/src/pubmed_types/models/journal_id.py
+-rw-r--r--   0        0        0      942 2023-06-03 02:44:02.620566 pubmed_types-0.1.2/src/pubmed_types/models/journal_issue.py
+-rw-r--r--   0        0        0      107 2023-06-03 02:44:02.832563 pubmed_types-0.1.2/src/pubmed_types/models/journal_issue_cited_medium.py
+-rw-r--r--   0        0        0     2752 2023-06-03 02:44:02.236571 pubmed_types-0.1.2/src/pubmed_types/models/journal_meta.py
+-rw-r--r--   0        0        0     7406 2023-06-03 02:44:02.252570 pubmed_types-0.1.2/src/pubmed_types/models/journal_subtitle.py
+-rw-r--r--   0        0        0     7404 2023-06-03 02:44:02.264570 pubmed_types-0.1.2/src/pubmed_types/models/journal_title.py
+-rw-r--r--   0        0        0     1683 2023-06-03 02:44:02.268570 pubmed_types-0.1.2/src/pubmed_types/models/journal_title_group.py
+-rw-r--r--   0        0        0     1342 2023-06-03 02:44:02.624565 pubmed_types-0.1.2/src/pubmed_types/models/keyword.py
+-rw-r--r--   0        0        0      601 2023-06-03 02:44:02.624565 pubmed_types-0.1.2/src/pubmed_types/models/keyword_list.py
+-rw-r--r--   0        0        0      184 2023-06-03 02:44:02.844563 pubmed_types-0.1.2/src/pubmed_types/models/keyword_list_owner.py
+-rw-r--r--   0        0        0       81 2023-06-03 02:44:02.844563 pubmed_types-0.1.2/src/pubmed_types/models/keyword_major_topic_yn.py
+-rw-r--r--   0        0        0      460 2023-06-03 02:44:02.624565 pubmed_types-0.1.2/src/pubmed_types/models/location_label.py
+-rw-r--r--   0        0        0      205 2023-06-03 02:44:02.852563 pubmed_types-0.1.2/src/pubmed_types/models/location_label_type.py
+-rw-r--r--   0        0        0     1338 2023-06-03 02:44:02.272570 pubmed_types-0.1.2/src/pubmed_types/models/lpage.py
+-rw-r--r--   0        0        0      108 2023-06-03 02:44:02.792563 pubmed_types-0.1.2/src/pubmed_types/models/media_orientation.py
+-rw-r--r--   0        0        0      145 2023-06-03 02:44:02.796563 pubmed_types-0.1.2/src/pubmed_types/models/media_position.py
+-rw-r--r--   0        0        0     5578 2023-06-03 02:44:02.568566 pubmed_types-0.1.2/src/pubmed_types/models/medline_citation.py
+-rw-r--r--   0        0        0      178 2023-06-03 02:44:02.828563 pubmed_types-0.1.2/src/pubmed_types/models/medline_citation_owner.py
+-rw-r--r--   0        0        0      284 2023-06-03 02:44:02.828563 pubmed_types-0.1.2/src/pubmed_types/models/medline_citation_status.py
+-rw-r--r--   0        0        0      813 2023-06-03 02:44:02.624565 pubmed_types-0.1.2/src/pubmed_types/models/medline_journal_info.py
+-rw-r--r--   0        0        0      618 2023-06-03 02:44:02.628565 pubmed_types-0.1.2/src/pubmed_types/models/mesh_heading.py
+-rw-r--r--   0        0        0      376 2023-06-03 02:44:02.628565 pubmed_types-0.1.2/src/pubmed_types/models/mesh_heading_list.py
+-rw-r--r--   0        0        0     6803 2023-06-03 02:44:02.284570 pubmed_types-0.1.2/src/pubmed_types/models/meta_name.py
+-rw-r--r--   0        0        0     6806 2023-06-03 02:44:02.296570 pubmed_types-0.1.2/src/pubmed_types/models/meta_value.py
+-rw-r--r--   0        0        0     1408 2023-06-03 02:44:02.300570 pubmed_types-0.1.2/src/pubmed_types/models/milestone_end.py
+-rw-r--r--   0        0        0     1414 2023-06-03 02:44:02.304570 pubmed_types-0.1.2/src/pubmed_types/models/milestone_start.py
+-rw-r--r--   0        0        0       83 2023-06-03 02:44:02.772564 pubmed_types-0.1.2/src/pubmed_types/models/monospace_toggle.py
+-rw-r--r--   0        0        0     1334 2023-06-03 02:44:02.304570 pubmed_types-0.1.2/src/pubmed_types/models/month.py
+-rw-r--r--   0        0        0      153 2023-06-03 02:44:02.784563 pubmed_types-0.1.2/src/pubmed_types/models/name_name_style.py
+-rw-r--r--   0        0        0      423 2023-06-03 02:44:02.628565 pubmed_types-0.1.2/src/pubmed_types/models/name_of_substance.py
+-rw-r--r--   0        0        0     1422 2023-06-03 02:44:02.308570 pubmed_types-0.1.2/src/pubmed_types/models/object_id.py
+-rw-r--r--   0        0        0      354 2023-06-03 02:44:02.632565 pubmed_types-0.1.2/src/pubmed_types/models/object_list.py
+-rw-r--r--   0        0        0      497 2023-06-03 02:44:02.632565 pubmed_types-0.1.2/src/pubmed_types/models/object_mod.py
+-rw-r--r--   0        0        0       81 2023-06-03 02:44:02.820563 pubmed_types-0.1.2/src/pubmed_types/models/option_correct.py
+-rw-r--r--   0        0        0       15 2023-06-03 02:17:59.961981 pubmed_types-0.1.2/src/pubmed_types/models/org/__init__.py
+-rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.2/src/pubmed_types/models/org/niso/__init__.py
+-rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.2/src/pubmed_types/models/org/niso/schemas/__init__.py
+-rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.2/src/pubmed_types/models/org/niso/schemas/ali/__init__.py
+-rw-r--r--   0        0        0      124 2023-06-03 02:43:58.380623 pubmed_types-0.1.2/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/__init__.py
+-rw-r--r--   0        0        0      631 2023-06-03 02:44:02.552566 pubmed_types-0.1.2/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/free_to_read.py
+-rw-r--r--   0        0        0      578 2023-06-03 02:44:02.552566 pubmed_types-0.1.2/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/license_ref.py
+-rw-r--r--   0        0        0       15 2023-06-03 02:17:59.961981 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/__init__.py
+-rw-r--r--   0        0        0       15 2023-06-03 02:17:59.989981 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/__init__.py
+-rw-r--r--   0        0        0       15 2023-06-03 02:17:59.989981 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/__init__.py
+-rw-r--r--   0        0        0    18558 2023-06-03 02:43:58.344624 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/__init__.py
+-rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.116600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/abs.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.132599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/and_mod.py
+-rw-r--r--   0        0        0     2149 2023-06-03 02:44:00.364596 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/annotation.py
+-rw-r--r--   0        0        0     1582 2023-06-03 02:44:00.148599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/approx.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.184599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccos.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.184599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccosh.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.184599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccot.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.188599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccoth.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.188599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccsc.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.188599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccsch.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.188599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arcsec.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.188599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arcsech.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.180599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arcsin.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.192599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arcsinh.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.184599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arctan.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.192599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arctanh.py
+-rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.120600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arg.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.164599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/card.py
+-rw-r--r--   0        0        0      466 2023-06-03 02:44:00.160599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cartesianproduct.py
+-rw-r--r--   0        0        0     1737 2023-06-03 02:44:00.092600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cbytes.py
+-rw-r--r--   0        0        0     1584 2023-06-03 02:44:00.128600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ceiling.py
+-rw-r--r--   0        0        0      450 2023-06-03 02:44:00.096600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/codomain.py
+-rw-r--r--   0        0        0      168 2023-06-03 02:44:00.224598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/columnalignstyle.py
+-rw-r--r--   0        0        0      452 2023-06-03 02:44:00.208598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/complexes.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.104600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/compose.py
+-rw-r--r--   0        0        0  1555308 2023-06-03 02:44:00.088600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/condition.py
+-rw-r--r--   0        0        0     1588 2023-06-03 02:44:00.120600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/conjugate.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cos.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.176599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cosh.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.176599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cot.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.180599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/coth.py
+-rw-r--r--   0        0        0     1767 2023-06-03 02:44:00.092600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cs.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/csc.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.180599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/csch.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.156599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/curl.py
+-rw-r--r--   0        0        0      189 2023-06-03 02:44:02.664565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/declare_occurrence.py
+-rw-r--r--   0        0        0      456 2023-06-03 02:44:00.196599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/determinant.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.152599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/diff.py
+-rw-r--r--   0        0        0      454 2023-06-03 02:44:00.156599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/divergence.py
+-rw-r--r--   0        0        0     1582 2023-06-03 02:44:00.108600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/divide.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.096600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/domain.py
+-rw-r--r--   0        0        0      450 2023-06-03 02:44:00.208598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/emptyset.py
+-rw-r--r--   0        0        0      438 2023-06-03 02:44:00.140599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/eq.py
+-rw-r--r--   0        0        0      454 2023-06-03 02:44:00.140599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/equivalent.py
+-rw-r--r--   0        0        0      454 2023-06-03 02:44:00.216598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/eulergamma.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.140599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/exists.py
+-rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.128600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/exp.py
+-rw-r--r--   0        0        0      458 2023-06-03 02:44:00.208598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/exponentiale.py
+-rw-r--r--   0        0        0     1588 2023-06-03 02:44:00.116600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/factorial.py
+-rw-r--r--   0        0        0     1586 2023-06-03 02:44:00.148599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/factorof.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.212598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/false.py
+-rw-r--r--   0        0        0     1580 2023-06-03 02:44:00.124600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/floor.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.140599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/forall.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.132599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/gcd.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.144599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/geq.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.156599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/grad.py
+-rw-r--r--   0        0        0      438 2023-06-03 02:44:00.140599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/gt.py
+-rw-r--r--   0        0        0      444 2023-06-03 02:44:00.096600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ident.py
+-rw-r--r--   0        0        0      444 2023-06-03 02:44:00.100600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/image.py
+-rw-r--r--   0        0        0     1588 2023-06-03 02:44:00.124600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/imaginary.py
+-rw-r--r--   0        0        0      454 2023-06-03 02:44:00.212598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/imaginaryi.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.136599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/implies.py
+-rw-r--r--   0        0        0      438 2023-06-03 02:44:00.160599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/in_mod.py
+-rw-r--r--   0        0        0      450 2023-06-03 02:44:00.216598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/infinity.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.152599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/int_mod.py
+-rw-r--r--   0        0        0      450 2023-06-03 02:44:00.204599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/integers.py
+-rw-r--r--   0        0        0      452 2023-06-03 02:44:00.160599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/intersect.py
+-rw-r--r--   0        0        0      450 2023-06-03 02:44:00.096600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/interval.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.096600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/inverse.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.100600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/lambda_mod.py
+-rw-r--r--   0        0        0      452 2023-06-03 02:44:00.156599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/laplacian.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.132599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/lcm.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.144599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/leq.py
+-rw-r--r--   0        0        0      444 2023-06-03 02:44:00.168599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/limit.py
+-rw-r--r--   0        0        0      161 2023-06-03 02:44:00.224598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/linestyle.py
+-rw-r--r--   0        0        0      161 2023-06-03 02:44:02.664565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/list_order.py
+-rw-r--r--   0        0        0      438 2023-06-03 02:44:00.100600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ln.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.100600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/log.py
+-rw-r--r--   0        0        0      438 2023-06-03 02:44:00.140599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/lt.py
+-rw-r--r--   0        0        0      136 2023-06-03 02:44:02.664565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maction_value.py
+-rw-r--r--   0        0        0     2637 2023-06-03 02:44:00.268597 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maligngroup.py
+-rw-r--r--   0        0        0      207 2023-06-03 02:44:02.708564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maligngroup_groupalign.py
+-rw-r--r--   0        0        0      140 2023-06-03 02:44:02.708564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maligngroup_value.py
+-rw-r--r--   0        0        0     2605 2023-06-03 02:44:00.264598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/malignmark.py
+-rw-r--r--   0        0        0      144 2023-06-03 02:44:02.708564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/malignmark_edge.py
+-rw-r--r--   0        0        0      139 2023-06-03 02:44:02.708564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/malignmark_value.py
+-rw-r--r--   0        0        0    74524 2023-06-03 02:44:00.364596 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math.py
+-rw-r--r--   0        0        0      140 2023-06-03 02:44:02.744564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_accent.py
+-rw-r--r--   0        0        0      145 2023-06-03 02:44:02.744564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_accentunder.py
+-rw-r--r--   0        0        0      161 2023-06-03 02:44:02.744564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_align.py
+-rw-r--r--   0        0        0      142 2023-06-03 02:44:02.744564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_bevelled.py
+-rw-r--r--   0        0        0      165 2023-06-03 02:44:02.744564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_charalign.py
+-rw-r--r--   0        0        0      166 2023-06-03 02:44:02.744564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_denomalign.py
+-rw-r--r--   0        0        0      131 2023-06-03 02:44:02.748564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_dir.py
+-rw-r--r--   0        0        0      145 2023-06-03 02:44:02.768564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_display.py
+-rw-r--r--   0        0        0      146 2023-06-03 02:44:02.744564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_displaystyle.py
+-rw-r--r--   0        0        0      138 2023-06-03 02:44:02.748564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_edge.py
+-rw-r--r--   0        0        0      146 2023-06-03 02:44:02.748564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_equalcolumns.py
+-rw-r--r--   0        0        0      143 2023-06-03 02:44:02.748564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_equalrows.py
+-rw-r--r--   0        0        0      139 2023-06-03 02:44:02.748564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_fence.py
+-rw-r--r--   0        0        0      166 2023-06-03 02:44:02.748564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_form.py
+-rw-r--r--   0        0        0      199 2023-06-03 02:44:02.752564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_indentalign.py
+-rw-r--r--   0        0        0      236 2023-06-03 02:44:02.752564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_indentalignfirst.py
+-rw-r--r--   0        0        0      235 2023-06-03 02:44:02.752564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_indentalignlast.py
+-rw-r--r--   0        0        0      185 2023-06-03 02:44:02.744564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_infixlinebreakstyle.py
+-rw-r--r--   0        0        0      141 2023-06-03 02:44:02.752564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_largeop.py
+-rw-r--r--   0        0        0      225 2023-06-03 02:44:02.752564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_linebreak.py
+-rw-r--r--   0        0        0      228 2023-06-03 02:44:02.756564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_linebreakstyle.py
+-rw-r--r--   0        0        0      208 2023-06-03 02:44:02.756564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_location.py
+-rw-r--r--   0        0        0      495 2023-06-03 02:44:02.756564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_longdivstyle.py
+-rw-r--r--   0        0        0      641 2023-06-03 02:44:02.760564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_mathvariant.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.760564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_movablelimits.py
+-rw-r--r--   0        0        0      164 2023-06-03 02:44:02.760564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_numalign.py
+-rw-r--r--   0        0        0      220 2023-06-03 02:44:02.768564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_overflow.py
+-rw-r--r--   0        0        0      143 2023-06-03 02:44:02.760564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_separator.py
+-rw-r--r--   0        0        0      204 2023-06-03 02:44:02.760564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_side.py
+-rw-r--r--   0        0        0      200 2023-06-03 02:44:02.764564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_stackalign.py
+-rw-r--r--   0        0        0      142 2023-06-03 02:44:02.764564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_stretchy.py
+-rw-r--r--   0        0        0      143 2023-06-03 02:44:02.764564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_symmetric.py
+-rw-r--r--   0        0        0      117 2023-06-03 02:44:02.740564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_value.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.196599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/matrix.py
+-rw-r--r--   0        0        0      452 2023-06-03 02:44:00.196599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/matrixrow.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.128600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/max.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.192599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mean.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.192599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/median.py
+-rw-r--r--   0        0        0      137 2023-06-03 02:44:02.680565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/menclose_value.py
+-rw-r--r--   0        0        0      135 2023-06-03 02:44:02.680565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/merror_value.py
+-rw-r--r--   0        0        0      136 2023-06-03 02:44:02.680565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfenced_value.py
+-rw-r--r--   0        0        0      143 2023-06-03 02:44:02.704564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfrac_bevelled.py
+-rw-r--r--   0        0        0      167 2023-06-03 02:44:02.704564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfrac_denomalign.py
+-rw-r--r--   0        0        0      165 2023-06-03 02:44:02.704564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfrac_numalign.py
+-rw-r--r--   0        0        0      120 2023-06-03 02:44:02.704564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfrac_value.py
+-rw-r--r--   0        0        0     5862 2023-06-03 02:44:00.256598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph.py
+-rw-r--r--   0        0        0      151 2023-06-03 02:44:02.660565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_fontstyle.py
+-rw-r--r--   0        0        0      148 2023-06-03 02:44:02.660565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_fontweight.py
+-rw-r--r--   0        0        0      643 2023-06-03 02:44:02.660565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_mathvariant.py
+-rw-r--r--   0        0        0      135 2023-06-03 02:44:02.660565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_value.py
+-rw-r--r--   0        0        0     5329 2023-06-03 02:44:00.228598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi.py
+-rw-r--r--   0        0        0      129 2023-06-03 02:44:02.732564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_dir.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.736564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_fontstyle.py
+-rw-r--r--   0        0        0      144 2023-06-03 02:44:02.732564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_fontweight.py
+-rw-r--r--   0        0        0      639 2023-06-03 02:44:02.732564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_mathvariant.py
+-rw-r--r--   0        0        0      131 2023-06-03 02:44:02.732564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_value.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.132599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/min.py
+-rw-r--r--   0        0        0     1580 2023-06-03 02:44:00.108600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/minus.py
+-rw-r--r--   0        0        0     3231 2023-06-03 02:44:00.276597 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlabeledtr.py
+-rw-r--r--   0        0        0      214 2023-06-03 02:44:02.736564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlabeledtr_rowalign.py
+-rw-r--r--   0        0        0      139 2023-06-03 02:44:02.736564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlabeledtr_value.py
+-rw-r--r--   0        0        0      499 2023-06-03 02:44:02.664565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlongdiv_longdivstyle.py
+-rw-r--r--   0        0        0      137 2023-06-03 02:44:02.664565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlongdiv_value.py
+-rw-r--r--   0        0        0      142 2023-06-03 02:44:02.672565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mmultiscripts_value.py
+-rw-r--r--   0        0        0     5329 2023-06-03 02:44:00.232598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn.py
+-rw-r--r--   0        0        0      129 2023-06-03 02:44:02.732564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_dir.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.732564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_fontstyle.py
+-rw-r--r--   0        0        0      144 2023-06-03 02:44:02.732564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_fontweight.py
+-rw-r--r--   0        0        0      639 2023-06-03 02:44:02.732564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_mathvariant.py
+-rw-r--r--   0        0        0      131 2023-06-03 02:44:02.728564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_value.py
+-rw-r--r--   0        0        0    10043 2023-06-03 02:44:00.240598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo.py
+-rw-r--r--   0        0        0      138 2023-06-03 02:44:02.724564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_accent.py
+-rw-r--r--   0        0        0      129 2023-06-03 02:44:02.720564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_dir.py
+-rw-r--r--   0        0        0      137 2023-06-03 02:44:02.724564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_fence.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.720564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_fontstyle.py
+-rw-r--r--   0        0        0      144 2023-06-03 02:44:02.720564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_fontweight.py
+-rw-r--r--   0        0        0      164 2023-06-03 02:44:02.724564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_form.py
+-rw-r--r--   0        0        0      197 2023-06-03 02:44:02.728564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_indentalign.py
+-rw-r--r--   0        0        0      234 2023-06-03 02:44:02.728564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_indentalignfirst.py
+-rw-r--r--   0        0        0      233 2023-06-03 02:44:02.728564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_indentalignlast.py
+-rw-r--r--   0        0        0      139 2023-06-03 02:44:02.724564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_largeop.py
+-rw-r--r--   0        0        0      223 2023-06-03 02:44:02.728564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_linebreak.py
+-rw-r--r--   0        0        0      226 2023-06-03 02:44:02.728564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_linebreakstyle.py
+-rw-r--r--   0        0        0      639 2023-06-03 02:44:02.720564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_mathvariant.py
+-rw-r--r--   0        0        0      145 2023-06-03 02:44:02.724564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_movablelimits.py
+-rw-r--r--   0        0        0      141 2023-06-03 02:44:02.724564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_separator.py
+-rw-r--r--   0        0        0      140 2023-06-03 02:44:02.724564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_stretchy.py
+-rw-r--r--   0        0        0      141 2023-06-03 02:44:02.724564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_symmetric.py
+-rw-r--r--   0        0        0      125 2023-06-03 02:44:02.720564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_value.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.196599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mode.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.100600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/moment.py
+-rw-r--r--   0        0        0      141 2023-06-03 02:44:02.676565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mover_accent.py
+-rw-r--r--   0        0        0      162 2023-06-03 02:44:02.676565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mover_align.py
+-rw-r--r--   0        0        0      134 2023-06-03 02:44:02.676565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mover_value.py
+-rw-r--r--   0        0        0      136 2023-06-03 02:44:02.680565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mpadded_value.py
+-rw-r--r--   0        0        0      137 2023-06-03 02:44:02.680565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mphantom_value.py
+-rw-r--r--   0        0        0     2432 2023-06-03 02:44:00.264598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mprescripts.py
+-rw-r--r--   0        0        0      140 2023-06-03 02:44:02.736564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mprescripts_value.py
+-rw-r--r--   0        0        0      134 2023-06-03 02:44:02.700564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mroot_value.py
+-rw-r--r--   0        0        0      131 2023-06-03 02:44:02.708564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mrow_dir.py
+-rw-r--r--   0        0        0      133 2023-06-03 02:44:02.704564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mrow_value.py
+-rw-r--r--   0        0        0     5585 2023-06-03 02:44:00.252598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms.py
+-rw-r--r--   0        0        0      129 2023-06-03 02:44:02.712564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_dir.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.712564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_fontstyle.py
+-rw-r--r--   0        0        0      144 2023-06-03 02:44:02.712564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_fontweight.py
+-rw-r--r--   0        0        0      639 2023-06-03 02:44:02.708564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_mathvariant.py
+-rw-r--r--   0        0        0      131 2023-06-03 02:44:02.708564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_value.py
+-rw-r--r--   0        0        0      213 2023-06-03 02:44:02.740564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mscarries_location.py
+-rw-r--r--   0        0        0      292 2023-06-03 02:44:02.740564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mscarries_value.py
+-rw-r--r--   0        0        0      211 2023-06-03 02:44:02.740564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mscarry_location.py
+-rw-r--r--   0        0        0      290 2023-06-03 02:44:02.740564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mscarry_value.py
+-rw-r--r--   0        0        0      136 2023-06-03 02:44:02.740564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msgroup_value.py
+-rw-r--r--   0        0        0     3475 2023-06-03 02:44:00.260598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msline.py
+-rw-r--r--   0        0        0      121 2023-06-03 02:44:02.740564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msline_value.py
+-rw-r--r--   0        0        0     5838 2023-06-03 02:44:00.248598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace.py
+-rw-r--r--   0        0        0      133 2023-06-03 02:44:02.712564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_dir.py
+-rw-r--r--   0        0        0      151 2023-06-03 02:44:02.716564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_fontstyle.py
+-rw-r--r--   0        0        0      148 2023-06-03 02:44:02.716564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_fontweight.py
+-rw-r--r--   0        0        0      269 2023-06-03 02:44:02.716564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_linebreak.py
+-rw-r--r--   0        0        0      643 2023-06-03 02:44:02.712564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_mathvariant.py
+-rw-r--r--   0        0        0      135 2023-06-03 02:44:02.712564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_value.py
+-rw-r--r--   0        0        0      134 2023-06-03 02:44:02.700564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msqrt_value.py
+-rw-r--r--   0        0        0      134 2023-06-03 02:44:02.740564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msrow_value.py
+-rw-r--r--   0        0        0      167 2023-06-03 02:44:02.664565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstack_charalign.py
+-rw-r--r--   0        0        0      202 2023-06-03 02:44:02.664565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstack_stackalign.py
+-rw-r--r--   0        0        0      123 2023-06-03 02:44:02.664565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstack_value.py
+-rw-r--r--   0        0        0      142 2023-06-03 02:44:02.684565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_accent.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.684565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_accentunder.py
+-rw-r--r--   0        0        0      163 2023-06-03 02:44:02.684565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_align.py
+-rw-r--r--   0        0        0      144 2023-06-03 02:44:02.684565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_bevelled.py
+-rw-r--r--   0        0        0      167 2023-06-03 02:44:02.684565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_charalign.py
+-rw-r--r--   0        0        0      168 2023-06-03 02:44:02.684565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_denomalign.py
+-rw-r--r--   0        0        0      133 2023-06-03 02:44:02.688565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_dir.py
+-rw-r--r--   0        0        0      148 2023-06-03 02:44:02.680565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_displaystyle.py
+-rw-r--r--   0        0        0      140 2023-06-03 02:44:02.688565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_edge.py
+-rw-r--r--   0        0        0      148 2023-06-03 02:44:02.688565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_equalcolumns.py
+-rw-r--r--   0        0        0      145 2023-06-03 02:44:02.688565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_equalrows.py
+-rw-r--r--   0        0        0      141 2023-06-03 02:44:02.688565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_fence.py
+-rw-r--r--   0        0        0      151 2023-06-03 02:44:02.700564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_fontstyle.py
+-rw-r--r--   0        0        0      148 2023-06-03 02:44:02.700564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_fontweight.py
+-rw-r--r--   0        0        0      168 2023-06-03 02:44:02.688565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_form.py
+-rw-r--r--   0        0        0      201 2023-06-03 02:44:02.692565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_indentalign.py
+-rw-r--r--   0        0        0      238 2023-06-03 02:44:02.692565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_indentalignfirst.py
+-rw-r--r--   0        0        0      237 2023-06-03 02:44:02.692565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_indentalignlast.py
+-rw-r--r--   0        0        0      187 2023-06-03 02:44:02.684565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_infixlinebreakstyle.py
+-rw-r--r--   0        0        0      143 2023-06-03 02:44:02.692565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_largeop.py
+-rw-r--r--   0        0        0      227 2023-06-03 02:44:02.692565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_linebreak.py
+-rw-r--r--   0        0        0      230 2023-06-03 02:44:02.692565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_linebreakstyle.py
+-rw-r--r--   0        0        0      210 2023-06-03 02:44:02.692565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_location.py
+-rw-r--r--   0        0        0      497 2023-06-03 02:44:02.696565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_longdivstyle.py
+-rw-r--r--   0        0        0      643 2023-06-03 02:44:02.696565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_mathvariant.py
+-rw-r--r--   0        0        0      149 2023-06-03 02:44:02.696565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_movablelimits.py
+-rw-r--r--   0        0        0      166 2023-06-03 02:44:02.696565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_numalign.py
+-rw-r--r--   0        0        0      145 2023-06-03 02:44:02.696565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_separator.py
+-rw-r--r--   0        0        0      206 2023-06-03 02:44:02.700564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_side.py
+-rw-r--r--   0        0        0      202 2023-06-03 02:44:02.700564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_stackalign.py
+-rw-r--r--   0        0        0      144 2023-06-03 02:44:02.700564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_stretchy.py
+-rw-r--r--   0        0        0      145 2023-06-03 02:44:02.700564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_symmetric.py
+-rw-r--r--   0        0        0      135 2023-06-03 02:44:02.680565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_value.py
+-rw-r--r--   0        0        0      133 2023-06-03 02:44:02.680565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msub_value.py
+-rw-r--r--   0        0        0      136 2023-06-03 02:44:02.676565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msubsup_value.py
+-rw-r--r--   0        0        0      133 2023-06-03 02:44:02.676565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msup_value.py
+-rw-r--r--   0        0        0     6510 2023-06-03 02:44:00.272597 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable.py
+-rw-r--r--   0        0        0      148 2023-06-03 02:44:02.668565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_displaystyle.py
+-rw-r--r--   0        0        0      148 2023-06-03 02:44:02.668565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_equalcolumns.py
+-rw-r--r--   0        0        0      145 2023-06-03 02:44:02.668565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_equalrows.py
+-rw-r--r--   0        0        0      206 2023-06-03 02:44:02.668565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_side.py
+-rw-r--r--   0        0        0      141 2023-06-03 02:44:02.668565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_value.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.280597 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtd.py
+-rw-r--r--   0        0        0     5386 2023-06-03 02:44:00.244598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext.py
+-rw-r--r--   0        0        0      132 2023-06-03 02:44:02.716564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_dir.py
+-rw-r--r--   0        0        0      150 2023-06-03 02:44:02.716564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_fontstyle.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.716564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_fontweight.py
+-rw-r--r--   0        0        0      642 2023-06-03 02:44:02.716564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_mathvariant.py
+-rw-r--r--   0        0        0      134 2023-06-03 02:44:02.716564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_value.py
+-rw-r--r--   0        0        0     3175 2023-06-03 02:44:00.280597 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtr.py
+-rw-r--r--   0        0        0      207 2023-06-03 02:44:02.672565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtr_rowalign.py
+-rw-r--r--   0        0        0      132 2023-06-03 02:44:02.668565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtr_value.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.676565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munder_accentunder.py
+-rw-r--r--   0        0        0      163 2023-06-03 02:44:02.676565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munder_align.py
+-rw-r--r--   0        0        0      135 2023-06-03 02:44:02.676565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munder_value.py
+-rw-r--r--   0        0        0      146 2023-06-03 02:44:02.672565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munderover_accent.py
+-rw-r--r--   0        0        0      151 2023-06-03 02:44:02.672565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munderover_accentunder.py
+-rw-r--r--   0        0        0      167 2023-06-03 02:44:02.672565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munderover_align.py
+-rw-r--r--   0        0        0      139 2023-06-03 02:44:02.672565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munderover_value.py
+-rw-r--r--   0        0        0      462 2023-06-03 02:44:00.204599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/naturalnumbers.py
+-rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.144599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/neq.py
+-rw-r--r--   0        0        0     2401 2023-06-03 02:44:00.260598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/none.py
+-rw-r--r--   0        0        0      133 2023-06-03 02:44:02.736564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/none_value.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.136599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/not_mod.py
+-rw-r--r--   0        0        0      454 2023-06-03 02:44:00.212598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/notanumber.py
+-rw-r--r--   0        0        0      444 2023-06-03 02:44:00.160599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/notin.py
+-rw-r--r--   0        0        0      456 2023-06-03 02:44:00.164599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/notprsubset.py
+-rw-r--r--   0        0        0      452 2023-06-03 02:44:00.164599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/notsubset.py
+-rw-r--r--   0        0        0      438 2023-06-03 02:44:00.136599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/or_mod.py
+-rw-r--r--   0        0        0      458 2023-06-03 02:44:00.204599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/outerproduct.py
+-rw-r--r--   0        0        0      456 2023-06-03 02:44:00.156599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/partialdiff.py
+-rw-r--r--   0        0        0      438 2023-06-03 02:44:00.216598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/pi.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.132599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/plus.py
+-rw-r--r--   0        0        0     1580 2023-06-03 02:44:00.108600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/power.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.208598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/primes.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.168599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/product.py
+-rw-r--r--   0        0        0      450 2023-06-03 02:44:00.164599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/prsubset.py
+-rw-r--r--   0        0        0     1586 2023-06-03 02:44:00.104600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/quotient.py
+-rw-r--r--   0        0        0      452 2023-06-03 02:44:00.204599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/rationals.py
+-rw-r--r--   0        0        0     1578 2023-06-03 02:44:00.124600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/real.py
+-rw-r--r--   0        0        0      444 2023-06-03 02:44:00.204599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/reals.py
+-rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.112600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/rem.py
+-rw-r--r--   0        0        0     1578 2023-06-03 02:44:00.112600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/root.py
+-rw-r--r--   0        0        0      460 2023-06-03 02:44:00.200599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/scalarproduct.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.192599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sdev.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sec.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.180599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sech.py
+-rw-r--r--   0        0        0      450 2023-06-03 02:44:00.200599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/selector.py
+-rw-r--r--   0        0        0      215 2023-06-03 02:44:00.092600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sep.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.164599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/setdiff.py
+-rw-r--r--   0        0        0     1405 2023-06-03 02:44:00.088600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/share.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sin.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.176599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sinh.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.164599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/subset.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.168599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sum.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/tan.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.176599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/tanh.py
+-rw-r--r--   0        0        0     1710 2023-06-03 02:44:00.152599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/tendsto.py
+-rw-r--r--   0        0        0      444 2023-06-03 02:44:00.132599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/times.py
+-rw-r--r--   0        0        0      452 2023-06-03 02:44:00.200599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/transpose.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.212598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/true.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.160599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/union.py
+-rw-r--r--   0        0        0      450 2023-06-03 02:44:00.192599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/variance.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.196599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/vector.py
+-rw-r--r--   0        0        0      460 2023-06-03 02:44:00.200599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/vectorproduct.py
+-rw-r--r--   0        0        0      209 2023-06-03 02:44:00.224598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/verticalalign.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.136599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/xor.py
+-rw-r--r--   0        0        0       15 2023-06-03 02:17:59.961981 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/__init__.py
+-rw-r--r--   0        0        0      488 2023-06-03 02:43:58.316624 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/__init__.py
+-rw-r--r--   0        0        0      188 2023-06-03 02:44:02.660565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/actuate_value.py
+-rw-r--r--   0        0        0     1893 2023-06-03 02:43:58.428623 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/arc_type.py
+-rw-r--r--   0        0        0     1169 2023-06-03 02:43:58.420623 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/extended.py
+-rw-r--r--   0        0        0     1453 2023-06-03 02:43:58.428623 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/locator_type.py
+-rw-r--r--   0        0        0     1244 2023-06-03 02:43:58.424623 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/resource_type.py
+-rw-r--r--   0        0        0      193 2023-06-03 02:44:02.660565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/show_value.py
+-rw-r--r--   0        0        0     1940 2023-06-03 02:43:58.416623 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/simple.py
+-rw-r--r--   0        0        0     1203 2023-06-03 02:43:58.424623 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/title_elt_type.py
+-rw-r--r--   0        0        0      247 2023-06-03 02:44:02.660565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/type_value.py
+-rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/xml/__init__.py
+-rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/xml/pkg_1998/__init__.py
+-rw-r--r--   0        0        0      120 2023-06-03 02:43:58.380623 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/xml/pkg_1998/namespace/__init__.py
+-rw-r--r--   0        0        0      118 2023-06-03 02:44:02.656565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/xml/pkg_1998/namespace/lang_value.py
+-rw-r--r--   0        0        0      154 2023-06-03 02:44:02.656565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/xml/pkg_1998/namespace/space_value.py
+-rw-r--r--   0        0        0      997 2023-06-03 02:44:02.632565 pubmed_types-0.1.2/src/pubmed_types/models/other_abstract.py
+-rw-r--r--   0        0        0      223 2023-06-03 02:44:02.844563 pubmed_types-0.1.2/src/pubmed_types/models/other_abstract_type.py
+-rw-r--r--   0        0        0      518 2023-06-03 02:44:02.632565 pubmed_types-0.1.2/src/pubmed_types/models/other_id.py
+-rw-r--r--   0        0        0      257 2023-06-03 02:44:02.840563 pubmed_types-0.1.2/src/pubmed_types/models/other_id_source.py
+-rw-r--r--   0        0        0      863 2023-06-03 02:44:02.312570 pubmed_types-0.1.2/src/pubmed_types/models/overline_end.py
+-rw-r--r--   0        0        0      747 2023-06-03 02:44:02.312570 pubmed_types-0.1.2/src/pubmed_types/models/overline_start.py
+-rw-r--r--   0        0        0       82 2023-06-03 02:44:02.772564 pubmed_types-0.1.2/src/pubmed_types/models/overline_toggle.py
+-rw-r--r--   0        0        0      692 2023-06-03 02:44:02.316570 pubmed_types-0.1.2/src/pubmed_types/models/page_count.py
+-rw-r--r--   0        0        0     1349 2023-06-03 02:44:02.320570 pubmed_types-0.1.2/src/pubmed_types/models/page_range.py
+-rw-r--r--   0        0        0      649 2023-06-03 02:44:02.636565 pubmed_types-0.1.2/src/pubmed_types/models/pagination.py
+-rw-r--r--   0        0        0     1147 2023-06-03 02:44:02.636565 pubmed_types-0.1.2/src/pubmed_types/models/param.py
+-rw-r--r--   0        0        0      831 2023-06-03 02:44:02.640565 pubmed_types-0.1.2/src/pubmed_types/models/personal_name_subject.py
+-rw-r--r--   0        0        0      426 2023-06-03 02:44:02.640565 pubmed_types-0.1.2/src/pubmed_types/models/personal_name_subject_list.py
+-rw-r--r--   0        0        0      461 2023-06-03 02:44:02.632565 pubmed_types-0.1.2/src/pubmed_types/models/pmid.py
+-rw-r--r--   0        0        0     1366 2023-06-03 02:44:02.320570 pubmed_types-0.1.2/src/pubmed_types/models/postal_code.py
+-rw-r--r--   0        0        0      112 2023-06-03 02:44:02.796563 pubmed_types-0.1.2/src/pubmed_types/models/preformat_orientation.py
+-rw-r--r--   0        0        0      149 2023-06-03 02:44:02.796563 pubmed_types-0.1.2/src/pubmed_types/models/preformat_position.py
+-rw-r--r--   0        0        0     2142 2023-06-03 02:44:02.324570 pubmed_types-0.1.2/src/pubmed_types/models/principal_award_recipient.py
+-rw-r--r--   0        0        0     1855 2023-06-03 02:44:02.328570 pubmed_types-0.1.2/src/pubmed_types/models/principal_investigator.py
+-rw-r--r--   0        0        0     2483 2023-06-03 02:44:02.332569 pubmed_types-0.1.2/src/pubmed_types/models/processing_meta.py
+-rw-r--r--   0        0        0      148 2023-06-03 02:44:02.824563 pubmed_types-0.1.2/src/pubmed_types/models/processing_meta_base_tagset.py
+-rw-r--r--   0        0        0      109 2023-06-03 02:44:02.824563 pubmed_types-0.1.2/src/pubmed_types/models/processing_meta_mathml_version.py
+-rw-r--r--   0        0        0      138 2023-06-03 02:44:02.824563 pubmed_types-0.1.2/src/pubmed_types/models/processing_meta_table_model.py
+-rw-r--r--   0        0        0      116 2023-06-03 02:44:02.828563 pubmed_types-0.1.2/src/pubmed_types/models/processing_meta_tagset_family.py
+-rw-r--r--   0        0        0      936 2023-06-03 02:44:02.912562 pubmed_types-0.1.2/src/pubmed_types/models/pub_date_1.py
+-rw-r--r--   0        0        0     2895 2023-06-03 02:44:02.916561 pubmed_types-0.1.2/src/pubmed_types/models/pub_date_2.py
+-rw-r--r--   0        0        0      740 2023-06-03 02:44:02.332569 pubmed_types-0.1.2/src/pubmed_types/models/pub_date_not_available.py
+-rw-r--r--   0        0        0      408 2023-06-03 02:18:04.041925 pubmed_types-0.1.2/src/pubmed_types/models/pub_date_pub_status.py
+-rw-r--r--   0        0        0      708 2023-06-03 02:44:02.336569 pubmed_types-0.1.2/src/pubmed_types/models/pub_history.py
+-rw-r--r--   0        0        0     2871 2023-06-03 02:44:02.340569 pubmed_types-0.1.2/src/pubmed_types/models/pub_id.py
+-rw-r--r--   0        0        0     1462 2023-06-03 02:44:02.644565 pubmed_types-0.1.2/src/pubmed_types/models/pub_med_pub_date.py
+-rw-r--r--   0        0        0      496 2023-06-03 02:44:02.848563 pubmed_types-0.1.2/src/pubmed_types/models/pub_med_pub_date_pub_status.py
+-rw-r--r--   0        0        0      423 2023-06-03 02:44:02.640565 pubmed_types-0.1.2/src/pubmed_types/models/publication_type.py
+-rw-r--r--   0        0        0      400 2023-06-03 02:44:02.640565 pubmed_types-0.1.2/src/pubmed_types/models/publication_type_list.py
+-rw-r--r--   0        0        0     1192 2023-06-03 02:18:03.561932 pubmed_types-0.1.2/src/pubmed_types/models/publisher.py
+-rw-r--r--   0        0        0      606 2023-06-03 02:44:02.920561 pubmed_types-0.1.2/src/pubmed_types/models/publisher_1.py
+-rw-r--r--   0        0        0     1193 2023-06-03 02:44:02.920561 pubmed_types-0.1.2/src/pubmed_types/models/publisher_2.py
+-rw-r--r--   0        0        0     1013 2023-06-03 02:44:02.924561 pubmed_types-0.1.2/src/pubmed_types/models/publisher_name_1.py
+-rw-r--r--   0        0        0      600 2023-06-03 02:44:02.556566 pubmed_types-0.1.2/src/pubmed_types/models/pubmed_article.py
+-rw-r--r--   0        0        0      839 2023-06-03 02:44:02.552566 pubmed_types-0.1.2/src/pubmed_types/models/pubmed_article_set.py
+-rw-r--r--   0        0        0      611 2023-06-03 02:44:02.556566 pubmed_types-0.1.2/src/pubmed_types/models/pubmed_book_article.py
+-rw-r--r--   0        0        0      384 2023-06-03 02:44:02.556566 pubmed_types-0.1.2/src/pubmed_types/models/pubmed_book_article_set.py
+-rw-r--r--   0        0        0      991 2023-06-03 02:44:02.572566 pubmed_types-0.1.2/src/pubmed_types/models/pubmed_book_data.py
+-rw-r--r--   0        0        0     1217 2023-06-03 02:44:02.572566 pubmed_types-0.1.2/src/pubmed_types/models/pubmed_data.py
+-rw-r--r--   0        0        0      724 2023-06-03 02:44:02.644565 pubmed_types-0.1.2/src/pubmed_types/models/qualifier_name.py
+-rw-r--r--   0        0        0       87 2023-06-03 02:44:02.840563 pubmed_types-0.1.2/src/pubmed_types/models/qualifier_name_major_topic_yn.py
+-rw-r--r--   0        0        0      268 2023-06-03 02:44:02.800563 pubmed_types-0.1.2/src/pubmed_types/models/question_question_response_type.py
+-rw-r--r--   0        0        0      695 2023-06-03 02:44:02.344569 pubmed_types-0.1.2/src/pubmed_types/models/ref_count.py
+-rw-r--r--   0        0        0      576 2023-06-03 02:44:02.644565 pubmed_types-0.1.2/src/pubmed_types/models/reference.py
+-rw-r--r--   0        0        0      678 2023-06-03 02:44:02.644565 pubmed_types-0.1.2/src/pubmed_types/models/reference_list.py
+-rw-r--r--   0        0        0      460 2023-06-03 02:18:03.773929 pubmed_types-0.1.2/src/pubmed_types/models/replaces.py
+-rw-r--r--   0        0        0      192 2023-06-03 02:18:04.045925 pubmed_types-0.1.2/src/pubmed_types/models/replaces_id_type.py
+-rw-r--r--   0        0        0     1440 2023-06-03 02:44:02.348569 pubmed_types-0.1.2/src/pubmed_types/models/resource_group.py
+-rw-r--r--   0        0        0     2014 2023-06-03 02:44:02.348569 pubmed_types-0.1.2/src/pubmed_types/models/resource_id.py
+-rw-r--r--   0        0        0     4999 2023-06-03 02:44:02.356569 pubmed_types-0.1.2/src/pubmed_types/models/resource_name.py
+-rw-r--r--   0        0        0     1009 2023-06-03 02:44:02.360569 pubmed_types-0.1.2/src/pubmed_types/models/resource_wrap.py
+-rw-r--r--   0        0        0     2223 2023-06-03 02:44:02.364569 pubmed_types-0.1.2/src/pubmed_types/models/response.py
+-rw-r--r--   0        0        0     3137 2023-06-03 02:44:02.368569 pubmed_types-0.1.2/src/pubmed_types/models/restricted_by.py
+-rw-r--r--   0        0        0       79 2023-06-03 02:44:02.772564 pubmed_types-0.1.2/src/pubmed_types/models/roman_toggle.py
+-rw-r--r--   0        0        0      728 2023-06-03 02:44:02.368569 pubmed_types-0.1.2/src/pubmed_types/models/rp.py
+-rw-r--r--   0        0        0     1346 2023-06-03 02:44:02.372569 pubmed_types-0.1.2/src/pubmed_types/models/rt.py
+-rw-r--r--   0        0        0       83 2023-06-03 02:44:02.772564 pubmed_types-0.1.2/src/pubmed_types/models/sans_serif_toggle.py
+-rw-r--r--   0        0        0       76 2023-06-03 02:44:02.776564 pubmed_types-0.1.2/src/pubmed_types/models/sc_toggle.py
+-rw-r--r--   0        0        0     1337 2023-06-03 02:44:02.376569 pubmed_types-0.1.2/src/pubmed_types/models/season.py
+-rw-r--r--   0        0        0      765 2023-06-03 02:44:02.648565 pubmed_types-0.1.2/src/pubmed_types/models/section.py
+-rw-r--r--   0        0        0     1341 2023-06-03 02:44:02.648565 pubmed_types-0.1.2/src/pubmed_types/models/section_title.py
+-rw-r--r--   0        0        0      347 2023-06-03 02:44:02.648565 pubmed_types-0.1.2/src/pubmed_types/models/sections.py
+-rw-r--r--   0        0        0     9015 2023-06-03 02:44:02.388569 pubmed_types-0.1.2/src/pubmed_types/models/self_uri.py
+-rw-r--r--   0        0        0     7416 2023-06-03 02:44:02.400569 pubmed_types-0.1.2/src/pubmed_types/models/series_text.py
+-rw-r--r--   0        0        0     7394 2023-06-03 02:44:02.412568 pubmed_types-0.1.2/src/pubmed_types/models/series_title.py
+-rw-r--r--   0        0        0     7912 2023-06-03 02:44:02.424568 pubmed_types-0.1.2/src/pubmed_types/models/sig.py
+-rw-r--r--   0        0        0     8403 2023-06-03 02:44:02.440568 pubmed_types-0.1.2/src/pubmed_types/models/sig_block.py
+-rw-r--r--   0        0        0     1361 2023-06-03 02:44:02.444568 pubmed_types-0.1.2/src/pubmed_types/models/state.py
+-rw-r--r--   0        0        0       80 2023-06-03 02:44:02.776564 pubmed_types-0.1.2/src/pubmed_types/models/strike_toggle.py
+-rw-r--r--   0        0        0     8497 2023-06-03 02:44:02.460568 pubmed_types-0.1.2/src/pubmed_types/models/string_conf.py
+-rw-r--r--   0        0        0      159 2023-06-03 02:44:02.784563 pubmed_types-0.1.2/src/pubmed_types/models/string_name_name_style.py
+-rw-r--r--   0        0        0       87 2023-06-03 02:44:02.780563 pubmed_types-0.1.2/src/pubmed_types/models/styled_content_toggle.py
+-rw-r--r--   0        0        0      993 2023-06-03 02:44:02.924561 pubmed_types-0.1.2/src/pubmed_types/models/sub_1.py
+-rw-r--r--   0        0        0       92 2023-06-03 02:44:02.780563 pubmed_types-0.1.2/src/pubmed_types/models/sub_arrange.py
+-rw-r--r--   0        0        0     2576 2023-06-03 02:44:02.468568 pubmed_types-0.1.2/src/pubmed_types/models/sub_article.py
+-rw-r--r--   0        0        0      999 2023-06-03 02:44:02.924561 pubmed_types-0.1.2/src/pubmed_types/models/suffix_1.py
+-rw-r--r--   0        0        0      993 2023-06-03 02:44:02.928561 pubmed_types-0.1.2/src/pubmed_types/models/sup_1.py
+-rw-r--r--   0        0        0       92 2023-06-03 02:44:02.780563 pubmed_types-0.1.2/src/pubmed_types/models/sup_arrange.py
+-rw-r--r--   0        0        0      386 2023-06-03 02:44:02.648565 pubmed_types-0.1.2/src/pubmed_types/models/suppl_mesh_list.py
+-rw-r--r--   0        0        0      668 2023-06-03 02:44:02.652565 pubmed_types-0.1.2/src/pubmed_types/models/suppl_mesh_name.py
+-rw-r--r--   0        0        0      185 2023-06-03 02:44:02.836563 pubmed_types-0.1.2/src/pubmed_types/models/suppl_mesh_name_type.py
+-rw-r--r--   0        0        0      124 2023-06-03 02:44:02.800563 pubmed_types-0.1.2/src/pubmed_types/models/supplementary_material_orientation.py
+-rw-r--r--   0        0        0      161 2023-06-03 02:44:02.800563 pubmed_types-0.1.2/src/pubmed_types/models/supplementary_material_position.py
+-rw-r--r--   0        0        0     1316 2023-06-03 02:44:02.472568 pubmed_types-0.1.2/src/pubmed_types/models/support_description.py
+-rw-r--r--   0        0        0     1500 2023-06-03 02:44:02.476568 pubmed_types-0.1.2/src/pubmed_types/models/support_group.py
+-rw-r--r--   0        0        0     9397 2023-06-03 02:44:02.500567 pubmed_types-0.1.2/src/pubmed_types/models/support_source.py
+-rw-r--r--   0        0        0      695 2023-06-03 02:44:02.500567 pubmed_types-0.1.2/src/pubmed_types/models/table_count.py
+-rw-r--r--   0        0        0      220 2023-06-03 02:44:02.804563 pubmed_types-0.1.2/src/pubmed_types/models/table_frame.py
+-rw-r--r--   0        0        0      140 2023-06-03 02:44:02.804563 pubmed_types-0.1.2/src/pubmed_types/models/table_rules.py
+-rw-r--r--   0        0        0      117 2023-06-03 02:44:02.820563 pubmed_types-0.1.2/src/pubmed_types/models/table_wrap_group_orientation.py
+-rw-r--r--   0        0        0      154 2023-06-03 02:44:02.820563 pubmed_types-0.1.2/src/pubmed_types/models/table_wrap_group_position.py
+-rw-r--r--   0        0        0      112 2023-06-03 02:44:02.800563 pubmed_types-0.1.2/src/pubmed_types/models/table_wrap_orientation.py
+-rw-r--r--   0        0        0      149 2023-06-03 02:44:02.800563 pubmed_types-0.1.2/src/pubmed_types/models/table_wrap_position.py
+-rw-r--r--   0        0        0      150 2023-06-03 02:44:02.816563 pubmed_types-0.1.2/src/pubmed_types/models/tbody_align.py
+-rw-r--r--   0        0        0      135 2023-06-03 02:44:02.820563 pubmed_types-0.1.2/src/pubmed_types/models/tbody_valign.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.812563 pubmed_types-0.1.2/src/pubmed_types/models/td_align.py
+-rw-r--r--   0        0        0      129 2023-06-03 02:44:02.812563 pubmed_types-0.1.2/src/pubmed_types/models/td_scope.py
+-rw-r--r--   0        0        0      132 2023-06-03 02:44:02.816563 pubmed_types-0.1.2/src/pubmed_types/models/td_valign.py
+-rw-r--r--   0        0        0     1386 2023-06-03 02:44:02.504567 pubmed_types-0.1.2/src/pubmed_types/models/tex_math.py
+-rw-r--r--   0        0        0      128 2023-06-03 02:44:02.780563 pubmed_types-0.1.2/src/pubmed_types/models/tex_math_notation.py
+-rw-r--r--   0        0        0      150 2023-06-03 02:44:02.816563 pubmed_types-0.1.2/src/pubmed_types/models/tfoot_align.py
+-rw-r--r--   0        0        0      135 2023-06-03 02:44:02.816563 pubmed_types-0.1.2/src/pubmed_types/models/tfoot_valign.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.812563 pubmed_types-0.1.2/src/pubmed_types/models/th_align.py
+-rw-r--r--   0        0        0      129 2023-06-03 02:44:02.812563 pubmed_types-0.1.2/src/pubmed_types/models/th_scope.py
+-rw-r--r--   0        0        0      132 2023-06-03 02:44:02.812563 pubmed_types-0.1.2/src/pubmed_types/models/th_valign.py
+-rw-r--r--   0        0        0      150 2023-06-03 02:44:02.808563 pubmed_types-0.1.2/src/pubmed_types/models/thead_align.py
+-rw-r--r--   0        0        0      135 2023-06-03 02:44:02.808563 pubmed_types-0.1.2/src/pubmed_types/models/thead_valign.py
+-rw-r--r--   0        0        0     1542 2023-06-03 02:44:02.508567 pubmed_types-0.1.2/src/pubmed_types/models/title_group.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.808563 pubmed_types-0.1.2/src/pubmed_types/models/tr_align.py
+-rw-r--r--   0        0        0      132 2023-06-03 02:44:02.808563 pubmed_types-0.1.2/src/pubmed_types/models/tr_valign.py
+-rw-r--r--   0        0        0     8912 2023-06-03 02:44:02.520567 pubmed_types-0.1.2/src/pubmed_types/models/trans_abstract.py
+-rw-r--r--   0        0        0     7376 2023-06-03 02:44:02.532567 pubmed_types-0.1.2/src/pubmed_types/models/trans_subtitle.py
+-rw-r--r--   0        0        0     1641 2023-06-03 02:44:02.536567 pubmed_types-0.1.2/src/pubmed_types/models/trans_title_group.py
+-rw-r--r--   0        0        0     2610 2023-06-03 02:44:02.584566 pubmed_types-0.1.2/src/pubmed_types/models/u.py
+-rw-r--r--   0        0        0      866 2023-06-03 02:44:02.536567 pubmed_types-0.1.2/src/pubmed_types/models/underline_end.py
+-rw-r--r--   0        0        0      750 2023-06-03 02:44:02.540567 pubmed_types-0.1.2/src/pubmed_types/models/underline_start.py
+-rw-r--r--   0        0        0       83 2023-06-03 02:44:02.776564 pubmed_types-0.1.2/src/pubmed_types/models/underline_toggle.py
+-rw-r--r--   0        0        0      614 2023-06-03 02:44:02.652565 pubmed_types-0.1.2/src/pubmed_types/models/url.py
+-rw-r--r--   0        0        0      661 2023-06-03 02:44:02.856562 pubmed_types-0.1.2/src/pubmed_types/models/url_lang.py
+-rw-r--r--   0        0        0      150 2023-06-03 02:44:02.856562 pubmed_types-0.1.2/src/pubmed_types/models/url_type.py
+-rw-r--r--   0        0        0     1072 2023-06-03 02:44:02.656565 pubmed_types-0.1.2/src/pubmed_types/models/vernacular_title.py
+-rw-r--r--   0        0        0     2893 2023-06-03 02:44:02.544567 pubmed_types-0.1.2/src/pubmed_types/models/volume_issue_group.py
+-rw-r--r--   0        0        0      962 2023-06-03 02:44:02.656565 pubmed_types-0.1.2/src/pubmed_types/models/volume_title.py
+-rw-r--r--   0        0        0      692 2023-06-03 02:44:02.548566 pubmed_types-0.1.2/src/pubmed_types/models/word_count.py
+-rw-r--r--   0        0        0      330 2023-06-03 02:44:02.656565 pubmed_types-0.1.2/src/pubmed_types/models/xs_pattern.py
+-rw-r--r--   0        0        0     1627 2023-06-03 02:44:02.552566 pubmed_types-0.1.2/src/pubmed_types/models/year.py
+-rw-r--r--   0        0        0     5511 1970-01-01 00:00:00.000000 pubmed_types-0.1.2/PKG-INFO
```

### Comparing `pubmed_types-0.1.1/LICENSE` & `pubmed_types-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/README.md` & `pubmed_types-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,246 +1,273 @@
 00000000: 2320 7075 626d 6564 2d74 7970 6573 2028  # pubmed-types (
-00000010: 7630 2e31 2e31 290a 0a23 2320 496e 7472  v0.1.1)..## Intr
-00000020: 6f64 7563 7469 6f6e 0a0a 4120 636f 6d70  oduction..A comp
-00000030: 6c65 7465 2069 6d70 6c65 6d65 6e74 6174  lete implementat
-00000040: 696f 6e20 6f66 2074 6865 2058 4d4c 2073  ion of the XML s
-00000050: 6368 656d 6120 666f 7220 504d 4320 4f70  chema for PMC Op
-00000060: 656e 2041 6363 6573 7320 6172 7469 636c  en Access articl
-00000070: 6573 2061 6e64 2050 7562 6d65 640a 6172  es and Pubmed.ar
-00000080: 7469 636c 6520 7365 7473 2028 6369 7461  ticle sets (cita
-00000090: 7469 6f6e 7329 2e0a 0a54 6869 7320 7061  tions)...This pa
-000000a0: 636b 6167 6520 6865 6c70 7320 746f 2070  ckage helps to p
-000000b0: 6172 7365 2050 7562 4d65 6420 584d 4c20  arse PubMed XML 
-000000c0: 6461 7461 2069 6e74 6f20 5079 6461 6e74  data into Pydant
-000000d0: 6963 206d 6f64 656c 732e 2054 6869 7320  ic models. This 
-000000e0: 7661 6c69 6461 7465 7320 7468 650a 696e  validates the.in
-000000f0: 7075 7420 786d 6c20 6461 7461 2061 6e64  put xml data and
-00000100: 2070 726f 7669 6465 7320 7479 7065 6869   provides typehi
-00000110: 6e74 7320 666f 7220 776f 726b 696e 6720  nts for working 
-00000120: 7769 7468 2074 6865 2063 6f6d 706c 6578  with the complex
-00000130: 2058 4d4c 2073 7472 7563 7475 7265 730a   XML structures.
-00000140: 7072 6573 656e 7420 696e 2050 7562 4d65  present in PubMe
-00000150: 6420 6461 7461 2e0a 0a23 2320 5768 7920  d data...## Why 
-00000160: 646f 2049 206e 6565 6420 7468 6973 3f0a  do I need this?.
-00000170: 0a50 7562 4d65 6420 6b65 6570 7320 7472  .PubMed keeps tr
-00000180: 6163 6b20 6f66 2031 3073 206f 6620 6d69  ack of 10s of mi
-00000190: 6c6c 696f 6e73 206f 6620 7265 7365 6172  llions of resear
-000001a0: 6368 2064 6174 612c 2061 6e64 2061 2063  ch data, and a c
-000001b0: 6f6d 706c 6578 2058 4d4c 2073 7472 7563  omplex XML struc
-000001c0: 7475 7265 2069 730a 7573 6564 2074 6f20  ture is.used to 
-000001d0: 7374 6f72 6520 6974 2e20 5061 7273 696e  store it. Parsin
-000001e0: 6720 584d 4c20 6f6e 2069 7473 206f 776e  g XML on its own
-000001f0: 2069 7320 6368 616c 6c65 6e67 696e 6720   is challenging 
-00000200: 656e 6f75 6768 2e20 4164 6420 746f 2069  enough. Add to i
-00000210: 7420 7468 6520 6665 6174 7572 650a 7269  t the feature.ri
-00000220: 6368 2064 6174 6120 696e 7369 6465 206f  ch data inside o
-00000230: 6620 6561 6368 2063 6974 6174 696f 6e2c  f each citation,
-00000240: 2061 6e64 2079 6f75 2077 696c 6c20 6669   and you will fi
-00000250: 6e64 2079 6f75 7273 656c 6620 7769 7468  nd yourself with
-00000260: 2068 6f75 7273 206f 7220 6461 7973 206f   hours or days o
-00000270: 660a 6e61 7669 6761 7469 6e67 2074 6865  f.navigating the
-00000280: 2058 4d4c 2073 7472 7563 7475 7265 2e0a   XML structure..
-00000290: 0a54 6865 2061 7070 726f 6163 6820 6865  .The approach he
-000002a0: 7265 2077 6173 2074 6f20 6175 746f 6765  re was to autoge
-000002b0: 6e65 7261 7465 2050 7964 616e 7469 6320  nerate Pydantic 
-000002c0: 636c 6173 7365 7320 746f 2070 6172 7365  classes to parse
-000002d0: 2074 6865 2058 4d4c 2075 7369 6e67 2074   the XML using t
-000002e0: 6865 0a60 7873 6461 7461 2d70 7964 616e  he.`xsdata-pydan
-000002f0: 7469 6360 2074 6f6f 6c2e 2054 6869 7320  tic` tool. This 
-00000300: 6170 7072 6f61 6368 2068 6173 2074 6865  approach has the
-00000310: 2062 656e 6566 6974 206f 6620 6d61 6b69   benefit of maki
-00000320: 6e67 2073 7572 6520 6576 6572 7920 7069  ng sure every pi
-00000330: 6563 6520 6f66 2064 6174 610a 6973 2070  ece of data.is p
-00000340: 6172 7365 6420 7072 6f70 6572 6c79 2c20  arsed properly, 
-00000350: 616e 6420 616e 2065 7272 6f72 2069 7320  and an error is 
-00000360: 7468 726f 776e 2069 7320 736f 6d65 7468  thrown is someth
-00000370: 696e 6720 6973 206d 6973 7369 6e67 206f  ing is missing o
-00000380: 7220 696e 636f 7272 6563 742e 2049 6e73  r incorrect. Ins
-00000390: 7465 6164 0a6f 6620 7573 696e 6720 6469  tead.of using di
-000003a0: 6374 696f 6e61 7269 6573 2074 6f20 686f  ctionaries to ho
-000003b0: 6c64 2074 6865 2064 6174 612c 2050 7964  ld the data, Pyd
-000003c0: 616e 7469 6320 636c 6173 7365 7320 6861  antic classes ha
-000003d0: 7665 2074 6865 2062 656e 6566 6974 206f  ve the benefit o
-000003e0: 6620 7072 6f76 6964 696e 670a 7479 7065  f providing.type
-000003f0: 2068 696e 7473 2077 6974 6820 7461 6220   hints with tab 
-00000400: 636f 6d70 6c65 7469 6f6e 2066 6f72 2049  completion for I
-00000410: 4445 732c 206d 616b 696e 6720 6974 2065  DEs, making it e
-00000420: 6173 6965 7220 746f 206e 6176 6967 6174  asier to navigat
-00000430: 6520 7468 6520 636f 6d70 6c65 780a 7374  e the complex.st
-00000440: 7275 6374 7572 6520 6f66 2074 6865 2063  ructure of the c
-00000450: 6974 6174 696f 6e20 6461 7461 2e0a 0a23  itation data...#
-00000460: 2320 486f 7720 646f 2049 2075 7365 2069  # How do I use i
-00000470: 743f 0a0a 4974 2069 7320 706f 7373 6962  t?..It is possib
-00000480: 6c65 2074 6f20 7573 6520 6078 7364 6174  le to use `xsdat
-00000490: 612d 7079 6461 6e74 6963 6020 616e 6420  a-pydantic` and 
-000004a0: 7468 6520 6175 746f 6765 6e65 7261 7465  the autogenerate
-000004b0: 6420 636c 6173 7365 7320 6469 7265 6374  d classes direct
-000004c0: 6c79 2074 6f20 7061 7273 650a 616e 2058  ly to parse.an X
-000004d0: 4d4c 2066 696c 652c 2062 7574 2077 6520  ML file, but we 
-000004e0: 7072 6f76 6964 6520 6120 636f 6e76 656e  provide a conven
-000004f0: 6965 6e63 6520 6675 6e63 7469 6f6e 2074  ience function t
-00000500: 6f20 6561 7369 6c79 206f 7065 6e20 5075  o easily open Pu
-00000510: 624d 6564 2058 4d6c 2063 6974 6174 696f  bMed XMl citatio
-00000520: 6e73 0a61 6e64 2050 4d43 206f 7065 6e20  ns.and PMC open 
-00000530: 6163 6365 7373 2061 7274 6963 6c65 732e  access articles.
-00000540: 0a0a 2323 2320 4578 616d 706c 6520 313a  ..### Example 1:
-00000550: 2041 2050 4d43 204f 7065 6e20 4163 6365   A PMC Open Acce
-00000560: 7373 2041 7274 6963 6c65 0a0a 6060 6070  ss Article..```p
-00000570: 7974 686f 6e0a 696d 706f 7274 2074 6172  ython.import tar
-00000580: 6669 6c65 0a69 6d70 6f72 7420 7572 6c6c  file.import urll
-00000590: 6962 2e72 6571 7565 7374 2061 7320 7265  ib.request as re
-000005a0: 7175 6573 740a 6672 6f6d 2063 6f6e 7465  quest.from conte
-000005b0: 7874 6c69 6220 696d 706f 7274 2063 6c6f  xtlib import clo
-000005c0: 7369 6e67 0a66 726f 6d20 7061 7468 6c69  sing.from pathli
-000005d0: 6220 696d 706f 7274 2050 6174 680a 0a66  b import Path..f
-000005e0: 726f 6d20 7075 626d 6564 5f74 7970 6573  rom pubmed_types
-000005f0: 2069 6d70 6f72 7420 7061 7273 655f 7075   import parse_pu
-00000600: 626d 6564 5f78 6d6c 0a0a 2320 496e 7075  bmed_xml..# Inpu
-00000610: 7420 6669 6c65 2073 6f75 7263 6520 616e  t file source an
-00000620: 6420 6f75 7470 7574 2066 696c 6520 6465  d output file de
-00000630: 7374 696e 6174 696f 6e0a 736f 7572 6365  stination.source
-00000640: 203d 2028 0a20 2020 2022 6674 703a 2f2f   = (.    "ftp://
-00000650: 6674 702e 6e63 6269 2e6e 6c6d 2e6e 6968  ftp.ncbi.nlm.nih
-00000660: 2e67 6f76 220a 2020 2020 2b20 222f 7075  .gov".    + "/pu
-00000670: 622f 706d 632f 6f61 5f62 756c 6b2f 6f61  b/pmc/oa_bulk/oa
-00000680: 5f63 6f6d 6d2f 786d 6c22 0a20 2020 202b  _comm/xml".    +
-00000690: 2022 2f6f 615f 636f 6d6d 5f78 6d6c 2e69   "/oa_comm_xml.i
-000006a0: 6e63 722e 3230 3233 2d30 332d 3231 2e74  ncr.2023-03-21.t
-000006b0: 6172 2e67 7a22 0a29 0a64 6573 7469 6e61  ar.gz".).destina
-000006c0: 7469 6f6e 203d 2050 6174 6828 2264 6f77  tion = Path("dow
-000006d0: 6e6c 6f61 6473 2229 0a64 6573 7469 6e61  nloads").destina
-000006e0: 7469 6f6e 2e6d 6b64 6972 2865 7869 7374  tion.mkdir(exist
-000006f0: 5f6f 6b3d 5472 7565 290a 0a23 2031 2e20  _ok=True)..# 1. 
-00000700: 4765 7420 616e 206f 7065 6e20 6163 6365  Get an open acce
-00000710: 7373 2061 7274 6963 6c65 2064 6174 6173  ss article datas
-00000720: 6574 2066 726f 6d20 7468 6520 4654 5020  et from the FTP 
-00000730: 7365 7276 6572 0a77 6974 6820 636c 6f73  server.with clos
-00000740: 696e 6728 7265 7175 6573 742e 7572 6c6f  ing(request.urlo
-00000750: 7065 6e28 736f 7572 6365 2929 2061 7320  pen(source)) as 
-00000760: 7572 6c3a 0a20 2020 2077 6974 6820 7461  url:.    with ta
-00000770: 7266 696c 652e 6f70 656e 2866 696c 656f  rfile.open(fileo
-00000780: 626a 3d75 726c 2c20 6d6f 6465 3d22 723a  bj=url, mode="r:
-00000790: 677a 2229 2061 7320 6672 3a0a 2020 2020  gz") as fr:.    
-000007a0: 2020 2020 6672 2e65 7874 7261 6374 616c      fr.extractal
-000007b0: 6c28 6465 7374 696e 6174 696f 6e29 0a0a  l(destination)..
-000007c0: 2320 322e 2050 6172 7365 2074 6865 2066  # 2. Parse the f
-000007d0: 696c 650a 6669 6c65 5f70 6174 6820 3d20  ile.file_path = 
-000007e0: 6465 7374 696e 6174 696f 6e2e 6a6f 696e  destination.join
-000007f0: 7061 7468 2822 504d 4330 3039 7878 7878  path("PMC009xxxx
-00000800: 7878 2229 2e6a 6f69 6e70 6174 6828 2250  xx").joinpath("P
-00000810: 4d43 3939 3730 3636 322e 786d 6c22 290a  MC9970662.xml").
-00000820: 6675 6c6c 5f74 6578 7420 3d20 7061 7273  full_text = pars
-00000830: 655f 7075 626d 6564 5f78 6d6c 2866 696c  e_pubmed_xml(fil
-00000840: 655f 7061 7468 290a 0a23 2033 2e20 5072  e_path)..# 3. Pr
-00000850: 696e 7420 6f75 7420 7468 6520 6172 7469  int out the arti
-00000860: 636c 6520 7469 746c 650a 7072 696e 7428  cle title.print(
-00000870: 6622 5469 746c 653a 207b 6675 6c6c 5f74  f"Title: {full_t
-00000880: 6578 742e 6672 6f6e 742e 6172 7469 636c  ext.front.articl
-00000890: 655f 6d65 7461 2e74 6974 6c65 5f67 726f  e_meta.title_gro
-000008a0: 7570 2e61 7274 6963 6c65 5f74 6974 6c65  up.article_title
-000008b0: 2e63 6f6e 7465 6e74 5b30 5d7d 2229 0a60  .content[0]}").`
-000008c0: 6060 0a0a 4f75 7470 7574 3a0a 0a60 6060  ``..Output:..```
-000008d0: 6261 7368 0a54 6974 6c65 3a20 4c61 6374  bash.Title: Lact
-000008e0: 6174 6520 6173 2061 206d 796f 6b69 6e65  ate as a myokine
-000008f0: 2061 6e64 2065 7865 726b 696e 653a 2064   and exerkine: d
-00000900: 7269 7665 7273 2061 6e64 2073 6967 6e61  rivers and signa
-00000910: 6c73 206f 6620 7068 7973 696f 6c6f 6779  ls of physiology
-00000920: 2061 6e64 206d 6574 6162 6f6c 6973 6d0a   and metabolism.
-00000930: 6060 600a 0a23 2323 2045 7861 6d70 6c65  ```..### Example
-00000940: 2032 3a20 4120 5075 626d 6564 2062 6173   2: A Pubmed bas
-00000950: 656c 696e 6520 6369 7461 7469 6f6e 2066  eline citation f
-00000960: 696c 650a 0a23 2323 2045 7861 6d70 6c65  ile..### Example
-00000970: 2031 3a20 4120 504d 4320 4f70 656e 2041   1: A PMC Open A
-00000980: 6363 6573 7320 4172 7469 636c 650a 0a60  ccess Article..`
-00000990: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
-000009a0: 677a 6970 0a69 6d70 6f72 7420 7572 6c6c  gzip.import urll
-000009b0: 6962 2e72 6571 7565 7374 2061 7320 7265  ib.request as re
-000009c0: 7175 6573 740a 6672 6f6d 2063 6f6e 7465  quest.from conte
-000009d0: 7874 6c69 6220 696d 706f 7274 2063 6c6f  xtlib import clo
-000009e0: 7369 6e67 0a66 726f 6d20 7061 7468 6c69  sing.from pathli
-000009f0: 6220 696d 706f 7274 2050 6174 680a 0a66  b import Path..f
-00000a00: 726f 6d20 7075 626d 6564 5f74 7970 6573  rom pubmed_types
-00000a10: 2069 6d70 6f72 7420 7061 7273 655f 7075   import parse_pu
-00000a20: 626d 6564 5f78 6d6c 2c20 5075 626d 6564  bmed_xml, Pubmed
-00000a30: 4172 7469 636c 6553 6574 0a0a 2320 496e  ArticleSet..# In
-00000a40: 7075 7420 6669 6c65 2073 6f75 7263 6520  put file source 
-00000a50: 616e 6420 6f75 7470 7574 2066 696c 6520  and output file 
-00000a60: 6465 7374 696e 6174 696f 6e0a 736f 7572  destination.sour
-00000a70: 6365 203d 2022 6674 703a 2f2f 6674 702e  ce = "ftp://ftp.
-00000a80: 6e63 6269 2e6e 6c6d 2e6e 6968 2e67 6f76  ncbi.nlm.nih.gov
-00000a90: 2220 2b20 222f 7075 626d 6564 2f75 7064  " + "/pubmed/upd
-00000aa0: 6174 6566 696c 6573 2220 2b20 222f 7075  atefiles" + "/pu
-00000ab0: 626d 6564 3233 6e31 3136 382e 786d 6c2e  bmed23n1168.xml.
-00000ac0: 677a 220a 6465 7374 696e 6174 696f 6e20  gz".destination 
-00000ad0: 3d20 5061 7468 2822 646f 776e 6c6f 6164  = Path("download
-00000ae0: 7322 292e 6a6f 696e 7061 7468 2822 7075  s").joinpath("pu
-00000af0: 626d 6564 3233 6e31 3136 382e 786d 6c22  bmed23n1168.xml"
-00000b00: 290a 6465 7374 696e 6174 696f 6e2e 7061  ).destination.pa
-00000b10: 7265 6e74 2e6d 6b64 6972 2865 7869 7374  rent.mkdir(exist
-00000b20: 5f6f 6b3d 5472 7565 290a 0a23 2031 2e20  _ok=True)..# 1. 
-00000b30: 4765 7420 6120 7075 626d 6564 2063 6974  Get a pubmed cit
-00000b40: 6174 696f 6e20 6461 696c 7920 7570 6461  ation daily upda
-00000b50: 7465 2066 696c 6520 6672 6f6d 2074 6865  te file from the
-00000b60: 2046 5450 2073 6572 7665 720a 7769 7468   FTP server.with
-00000b70: 2063 6c6f 7369 6e67 2872 6571 7565 7374   closing(request
-00000b80: 2e75 726c 6f70 656e 2873 6f75 7263 6529  .urlopen(source)
-00000b90: 2920 6173 2075 726c 3a0a 2020 2020 7769  ) as url:.    wi
-00000ba0: 7468 2067 7a69 702e 477a 6970 4669 6c65  th gzip.GzipFile
-00000bb0: 2866 696c 656f 626a 3d75 726c 2c20 6d6f  (fileobj=url, mo
-00000bc0: 6465 3d22 7262 2229 2061 7320 6672 3a0a  de="rb") as fr:.
-00000bd0: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
-00000be0: 6e28 6465 7374 696e 6174 696f 6e2c 206d  n(destination, m
-00000bf0: 6f64 653d 2277 6222 2920 6173 2066 773a  ode="wb") as fw:
-00000c00: 0a20 2020 2020 2020 2020 2020 2066 772e  .            fw.
-00000c10: 7772 6974 6528 6672 2e72 6561 6428 2929  write(fr.read())
-00000c20: 0a0a 2320 322e 2050 6172 7365 2074 6865  ..# 2. Parse the
-00000c30: 2066 696c 650a 6172 7469 636c 655f 7365   file.article_se
-00000c40: 7420 3d20 7061 7273 655f 7075 626d 6564  t = parse_pubmed
-00000c50: 5f78 6d6c 2864 6573 7469 6e61 7469 6f6e  _xml(destination
-00000c60: 290a 6173 7365 7274 2069 7369 6e73 7461  ).assert isinsta
-00000c70: 6e63 6528 6172 7469 636c 655f 7365 742c  nce(article_set,
-00000c80: 2050 7562 6d65 6441 7274 6963 6c65 5365   PubmedArticleSe
-00000c90: 7429 0a0a 2320 332e 2047 6574 2074 6865  t)..# 3. Get the
-00000ca0: 206e 756d 6265 7220 6f66 2063 6974 6174   number of citat
-00000cb0: 696f 6e73 2069 6e20 7468 6520 6669 6c65  ions in the file
-00000cc0: 0a70 7269 6e74 2866 224e 756d 6265 7220  .print(f"Number 
-00000cd0: 6f66 2063 6974 6174 696f 6e73 3a20 7b6c  of citations: {l
-00000ce0: 656e 2861 7274 6963 6c65 5f73 6574 2e70  en(article_set.p
-00000cf0: 7562 6d65 645f 6172 7469 636c 6529 7d22  ubmed_article)}"
-00000d00: 290a 7072 696e 7428 6622 7b61 7274 6963  ).print(f"{artic
-00000d10: 6c65 5f73 6574 2e70 7562 6d65 645f 6172  le_set.pubmed_ar
-00000d20: 7469 636c 655b 305d 2e6d 6564 6c69 6e65  ticle[0].medline
-00000d30: 5f63 6974 6174 696f 6e2e 6172 7469 636c  _citation.articl
-00000d40: 652e 6172 7469 636c 655f 7469 746c 652e  e.article_title.
-00000d50: 636f 6e74 656e 745b 305d 7d22 290a 6060  content[0]}").``
-00000d60: 600a 0a4f 7574 7075 743a 0a0a 6060 6062  `..Output:..```b
-00000d70: 6173 680a 4e75 6d62 6572 206f 6620 6369  ash.Number of ci
-00000d80: 7461 7469 6f6e 733a 2032 3534 330a 4120  tations: 2543.A 
-00000d90: 5061 7465 6e74 2061 6e64 2050 6174 7465  Patent and Patte
-00000da0: 726e 204d 6f74 6865 722e 0a60 6060 0a0a  rn Mother..```..
-00000db0: 2323 2046 4151 0a0a 2323 2320 5768 7920  ## FAQ..### Why 
-00000dc0: 646f 6573 2069 7420 7461 6b65 2073 6f20  does it take so 
-00000dd0: 6c6f 6e67 2074 6f20 7061 7273 6520 6120  long to parse a 
-00000de0: 7075 626d 6564 2063 6974 6174 696f 6e20  pubmed citation 
-00000df0: 7365 740a 0a54 6865 7265 2069 7320 6120  set..There is a 
-00000e00: 6c6f 7420 6f66 2064 6174 612c 2061 6e64  lot of data, and
-00000e10: 2074 6865 2073 6368 656d 6120 6973 2064   the schema is d
-00000e20: 6565 7020 616e 6420 636f 6d70 6c65 782e  eep and complex.
-00000e30: 0a0a 2323 2320 5768 7920 6172 6520 7468  ..### Why are th
-00000e40: 6520 7265 7475 726e 2073 7472 7563 7475  e return structu
-00000e50: 7265 7320 736f 2063 6f6d 706c 6963 6174  res so complicat
-00000e60: 6564 3f0a 0a54 6865 2072 6574 7572 6e20  ed?..The return 
-00000e70: 7374 7275 6374 7572 6573 2061 7265 2061  structures are a
-00000e80: 2064 6972 6563 7420 7265 666c 6563 7469   direct reflecti
-00000e90: 6f6e 206f 6620 7468 6520 584d 4c20 666f  on of the XML fo
-00000ea0: 726d 6174 2064 6566 696e 6564 2062 7920  rmat defined by 
-00000eb0: 7468 6520 4e4c 4d2e 2049 6e0a 7468 6520  the NLM. In.the 
-00000ec0: 6675 7475 7265 2073 6f6d 6520 7574 696c  future some util
-00000ed0: 6974 7920 636c 6173 7365 7320 6d69 6768  ity classes migh
-00000ee0: 7420 6265 206d 6164 6520 666f 7220 636f  t be made for co
-00000ef0: 6d6d 6f6e 2063 6f6d 706f 6e65 6e74 7320  mmon components 
-00000f00: 2874 6974 6c65 2c20 6175 7468 6f72 732c  (title, authors,
-00000f10: 0a65 7463 292c 2062 7574 2066 6f72 206e  .etc), but for n
-00000f20: 6f77 2074 6869 7320 6973 2069 6e74 656e  ow this is inten
-00000f30: 6465 6420 746f 2062 6520 616e 2075 6e62  ded to be an unb
-00000f40: 6961 7365 6420 7761 7920 6f66 2070 6172  iased way of par
-00000f50: 7369 6e67 2074 6865 2058 4d4c 2e0a       sing the XML..
+00000010: 7630 2e31 2e32 290a 0a3c 7020 616c 6967  v0.1.2)..<p alig
+00000020: 6e3d 2263 656e 7465 7222 3e0a 2020 2020  n="center">.    
+00000030: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000040: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000050: 2f70 7970 692f 646d 2f70 7562 6d65 642d  /pypi/dm/pubmed-
+00000060: 7479 7065 733f 7374 796c 653d 666c 6174  types?style=flat
+00000070: 2d73 7175 6172 6522 202f 3e0a 2020 2020  -square" />.    
+00000080: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000090: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000000a0: 2f70 7970 692f 6c2f 7075 626d 6564 2d74  /pypi/l/pubmed-t
+000000b0: 7970 6573 3f73 7479 6c65 3d66 6c61 742d  ypes?style=flat-
+000000c0: 7371 7561 7265 222f 3e0a 2020 2020 3c69  square"/>.    <i
+000000d0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+000000e0: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+000000f0: 7970 692f 762f 7075 626d 6564 2d74 7970  ypi/v/pubmed-typ
+00000100: 6573 3f73 7479 6c65 3d66 6c61 742d 7371  es?style=flat-sq
+00000110: 7561 7265 222f 3e0a 2020 2020 3c61 2068  uare"/>.    <a h
+00000120: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00000130: 6875 622e 636f 6d2f 7465 6672 612f 7873  hub.com/tefra/xs
+00000140: 6461 7461 2d70 7964 616e 7469 6322 3e3c  data-pydantic"><
+00000150: 696d 6720 616c 743d 2242 7569 6c74 2077  img alt="Built w
+00000160: 6974 683a 2078 7364 6174 612d 7079 6461  ith: xsdata-pyda
+00000170: 6e74 6963 2220 7372 633d 2268 7474 7073  ntic" src="https
+00000180: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000190: 6f2f 6261 6467 652f 636f 6465 2532 3073  o/badge/code%20s
+000001a0: 7479 6c65 2d62 6c61 636b 2d30 3030 3030  tyle-black-00000
+000001b0: 302e 7376 6722 3e3c 2f61 3e0a 3c2f 703e  0.svg"></a>.</p>
+000001c0: 0a0a 2323 2049 6e74 726f 6475 6374 696f  ..## Introductio
+000001d0: 6e0a 0a41 2063 6f6d 706c 6574 6520 696d  n..A complete im
+000001e0: 706c 656d 656e 7461 7469 6f6e 206f 6620  plementation of 
+000001f0: 7468 6520 584d 4c20 7363 6865 6d61 2066  the XML schema f
+00000200: 6f72 2050 4d43 204f 7065 6e20 4163 6365  or PMC Open Acce
+00000210: 7373 2061 7274 6963 6c65 7320 616e 6420  ss articles and 
+00000220: 5075 626d 6564 0a61 7274 6963 6c65 2073  Pubmed.article s
+00000230: 6574 7320 2863 6974 6174 696f 6e73 292e  ets (citations).
+00000240: 0a0a 5468 6973 2070 6163 6b61 6765 2068  ..This package h
+00000250: 656c 7073 2074 6f20 7061 7273 6520 5075  elps to parse Pu
+00000260: 624d 6564 2058 4d4c 2064 6174 6120 696e  bMed XML data in
+00000270: 746f 2050 7964 616e 7469 6320 6d6f 6465  to Pydantic mode
+00000280: 6c73 2e20 5468 6973 2076 616c 6964 6174  ls. This validat
+00000290: 6573 2074 6865 0a69 6e70 7574 2078 6d6c  es the.input xml
+000002a0: 2064 6174 6120 616e 6420 7072 6f76 6964   data and provid
+000002b0: 6573 2074 7970 6568 696e 7473 2066 6f72  es typehints for
+000002c0: 2077 6f72 6b69 6e67 2077 6974 6820 7468   working with th
+000002d0: 6520 636f 6d70 6c65 7820 584d 4c20 7374  e complex XML st
+000002e0: 7275 6374 7572 6573 0a70 7265 7365 6e74  ructures.present
+000002f0: 2069 6e20 5075 624d 6564 2064 6174 612e   in PubMed data.
+00000300: 0a0a 2323 2057 6879 2064 6f20 4920 6e65  ..## Why do I ne
+00000310: 6564 2074 6869 733f 0a0a 5075 624d 6564  ed this?..PubMed
+00000320: 206b 6565 7073 2074 7261 636b 206f 6620   keeps track of 
+00000330: 3130 7320 6f66 206d 696c 6c69 6f6e 7320  10s of millions 
+00000340: 6f66 2072 6573 6561 7263 6820 6461 7461  of research data
+00000350: 2c20 616e 6420 6120 636f 6d70 6c65 7820  , and a complex 
+00000360: 584d 4c20 7374 7275 6374 7572 6520 6973  XML structure is
+00000370: 0a75 7365 6420 746f 2073 746f 7265 2069  .used to store i
+00000380: 742e 2050 6172 7369 6e67 2058 4d4c 206f  t. Parsing XML o
+00000390: 6e20 6974 7320 6f77 6e20 6973 2063 6861  n its own is cha
+000003a0: 6c6c 656e 6769 6e67 2065 6e6f 7567 682e  llenging enough.
+000003b0: 2041 6464 2074 6f20 6974 2074 6865 2066   Add to it the f
+000003c0: 6561 7475 7265 0a72 6963 6820 6461 7461  eature.rich data
+000003d0: 2069 6e73 6964 6520 6f66 2065 6163 6820   inside of each 
+000003e0: 6369 7461 7469 6f6e 2c20 616e 6420 796f  citation, and yo
+000003f0: 7520 7769 6c6c 2066 696e 6420 796f 7572  u will find your
+00000400: 7365 6c66 2077 6974 6820 686f 7572 7320  self with hours 
+00000410: 6f72 2064 6179 7320 6f66 0a6e 6176 6967  or days of.navig
+00000420: 6174 696e 6720 7468 6520 584d 4c20 7374  ating the XML st
+00000430: 7275 6374 7572 652e 0a0a 5468 6520 6170  ructure...The ap
+00000440: 7072 6f61 6368 2068 6572 6520 7761 7320  proach here was 
+00000450: 746f 2061 7574 6f67 656e 6572 6174 6520  to autogenerate 
+00000460: 5079 6461 6e74 6963 2063 6c61 7373 6573  Pydantic classes
+00000470: 2074 6f20 7061 7273 6520 7468 6520 584d   to parse the XM
+00000480: 4c20 7573 696e 6720 7468 650a 6078 7364  L using the.`xsd
+00000490: 6174 612d 7079 6461 6e74 6963 6020 746f  ata-pydantic` to
+000004a0: 6f6c 2e20 5468 6973 2061 7070 726f 6163  ol. This approac
+000004b0: 6820 6861 7320 7468 6520 6265 6e65 6669  h has the benefi
+000004c0: 7420 6f66 206d 616b 696e 6720 7375 7265  t of making sure
+000004d0: 2065 7665 7279 2070 6965 6365 206f 6620   every piece of 
+000004e0: 6461 7461 0a69 7320 7061 7273 6564 2070  data.is parsed p
+000004f0: 726f 7065 726c 792c 2061 6e64 2061 6e20  roperly, and an 
+00000500: 6572 726f 7220 6973 2074 6872 6f77 6e20  error is thrown 
+00000510: 6973 2073 6f6d 6574 6869 6e67 2069 7320  is something is 
+00000520: 6d69 7373 696e 6720 6f72 2069 6e63 6f72  missing or incor
+00000530: 7265 6374 2e20 496e 7374 6561 640a 6f66  rect. Instead.of
+00000540: 2075 7369 6e67 2064 6963 7469 6f6e 6172   using dictionar
+00000550: 6965 7320 746f 2068 6f6c 6420 7468 6520  ies to hold the 
+00000560: 6461 7461 2c20 5079 6461 6e74 6963 2063  data, Pydantic c
+00000570: 6c61 7373 6573 2068 6176 6520 7468 6520  lasses have the 
+00000580: 6265 6e65 6669 7420 6f66 2070 726f 7669  benefit of provi
+00000590: 6469 6e67 0a74 7970 6520 6869 6e74 7320  ding.type hints 
+000005a0: 7769 7468 2074 6162 2063 6f6d 706c 6574  with tab complet
+000005b0: 696f 6e20 666f 7220 4944 4573 2c20 6d61  ion for IDEs, ma
+000005c0: 6b69 6e67 2069 7420 6561 7369 6572 2074  king it easier t
+000005d0: 6f20 6e61 7669 6761 7465 2074 6865 2063  o navigate the c
+000005e0: 6f6d 706c 6578 0a73 7472 7563 7475 7265  omplex.structure
+000005f0: 206f 6620 7468 6520 6369 7461 7469 6f6e   of the citation
+00000600: 2064 6174 612e 0a0a 2323 2048 6f77 2064   data...## How d
+00000610: 6f20 4920 7573 6520 6974 3f0a 0a49 7420  o I use it?..It 
+00000620: 6973 2070 6f73 7369 626c 6520 746f 2075  is possible to u
+00000630: 7365 2060 7873 6461 7461 2d70 7964 616e  se `xsdata-pydan
+00000640: 7469 6360 2061 6e64 2074 6865 2061 7574  tic` and the aut
+00000650: 6f67 656e 6572 6174 6564 2063 6c61 7373  ogenerated class
+00000660: 6573 2064 6972 6563 746c 7920 746f 2070  es directly to p
+00000670: 6172 7365 0a61 6e20 584d 4c20 6669 6c65  arse.an XML file
+00000680: 2c20 6275 7420 7765 2070 726f 7669 6465  , but we provide
+00000690: 2061 2063 6f6e 7665 6e69 656e 6365 2066   a convenience f
+000006a0: 756e 6374 696f 6e20 746f 2065 6173 696c  unction to easil
+000006b0: 7920 6f70 656e 2050 7562 4d65 6420 584d  y open PubMed XM
+000006c0: 6c20 6369 7461 7469 6f6e 730a 616e 6420  l citations.and 
+000006d0: 504d 4320 6f70 656e 2061 6363 6573 7320  PMC open access 
+000006e0: 6172 7469 636c 6573 2e0a 0a23 2323 2045  articles...### E
+000006f0: 7861 6d70 6c65 2031 3a20 4120 504d 4320  xample 1: A PMC 
+00000700: 4f70 656e 2041 6363 6573 7320 4172 7469  Open Access Arti
+00000710: 636c 650a 0a60 6060 7079 7468 6f6e 0a69  cle..```python.i
+00000720: 6d70 6f72 7420 7461 7266 696c 650a 696d  mport tarfile.im
+00000730: 706f 7274 2075 726c 6c69 622e 7265 7175  port urllib.requ
+00000740: 6573 7420 6173 2072 6571 7565 7374 0a66  est as request.f
+00000750: 726f 6d20 636f 6e74 6578 746c 6962 2069  rom contextlib i
+00000760: 6d70 6f72 7420 636c 6f73 696e 670a 6672  mport closing.fr
+00000770: 6f6d 2070 6174 686c 6962 2069 6d70 6f72  om pathlib impor
+00000780: 7420 5061 7468 0a0a 6672 6f6d 2070 7562  t Path..from pub
+00000790: 6d65 645f 7479 7065 7320 696d 706f 7274  med_types import
+000007a0: 2070 6172 7365 5f70 7562 6d65 645f 786d   parse_pubmed_xm
+000007b0: 6c0a 0a23 2049 6e70 7574 2066 696c 6520  l..# Input file 
+000007c0: 736f 7572 6365 2061 6e64 206f 7574 7075  source and outpu
+000007d0: 7420 6669 6c65 2064 6573 7469 6e61 7469  t file destinati
+000007e0: 6f6e 0a73 6f75 7263 6520 3d20 280a 2020  on.source = (.  
+000007f0: 2020 2266 7470 3a2f 2f66 7470 2e6e 6362    "ftp://ftp.ncb
+00000800: 692e 6e6c 6d2e 6e69 682e 676f 7622 0a20  i.nlm.nih.gov". 
+00000810: 2020 202b 2022 2f70 7562 2f70 6d63 2f6f     + "/pub/pmc/o
+00000820: 615f 6275 6c6b 2f6f 615f 636f 6d6d 2f78  a_bulk/oa_comm/x
+00000830: 6d6c 220a 2020 2020 2b20 222f 6f61 5f63  ml".    + "/oa_c
+00000840: 6f6d 6d5f 786d 6c2e 696e 6372 2e32 3032  omm_xml.incr.202
+00000850: 332d 3033 2d32 312e 7461 722e 677a 220a  3-03-21.tar.gz".
+00000860: 290a 6465 7374 696e 6174 696f 6e20 3d20  ).destination = 
+00000870: 5061 7468 2822 646f 776e 6c6f 6164 7322  Path("downloads"
+00000880: 290a 6465 7374 696e 6174 696f 6e2e 6d6b  ).destination.mk
+00000890: 6469 7228 6578 6973 745f 6f6b 3d54 7275  dir(exist_ok=Tru
+000008a0: 6529 0a0a 2320 312e 2047 6574 2061 6e20  e)..# 1. Get an 
+000008b0: 6f70 656e 2061 6363 6573 7320 6172 7469  open access arti
+000008c0: 636c 6520 6461 7461 7365 7420 6672 6f6d  cle dataset from
+000008d0: 2074 6865 2046 5450 2073 6572 7665 720a   the FTP server.
+000008e0: 7769 7468 2063 6c6f 7369 6e67 2872 6571  with closing(req
+000008f0: 7565 7374 2e75 726c 6f70 656e 2873 6f75  uest.urlopen(sou
+00000900: 7263 6529 2920 6173 2075 726c 3a0a 2020  rce)) as url:.  
+00000910: 2020 7769 7468 2074 6172 6669 6c65 2e6f    with tarfile.o
+00000920: 7065 6e28 6669 6c65 6f62 6a3d 7572 6c2c  pen(fileobj=url,
+00000930: 206d 6f64 653d 2272 3a67 7a22 2920 6173   mode="r:gz") as
+00000940: 2066 723a 0a20 2020 2020 2020 2066 722e   fr:.        fr.
+00000950: 6578 7472 6163 7461 6c6c 2864 6573 7469  extractall(desti
+00000960: 6e61 7469 6f6e 290a 0a23 2032 2e20 5061  nation)..# 2. Pa
+00000970: 7273 6520 7468 6520 6669 6c65 0a66 696c  rse the file.fil
+00000980: 655f 7061 7468 203d 2064 6573 7469 6e61  e_path = destina
+00000990: 7469 6f6e 2e6a 6f69 6e70 6174 6828 2250  tion.joinpath("P
+000009a0: 4d43 3030 3978 7878 7878 7822 292e 6a6f  MC009xxxxxx").jo
+000009b0: 696e 7061 7468 2822 504d 4339 3937 3036  inpath("PMC99706
+000009c0: 3632 2e78 6d6c 2229 0a66 756c 6c5f 7465  62.xml").full_te
+000009d0: 7874 203d 2070 6172 7365 5f70 7562 6d65  xt = parse_pubme
+000009e0: 645f 786d 6c28 6669 6c65 5f70 6174 6829  d_xml(file_path)
+000009f0: 0a0a 2320 332e 2050 7269 6e74 206f 7574  ..# 3. Print out
+00000a00: 2074 6865 2061 7274 6963 6c65 2074 6974   the article tit
+00000a10: 6c65 0a70 7269 6e74 2866 2254 6974 6c65  le.print(f"Title
+00000a20: 3a20 7b66 756c 6c5f 7465 7874 2e66 726f  : {full_text.fro
+00000a30: 6e74 2e61 7274 6963 6c65 5f6d 6574 612e  nt.article_meta.
+00000a40: 7469 746c 655f 6772 6f75 702e 6172 7469  title_group.arti
+00000a50: 636c 655f 7469 746c 652e 636f 6e74 656e  cle_title.conten
+00000a60: 745b 305d 7d22 290a 6060 600a 0a4f 7574  t[0]}").```..Out
+00000a70: 7075 743a 0a0a 6060 6062 6173 680a 5469  put:..```bash.Ti
+00000a80: 746c 653a 204c 6163 7461 7465 2061 7320  tle: Lactate as 
+00000a90: 6120 6d79 6f6b 696e 6520 616e 6420 6578  a myokine and ex
+00000aa0: 6572 6b69 6e65 3a20 6472 6976 6572 7320  erkine: drivers 
+00000ab0: 616e 6420 7369 676e 616c 7320 6f66 2070  and signals of p
+00000ac0: 6879 7369 6f6c 6f67 7920 616e 6420 6d65  hysiology and me
+00000ad0: 7461 626f 6c69 736d 0a60 6060 0a0a 2323  tabolism.```..##
+00000ae0: 2320 4578 616d 706c 6520 323a 2041 2050  # Example 2: A P
+00000af0: 7562 6d65 6420 6261 7365 6c69 6e65 2063  ubmed baseline c
+00000b00: 6974 6174 696f 6e20 6669 6c65 0a0a 2323  itation file..##
+00000b10: 2320 4578 616d 706c 6520 313a 2041 2050  # Example 1: A P
+00000b20: 4d43 204f 7065 6e20 4163 6365 7373 2041  MC Open Access A
+00000b30: 7274 6963 6c65 0a0a 6060 6070 7974 686f  rticle..```pytho
+00000b40: 6e0a 696d 706f 7274 2067 7a69 700a 696d  n.import gzip.im
+00000b50: 706f 7274 2075 726c 6c69 622e 7265 7175  port urllib.requ
+00000b60: 6573 7420 6173 2072 6571 7565 7374 0a66  est as request.f
+00000b70: 726f 6d20 636f 6e74 6578 746c 6962 2069  rom contextlib i
+00000b80: 6d70 6f72 7420 636c 6f73 696e 670a 6672  mport closing.fr
+00000b90: 6f6d 2070 6174 686c 6962 2069 6d70 6f72  om pathlib impor
+00000ba0: 7420 5061 7468 0a0a 6672 6f6d 2070 7562  t Path..from pub
+00000bb0: 6d65 645f 7479 7065 7320 696d 706f 7274  med_types import
+00000bc0: 2070 6172 7365 5f70 7562 6d65 645f 786d   parse_pubmed_xm
+00000bd0: 6c2c 2050 7562 6d65 6441 7274 6963 6c65  l, PubmedArticle
+00000be0: 5365 740a 0a23 2049 6e70 7574 2066 696c  Set..# Input fil
+00000bf0: 6520 736f 7572 6365 2061 6e64 206f 7574  e source and out
+00000c00: 7075 7420 6669 6c65 2064 6573 7469 6e61  put file destina
+00000c10: 7469 6f6e 0a73 6f75 7263 6520 3d20 2266  tion.source = "f
+00000c20: 7470 3a2f 2f66 7470 2e6e 6362 692e 6e6c  tp://ftp.ncbi.nl
+00000c30: 6d2e 6e69 682e 676f 7622 202b 2022 2f70  m.nih.gov" + "/p
+00000c40: 7562 6d65 642f 7570 6461 7465 6669 6c65  ubmed/updatefile
+00000c50: 7322 202b 2022 2f70 7562 6d65 6432 336e  s" + "/pubmed23n
+00000c60: 3131 3638 2e78 6d6c 2e67 7a22 0a64 6573  1168.xml.gz".des
+00000c70: 7469 6e61 7469 6f6e 203d 2050 6174 6828  tination = Path(
+00000c80: 2264 6f77 6e6c 6f61 6473 2229 2e6a 6f69  "downloads").joi
+00000c90: 6e70 6174 6828 2270 7562 6d65 6432 336e  npath("pubmed23n
+00000ca0: 3131 3638 2e78 6d6c 2229 0a64 6573 7469  1168.xml").desti
+00000cb0: 6e61 7469 6f6e 2e70 6172 656e 742e 6d6b  nation.parent.mk
+00000cc0: 6469 7228 6578 6973 745f 6f6b 3d54 7275  dir(exist_ok=Tru
+00000cd0: 6529 0a0a 2320 312e 2047 6574 2061 2070  e)..# 1. Get a p
+00000ce0: 7562 6d65 6420 6369 7461 7469 6f6e 2064  ubmed citation d
+00000cf0: 6169 6c79 2075 7064 6174 6520 6669 6c65  aily update file
+00000d00: 2066 726f 6d20 7468 6520 4654 5020 7365   from the FTP se
+00000d10: 7276 6572 0a77 6974 6820 636c 6f73 696e  rver.with closin
+00000d20: 6728 7265 7175 6573 742e 7572 6c6f 7065  g(request.urlope
+00000d30: 6e28 736f 7572 6365 2929 2061 7320 7572  n(source)) as ur
+00000d40: 6c3a 0a20 2020 2077 6974 6820 677a 6970  l:.    with gzip
+00000d50: 2e47 7a69 7046 696c 6528 6669 6c65 6f62  .GzipFile(fileob
+00000d60: 6a3d 7572 6c2c 206d 6f64 653d 2272 6222  j=url, mode="rb"
+00000d70: 2920 6173 2066 723a 0a20 2020 2020 2020  ) as fr:.       
+00000d80: 2077 6974 6820 6f70 656e 2864 6573 7469   with open(desti
+00000d90: 6e61 7469 6f6e 2c20 6d6f 6465 3d22 7762  nation, mode="wb
+00000da0: 2229 2061 7320 6677 3a0a 2020 2020 2020  ") as fw:.      
+00000db0: 2020 2020 2020 6677 2e77 7269 7465 2866        fw.write(f
+00000dc0: 722e 7265 6164 2829 290a 0a23 2032 2e20  r.read())..# 2. 
+00000dd0: 5061 7273 6520 7468 6520 6669 6c65 0a61  Parse the file.a
+00000de0: 7274 6963 6c65 5f73 6574 203d 2070 6172  rticle_set = par
+00000df0: 7365 5f70 7562 6d65 645f 786d 6c28 6465  se_pubmed_xml(de
+00000e00: 7374 696e 6174 696f 6e29 0a61 7373 6572  stination).asser
+00000e10: 7420 6973 696e 7374 616e 6365 2861 7274  t isinstance(art
+00000e20: 6963 6c65 5f73 6574 2c20 5075 626d 6564  icle_set, Pubmed
+00000e30: 4172 7469 636c 6553 6574 290a 0a23 2033  ArticleSet)..# 3
+00000e40: 2e20 4765 7420 7468 6520 6e75 6d62 6572  . Get the number
+00000e50: 206f 6620 6369 7461 7469 6f6e 7320 696e   of citations in
+00000e60: 2074 6865 2066 696c 650a 7072 696e 7428   the file.print(
+00000e70: 6622 4e75 6d62 6572 206f 6620 6369 7461  f"Number of cita
+00000e80: 7469 6f6e 733a 207b 6c65 6e28 6172 7469  tions: {len(arti
+00000e90: 636c 655f 7365 742e 7075 626d 6564 5f61  cle_set.pubmed_a
+00000ea0: 7274 6963 6c65 297d 2229 0a70 7269 6e74  rticle)}").print
+00000eb0: 2866 227b 6172 7469 636c 655f 7365 742e  (f"{article_set.
+00000ec0: 7075 626d 6564 5f61 7274 6963 6c65 5b30  pubmed_article[0
+00000ed0: 5d2e 6d65 646c 696e 655f 6369 7461 7469  ].medline_citati
+00000ee0: 6f6e 2e61 7274 6963 6c65 2e61 7274 6963  on.article.artic
+00000ef0: 6c65 5f74 6974 6c65 2e63 6f6e 7465 6e74  le_title.content
+00000f00: 5b30 5d7d 2229 0a60 6060 0a0a 4f75 7470  [0]}").```..Outp
+00000f10: 7574 3a0a 0a60 6060 6261 7368 0a4e 756d  ut:..```bash.Num
+00000f20: 6265 7220 6f66 2063 6974 6174 696f 6e73  ber of citations
+00000f30: 3a20 3235 3433 0a41 2050 6174 656e 7420  : 2543.A Patent 
+00000f40: 616e 6420 5061 7474 6572 6e20 4d6f 7468  and Pattern Moth
+00000f50: 6572 2e0a 6060 600a 0a23 2320 4641 510a  er..```..## FAQ.
+00000f60: 0a23 2323 2057 6879 2064 6f65 7320 6974  .### Why does it
+00000f70: 2074 616b 6520 736f 206c 6f6e 6720 746f   take so long to
+00000f80: 2070 6172 7365 2061 2070 7562 6d65 6420   parse a pubmed 
+00000f90: 6369 7461 7469 6f6e 2073 6574 0a0a 5468  citation set..Th
+00000fa0: 6572 6520 6973 2061 206c 6f74 206f 6620  ere is a lot of 
+00000fb0: 6461 7461 2c20 616e 6420 7468 6520 7363  data, and the sc
+00000fc0: 6865 6d61 2069 7320 6465 6570 2061 6e64  hema is deep and
+00000fd0: 2063 6f6d 706c 6578 2e0a 0a23 2323 2057   complex...### W
+00000fe0: 6879 2061 7265 2074 6865 2072 6574 7572  hy are the retur
+00000ff0: 6e20 7374 7275 6374 7572 6573 2073 6f20  n structures so 
+00001000: 636f 6d70 6c69 6361 7465 643f 0a0a 5468  complicated?..Th
+00001010: 6520 7265 7475 726e 2073 7472 7563 7475  e return structu
+00001020: 7265 7320 6172 6520 6120 6469 7265 6374  res are a direct
+00001030: 2072 6566 6c65 6374 696f 6e20 6f66 2074   reflection of t
+00001040: 6865 2058 4d4c 2066 6f72 6d61 7420 6465  he XML format de
+00001050: 6669 6e65 6420 6279 2074 6865 204e 4c4d  fined by the NLM
+00001060: 2e20 496e 0a74 6865 2066 7574 7572 6520  . In.the future 
+00001070: 736f 6d65 2075 7469 6c69 7479 2063 6c61  some utility cla
+00001080: 7373 6573 206d 6967 6874 2062 6520 6d61  sses might be ma
+00001090: 6465 2066 6f72 2063 6f6d 6d6f 6e20 636f  de for common co
+000010a0: 6d70 6f6e 656e 7473 2028 7469 746c 652c  mponents (title,
+000010b0: 2061 7574 686f 7273 2c0a 6574 6329 2c20   authors,.etc), 
+000010c0: 6275 7420 666f 7220 6e6f 7720 7468 6973  but for now this
+000010d0: 2069 7320 696e 7465 6e64 6564 2074 6f20   is intended to 
+000010e0: 6265 2061 6e20 756e 6269 6173 6564 2077  be an unbiased w
+000010f0: 6179 206f 6620 7061 7273 696e 6720 7468  ay of parsing th
+00001100: 6520 584d 4c2e 0a                        e XML..
```

### Comparing `pubmed_types-0.1.1/pyproject.toml` & `pubmed_types-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pubmed-types"
-version = "0.1.1"
+version = "0.1.2"
 authors = ["Nick Schaub <nick.schaub@nih.gov>"]
 description = "Pubmed XML parsing and typehints."
 readme = "README.md"
 license = "MIT"
 packages = [{include = "pubmed_types", from = "src"}]
 homepage = "https://github.com/nicholas-schaub/pubmed-types"
 repository = "https://github.com/nicholas-schaub/pubmed-types"
```

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/__init__.py` & `pubmed_types-0.1.2/src/pubmed_types/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/abbrev_journal_title.py` & `pubmed_types-0.1.2/src/pubmed_types/models/abbrev_journal_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/abstract_1.py` & `pubmed_types-0.1.2/src/pubmed_types/models/abstract_1.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/abstract_text.py` & `pubmed_types-0.1.2/src/pubmed_types/models/abstract_text.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/access_date.py` & `pubmed_types-0.1.2/src/pubmed_types/models/access_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/affiliation.py` & `pubmed_types-0.1.2/src/pubmed_types/models/affiliation.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/affiliation_info.py` & `pubmed_types-0.1.2/src/pubmed_types/models/affiliation_info.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/alt_text.py` & `pubmed_types-0.1.2/src/pubmed_types/models/alt_text.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/app.py` & `pubmed_types-0.1.2/src/pubmed_types/models/app.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/app_group.py` & `pubmed_types-0.1.2/src/pubmed_types/models/app_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/article_1.py` & `pubmed_types-0.1.2/src/pubmed_types/models/article_1.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/article_2.py` & `pubmed_types-0.1.2/src/pubmed_types/models/article_2.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/article_categories.py` & `pubmed_types-0.1.2/src/pubmed_types/models/article_categories.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/article_date.py` & `pubmed_types-0.1.2/src/pubmed_types/models/article_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/article_id.py` & `pubmed_types-0.1.2/src/pubmed_types/models/article_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/article_meta.py` & `pubmed_types-0.1.2/src/pubmed_types/models/article_meta.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/article_title_1.py` & `pubmed_types-0.1.2/src/pubmed_types/models/article_title_1.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/article_version.py` & `pubmed_types-0.1.2/src/pubmed_types/models/article_version.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/article_version_alternatives.py` & `pubmed_types-0.1.2/src/pubmed_types/models/article_version_alternatives.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/author.py` & `pubmed_types-0.1.2/src/pubmed_types/models/author.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/author_list.py` & `pubmed_types-0.1.2/src/pubmed_types/models/author_list.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/author_notes.py` & `pubmed_types-0.1.2/src/pubmed_types/models/author_notes.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/award_desc.py` & `pubmed_types-0.1.2/src/pubmed_types/models/award_desc.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/award_group.py` & `pubmed_types-0.1.2/src/pubmed_types/models/award_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/award_name.py` & `pubmed_types-0.1.2/src/pubmed_types/models/award_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/back.py` & `pubmed_types-0.1.2/src/pubmed_types/models/back.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/beginning_date.py` & `pubmed_types-0.1.2/src/pubmed_types/models/beginning_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/body.py` & `pubmed_types-0.1.2/src/pubmed_types/models/body.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/book.py` & `pubmed_types-0.1.2/src/pubmed_types/models/book.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/book_document.py` & `pubmed_types-0.1.2/src/pubmed_types/models/book_document.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/book_document_set.py` & `pubmed_types-0.1.2/src/pubmed_types/models/book_document_set.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/book_title.py` & `pubmed_types-0.1.2/src/pubmed_types/models/book_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/break_mod.py` & `pubmed_types-0.1.2/src/pubmed_types/models/break_mod.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/chemical.py` & `pubmed_types-0.1.2/src/pubmed_types/models/chemical.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/citation.py` & `pubmed_types-0.1.2/src/pubmed_types/models/citation.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/city.py` & `pubmed_types-0.1.2/src/pubmed_types/models/city.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/coi_statement.py` & `pubmed_types-0.1.2/src/pubmed_types/models/coi_statement.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/col.py` & `pubmed_types-0.1.2/src/pubmed_types/models/col.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/colgroup.py` & `pubmed_types-0.1.2/src/pubmed_types/models/colgroup.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/collection_title.py` & `pubmed_types-0.1.2/src/pubmed_types/models/collection_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/collective_name.py` & `pubmed_types-0.1.2/src/pubmed_types/models/collective_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/comments_corrections.py` & `pubmed_types-0.1.2/src/pubmed_types/models/comments_corrections.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/comments_corrections_ref_type.py` & `pubmed_types-0.1.2/src/pubmed_types/models/comments_corrections_ref_type.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/conf_num.py` & `pubmed_types-0.1.2/src/pubmed_types/models/conf_num.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/conf_theme.py` & `pubmed_types-0.1.2/src/pubmed_types/models/conf_theme.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/conference.py` & `pubmed_types-0.1.2/src/pubmed_types/models/conference.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/contrib_id.py` & `pubmed_types-0.1.2/src/pubmed_types/models/contrib_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/contributed_resource_group.py` & `pubmed_types-0.1.2/src/pubmed_types/models/contributed_resource_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/contribution_date.py` & `pubmed_types-0.1.2/src/pubmed_types/models/contribution_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/copyright_year.py` & `pubmed_types-0.1.2/src/pubmed_types/models/copyright_year.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/corresp.py` & `pubmed_types-0.1.2/src/pubmed_types/models/corresp.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/count.py` & `pubmed_types-0.1.2/src/pubmed_types/models/count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/counts.py` & `pubmed_types-0.1.2/src/pubmed_types/models/counts.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/custom_meta.py` & `pubmed_types-0.1.2/src/pubmed_types/models/custom_meta.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/custom_meta_group.py` & `pubmed_types-0.1.2/src/pubmed_types/models/custom_meta_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/data_bank.py` & `pubmed_types-0.1.2/src/pubmed_types/models/data_bank.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/data_bank_list.py` & `pubmed_types-0.1.2/src/pubmed_types/models/data_bank_list.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/date_completed.py` & `pubmed_types-0.1.2/src/pubmed_types/models/date_completed.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/date_revised.py` & `pubmed_types-0.1.2/src/pubmed_types/models/date_revised.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/day.py` & `pubmed_types-0.1.2/src/pubmed_types/models/day.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/descriptor_name.py` & `pubmed_types-0.1.2/src/pubmed_types/models/descriptor_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/elocation_id.py` & `pubmed_types-0.1.2/src/pubmed_types/models/elocation_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/elocation_id_1.py` & `pubmed_types-0.1.2/src/pubmed_types/models/elocation_id_1.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/ending_date.py` & `pubmed_types-0.1.2/src/pubmed_types/models/ending_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/equation_count.py` & `pubmed_types-0.1.2/src/pubmed_types/models/equation_count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/era.py` & `pubmed_types-0.1.2/src/pubmed_types/models/era.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/event.py` & `pubmed_types-0.1.2/src/pubmed_types/models/event.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/event_desc.py` & `pubmed_types-0.1.2/src/pubmed_types/models/event_desc.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/extended_by.py` & `pubmed_types-0.1.2/src/pubmed_types/models/extended_by.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/fig_count.py` & `pubmed_types-0.1.2/src/pubmed_types/models/fig_count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/floats_group.py` & `pubmed_types-0.1.2/src/pubmed_types/models/floats_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/fpage.py` & `pubmed_types-0.1.2/src/pubmed_types/models/fpage.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/front.py` & `pubmed_types-0.1.2/src/pubmed_types/models/front.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/front_stub.py` & `pubmed_types-0.1.2/src/pubmed_types/models/front_stub.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/funding_group.py` & `pubmed_types-0.1.2/src/pubmed_types/models/funding_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/funding_statement.py` & `pubmed_types-0.1.2/src/pubmed_types/models/funding_statement.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/glyph_data.py` & `pubmed_types-0.1.2/src/pubmed_types/models/glyph_data.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/glyph_ref.py` & `pubmed_types-0.1.2/src/pubmed_types/models/glyph_ref.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/grant.py` & `pubmed_types-0.1.2/src/pubmed_types/models/grant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/grant_list.py` & `pubmed_types-0.1.2/src/pubmed_types/models/grant_list.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/group.py` & `pubmed_types-0.1.2/src/pubmed_types/models/group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/history_2.py` & `pubmed_types-0.1.2/src/pubmed_types/models/history_2.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/hr.py` & `pubmed_types-0.1.2/src/pubmed_types/models/hr.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/i.py` & `pubmed_types-0.1.2/src/pubmed_types/models/i.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/index_term_range_end.py` & `pubmed_types-0.1.2/src/pubmed_types/models/index_term_range_end.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/individual_name.py` & `pubmed_types-0.1.2/src/pubmed_types/models/individual_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/institution_id.py` & `pubmed_types-0.1.2/src/pubmed_types/models/institution_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/investigator.py` & `pubmed_types-0.1.2/src/pubmed_types/models/investigator.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/issn_1.py` & `pubmed_types-0.1.2/src/pubmed_types/models/issn_1.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/issue_id.py` & `pubmed_types-0.1.2/src/pubmed_types/models/issue_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/issue_sponsor.py` & `pubmed_types-0.1.2/src/pubmed_types/models/issue_sponsor.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/issue_subtitle.py` & `pubmed_types-0.1.2/src/pubmed_types/models/issue_subtitle.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/issue_title_group.py` & `pubmed_types-0.1.2/src/pubmed_types/models/issue_title_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/journal.py` & `pubmed_types-0.1.2/src/pubmed_types/models/journal.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/journal_id.py` & `pubmed_types-0.1.2/src/pubmed_types/models/journal_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/journal_issue.py` & `pubmed_types-0.1.2/src/pubmed_types/models/journal_issue.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/journal_meta.py` & `pubmed_types-0.1.2/src/pubmed_types/models/journal_meta.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/journal_subtitle.py` & `pubmed_types-0.1.2/src/pubmed_types/models/journal_subtitle.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/journal_title.py` & `pubmed_types-0.1.2/src/pubmed_types/models/journal_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/journal_title_group.py` & `pubmed_types-0.1.2/src/pubmed_types/models/journal_title_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/keyword.py` & `pubmed_types-0.1.2/src/pubmed_types/models/keyword.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/keyword_list.py` & `pubmed_types-0.1.2/src/pubmed_types/models/keyword_list.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/lpage.py` & `pubmed_types-0.1.2/src/pubmed_types/models/lpage.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/medline_citation.py` & `pubmed_types-0.1.2/src/pubmed_types/models/medline_citation.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/medline_journal_info.py` & `pubmed_types-0.1.2/src/pubmed_types/models/medline_journal_info.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/mesh_heading.py` & `pubmed_types-0.1.2/src/pubmed_types/models/mesh_heading.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/meta_name.py` & `pubmed_types-0.1.2/src/pubmed_types/models/meta_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/meta_value.py` & `pubmed_types-0.1.2/src/pubmed_types/models/meta_value.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/milestone_end.py` & `pubmed_types-0.1.2/src/pubmed_types/models/milestone_end.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/milestone_start.py` & `pubmed_types-0.1.2/src/pubmed_types/models/milestone_start.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/month.py` & `pubmed_types-0.1.2/src/pubmed_types/models/month.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/object_id.py` & `pubmed_types-0.1.2/src/pubmed_types/models/object_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/free_to_read.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/free_to_read.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/license_ref.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/license_ref.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/__init__.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/__init__.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/abs.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/abs.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/annotation.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/annotation.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/approx.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/approx.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arg.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arg.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cbytes.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cbytes.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ceiling.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ceiling.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/condition.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/condition.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/conjugate.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/conjugate.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cs.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cs.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/divide.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/divide.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/exp.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/exp.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/factorial.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/factorial.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/factorof.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/factorof.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/floor.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/floor.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/imaginary.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/imaginary.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maligngroup.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maligngroup.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/malignmark.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/malignmark.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_mathvariant.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_mathvariant.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_mathvariant.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/minus.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/minus.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlabeledtr.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlabeledtr.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_mathvariant.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_mathvariant.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mprescripts.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mprescripts.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_mathvariant.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msline.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msline.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_mathvariant.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_mathvariant.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_mathvariant.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtr.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtr.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/neq.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/neq.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/none.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/none.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/power.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/power.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/quotient.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/quotient.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/real.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/real.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/rem.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/rem.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/root.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/root.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/share.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/share.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/tendsto.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/tendsto.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/arc_type.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/arc_type.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/extended.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/extended.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/locator_type.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/locator_type.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/resource_type.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/resource_type.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/simple.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/simple.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/title_elt_type.py` & `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/title_elt_type.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/other_abstract.py` & `pubmed_types-0.1.2/src/pubmed_types/models/other_abstract.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/other_id.py` & `pubmed_types-0.1.2/src/pubmed_types/models/other_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/overline_end.py` & `pubmed_types-0.1.2/src/pubmed_types/models/overline_end.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/overline_start.py` & `pubmed_types-0.1.2/src/pubmed_types/models/overline_start.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/page_count.py` & `pubmed_types-0.1.2/src/pubmed_types/models/page_count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/page_range.py` & `pubmed_types-0.1.2/src/pubmed_types/models/page_range.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/pagination.py` & `pubmed_types-0.1.2/src/pubmed_types/models/pagination.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/param.py` & `pubmed_types-0.1.2/src/pubmed_types/models/param.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/personal_name_subject.py` & `pubmed_types-0.1.2/src/pubmed_types/models/personal_name_subject.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/postal_code.py` & `pubmed_types-0.1.2/src/pubmed_types/models/postal_code.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/principal_award_recipient.py` & `pubmed_types-0.1.2/src/pubmed_types/models/principal_award_recipient.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/principal_investigator.py` & `pubmed_types-0.1.2/src/pubmed_types/models/principal_investigator.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/processing_meta.py` & `pubmed_types-0.1.2/src/pubmed_types/models/processing_meta.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/pub_date_1.py` & `pubmed_types-0.1.2/src/pubmed_types/models/pub_date_1.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/pub_date_2.py` & `pubmed_types-0.1.2/src/pubmed_types/models/pub_date_2.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/pub_date_not_available.py` & `pubmed_types-0.1.2/src/pubmed_types/models/pub_date_not_available.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/pub_history.py` & `pubmed_types-0.1.2/src/pubmed_types/models/pub_history.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/pub_id.py` & `pubmed_types-0.1.2/src/pubmed_types/models/pub_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/pub_med_pub_date.py` & `pubmed_types-0.1.2/src/pubmed_types/models/pub_med_pub_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/publisher.py` & `pubmed_types-0.1.2/src/pubmed_types/models/publisher.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/publisher_1.py` & `pubmed_types-0.1.2/src/pubmed_types/models/publisher_1.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/publisher_2.py` & `pubmed_types-0.1.2/src/pubmed_types/models/publisher_2.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/publisher_name_1.py` & `pubmed_types-0.1.2/src/pubmed_types/models/publisher_name_1.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/pubmed_article.py` & `pubmed_types-0.1.2/src/pubmed_types/models/pubmed_article.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/pubmed_article_set.py` & `pubmed_types-0.1.2/src/pubmed_types/models/pubmed_article_set.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/pubmed_book_article.py` & `pubmed_types-0.1.2/src/pubmed_types/models/pubmed_book_article.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/pubmed_book_data.py` & `pubmed_types-0.1.2/src/pubmed_types/models/pubmed_book_data.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/pubmed_data.py` & `pubmed_types-0.1.2/src/pubmed_types/models/pubmed_data.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/qualifier_name.py` & `pubmed_types-0.1.2/src/pubmed_types/models/qualifier_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/ref_count.py` & `pubmed_types-0.1.2/src/pubmed_types/models/ref_count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/reference.py` & `pubmed_types-0.1.2/src/pubmed_types/models/reference.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/reference_list.py` & `pubmed_types-0.1.2/src/pubmed_types/models/reference_list.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/resource_group.py` & `pubmed_types-0.1.2/src/pubmed_types/models/resource_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/resource_id.py` & `pubmed_types-0.1.2/src/pubmed_types/models/resource_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/resource_name.py` & `pubmed_types-0.1.2/src/pubmed_types/models/resource_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/resource_wrap.py` & `pubmed_types-0.1.2/src/pubmed_types/models/resource_wrap.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/response.py` & `pubmed_types-0.1.2/src/pubmed_types/models/response.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/restricted_by.py` & `pubmed_types-0.1.2/src/pubmed_types/models/restricted_by.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/rp.py` & `pubmed_types-0.1.2/src/pubmed_types/models/rp.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/rt.py` & `pubmed_types-0.1.2/src/pubmed_types/models/rt.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/season.py` & `pubmed_types-0.1.2/src/pubmed_types/models/season.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/section.py` & `pubmed_types-0.1.2/src/pubmed_types/models/section.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/section_title.py` & `pubmed_types-0.1.2/src/pubmed_types/models/section_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/self_uri.py` & `pubmed_types-0.1.2/src/pubmed_types/models/self_uri.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/series_text.py` & `pubmed_types-0.1.2/src/pubmed_types/models/series_text.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/series_title.py` & `pubmed_types-0.1.2/src/pubmed_types/models/series_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/sig.py` & `pubmed_types-0.1.2/src/pubmed_types/models/sig.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/sig_block.py` & `pubmed_types-0.1.2/src/pubmed_types/models/sig_block.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/state.py` & `pubmed_types-0.1.2/src/pubmed_types/models/state.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/string_conf.py` & `pubmed_types-0.1.2/src/pubmed_types/models/string_conf.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/sub_1.py` & `pubmed_types-0.1.2/src/pubmed_types/models/sub_1.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/sub_article.py` & `pubmed_types-0.1.2/src/pubmed_types/models/sub_article.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/suffix_1.py` & `pubmed_types-0.1.2/src/pubmed_types/models/suffix_1.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/sup_1.py` & `pubmed_types-0.1.2/src/pubmed_types/models/sup_1.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/suppl_mesh_name.py` & `pubmed_types-0.1.2/src/pubmed_types/models/suppl_mesh_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/support_description.py` & `pubmed_types-0.1.2/src/pubmed_types/models/support_description.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/support_group.py` & `pubmed_types-0.1.2/src/pubmed_types/models/support_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/support_source.py` & `pubmed_types-0.1.2/src/pubmed_types/models/support_source.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/table_count.py` & `pubmed_types-0.1.2/src/pubmed_types/models/table_count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/tex_math.py` & `pubmed_types-0.1.2/src/pubmed_types/models/tex_math.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/title_group.py` & `pubmed_types-0.1.2/src/pubmed_types/models/title_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/trans_abstract.py` & `pubmed_types-0.1.2/src/pubmed_types/models/trans_abstract.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/trans_subtitle.py` & `pubmed_types-0.1.2/src/pubmed_types/models/trans_subtitle.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/trans_title_group.py` & `pubmed_types-0.1.2/src/pubmed_types/models/trans_title_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/u.py` & `pubmed_types-0.1.2/src/pubmed_types/models/u.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/underline_end.py` & `pubmed_types-0.1.2/src/pubmed_types/models/underline_end.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/underline_start.py` & `pubmed_types-0.1.2/src/pubmed_types/models/underline_start.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/url.py` & `pubmed_types-0.1.2/src/pubmed_types/models/url.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/url_lang.py` & `pubmed_types-0.1.2/src/pubmed_types/models/url_lang.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/vernacular_title.py` & `pubmed_types-0.1.2/src/pubmed_types/models/vernacular_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/volume_issue_group.py` & `pubmed_types-0.1.2/src/pubmed_types/models/volume_issue_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/volume_title.py` & `pubmed_types-0.1.2/src/pubmed_types/models/volume_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/word_count.py` & `pubmed_types-0.1.2/src/pubmed_types/models/word_count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/src/pubmed_types/models/year.py` & `pubmed_types-0.1.2/src/pubmed_types/models/year.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.1/PKG-INFO` & `pubmed_types-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7075 626d  : 2.1.Name: pubm
 00000020: 6564 2d74 7970 6573 0a56 6572 7369 6f6e  ed-types.Version
-00000030: 3a20 302e 312e 310a 5375 6d6d 6172 793a  : 0.1.1.Summary:
+00000030: 3a20 302e 312e 320a 5375 6d6d 6172 793a  : 0.1.2.Summary:
 00000040: 2050 7562 6d65 6420 584d 4c20 7061 7273   Pubmed XML pars
 00000050: 696e 6720 616e 6420 7479 7065 6869 6e74  ing and typehint
 00000060: 732e 0a48 6f6d 652d 7061 6765 3a20 6874  s..Home-page: ht
 00000070: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00000080: 2f6e 6963 686f 6c61 732d 7363 6861 7562  /nicholas-schaub
 00000090: 2f70 7562 6d65 642d 7479 7065 730a 4c69  /pubmed-types.Li
 000000a0: 6365 6e73 653a 204d 4954 0a41 7574 686f  cense: MIT.Autho
@@ -67,252 +67,279 @@
 00000420: 746f 7279 2c20 6874 7470 733a 2f2f 6769  tory, https://gi
 00000430: 7468 7562 2e63 6f6d 2f6e 6963 686f 6c61  thub.com/nichola
 00000440: 732d 7363 6861 7562 2f70 7562 6d65 642d  s-schaub/pubmed-
 00000450: 7479 7065 730a 4465 7363 7269 7074 696f  types.Descriptio
 00000460: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
 00000470: 7465 7874 2f6d 6172 6b64 6f77 6e0a 0a23  text/markdown..#
 00000480: 2070 7562 6d65 642d 7479 7065 7320 2876   pubmed-types (v
-00000490: 302e 312e 3129 0a0a 2323 2049 6e74 726f  0.1.1)..## Intro
-000004a0: 6475 6374 696f 6e0a 0a41 2063 6f6d 706c  duction..A compl
-000004b0: 6574 6520 696d 706c 656d 656e 7461 7469  ete implementati
-000004c0: 6f6e 206f 6620 7468 6520 584d 4c20 7363  on of the XML sc
-000004d0: 6865 6d61 2066 6f72 2050 4d43 204f 7065  hema for PMC Ope
-000004e0: 6e20 4163 6365 7373 2061 7274 6963 6c65  n Access article
-000004f0: 7320 616e 6420 5075 626d 6564 0a61 7274  s and Pubmed.art
-00000500: 6963 6c65 2073 6574 7320 2863 6974 6174  icle sets (citat
-00000510: 696f 6e73 292e 0a0a 5468 6973 2070 6163  ions)...This pac
-00000520: 6b61 6765 2068 656c 7073 2074 6f20 7061  kage helps to pa
-00000530: 7273 6520 5075 624d 6564 2058 4d4c 2064  rse PubMed XML d
-00000540: 6174 6120 696e 746f 2050 7964 616e 7469  ata into Pydanti
-00000550: 6320 6d6f 6465 6c73 2e20 5468 6973 2076  c models. This v
-00000560: 616c 6964 6174 6573 2074 6865 0a69 6e70  alidates the.inp
-00000570: 7574 2078 6d6c 2064 6174 6120 616e 6420  ut xml data and 
-00000580: 7072 6f76 6964 6573 2074 7970 6568 696e  provides typehin
-00000590: 7473 2066 6f72 2077 6f72 6b69 6e67 2077  ts for working w
-000005a0: 6974 6820 7468 6520 636f 6d70 6c65 7820  ith the complex 
-000005b0: 584d 4c20 7374 7275 6374 7572 6573 0a70  XML structures.p
-000005c0: 7265 7365 6e74 2069 6e20 5075 624d 6564  resent in PubMed
-000005d0: 2064 6174 612e 0a0a 2323 2057 6879 2064   data...## Why d
-000005e0: 6f20 4920 6e65 6564 2074 6869 733f 0a0a  o I need this?..
-000005f0: 5075 624d 6564 206b 6565 7073 2074 7261  PubMed keeps tra
-00000600: 636b 206f 6620 3130 7320 6f66 206d 696c  ck of 10s of mil
-00000610: 6c69 6f6e 7320 6f66 2072 6573 6561 7263  lions of researc
-00000620: 6820 6461 7461 2c20 616e 6420 6120 636f  h data, and a co
-00000630: 6d70 6c65 7820 584d 4c20 7374 7275 6374  mplex XML struct
-00000640: 7572 6520 6973 0a75 7365 6420 746f 2073  ure is.used to s
-00000650: 746f 7265 2069 742e 2050 6172 7369 6e67  tore it. Parsing
-00000660: 2058 4d4c 206f 6e20 6974 7320 6f77 6e20   XML on its own 
-00000670: 6973 2063 6861 6c6c 656e 6769 6e67 2065  is challenging e
-00000680: 6e6f 7567 682e 2041 6464 2074 6f20 6974  nough. Add to it
-00000690: 2074 6865 2066 6561 7475 7265 0a72 6963   the feature.ric
-000006a0: 6820 6461 7461 2069 6e73 6964 6520 6f66  h data inside of
-000006b0: 2065 6163 6820 6369 7461 7469 6f6e 2c20   each citation, 
-000006c0: 616e 6420 796f 7520 7769 6c6c 2066 696e  and you will fin
-000006d0: 6420 796f 7572 7365 6c66 2077 6974 6820  d yourself with 
-000006e0: 686f 7572 7320 6f72 2064 6179 7320 6f66  hours or days of
-000006f0: 0a6e 6176 6967 6174 696e 6720 7468 6520  .navigating the 
-00000700: 584d 4c20 7374 7275 6374 7572 652e 0a0a  XML structure...
-00000710: 5468 6520 6170 7072 6f61 6368 2068 6572  The approach her
-00000720: 6520 7761 7320 746f 2061 7574 6f67 656e  e was to autogen
-00000730: 6572 6174 6520 5079 6461 6e74 6963 2063  erate Pydantic c
-00000740: 6c61 7373 6573 2074 6f20 7061 7273 6520  lasses to parse 
-00000750: 7468 6520 584d 4c20 7573 696e 6720 7468  the XML using th
-00000760: 650a 6078 7364 6174 612d 7079 6461 6e74  e.`xsdata-pydant
-00000770: 6963 6020 746f 6f6c 2e20 5468 6973 2061  ic` tool. This a
-00000780: 7070 726f 6163 6820 6861 7320 7468 6520  pproach has the 
-00000790: 6265 6e65 6669 7420 6f66 206d 616b 696e  benefit of makin
-000007a0: 6720 7375 7265 2065 7665 7279 2070 6965  g sure every pie
-000007b0: 6365 206f 6620 6461 7461 0a69 7320 7061  ce of data.is pa
-000007c0: 7273 6564 2070 726f 7065 726c 792c 2061  rsed properly, a
-000007d0: 6e64 2061 6e20 6572 726f 7220 6973 2074  nd an error is t
-000007e0: 6872 6f77 6e20 6973 2073 6f6d 6574 6869  hrown is somethi
-000007f0: 6e67 2069 7320 6d69 7373 696e 6720 6f72  ng is missing or
-00000800: 2069 6e63 6f72 7265 6374 2e20 496e 7374   incorrect. Inst
-00000810: 6561 640a 6f66 2075 7369 6e67 2064 6963  ead.of using dic
-00000820: 7469 6f6e 6172 6965 7320 746f 2068 6f6c  tionaries to hol
-00000830: 6420 7468 6520 6461 7461 2c20 5079 6461  d the data, Pyda
-00000840: 6e74 6963 2063 6c61 7373 6573 2068 6176  ntic classes hav
-00000850: 6520 7468 6520 6265 6e65 6669 7420 6f66  e the benefit of
-00000860: 2070 726f 7669 6469 6e67 0a74 7970 6520   providing.type 
-00000870: 6869 6e74 7320 7769 7468 2074 6162 2063  hints with tab c
-00000880: 6f6d 706c 6574 696f 6e20 666f 7220 4944  ompletion for ID
-00000890: 4573 2c20 6d61 6b69 6e67 2069 7420 6561  Es, making it ea
-000008a0: 7369 6572 2074 6f20 6e61 7669 6761 7465  sier to navigate
-000008b0: 2074 6865 2063 6f6d 706c 6578 0a73 7472   the complex.str
-000008c0: 7563 7475 7265 206f 6620 7468 6520 6369  ucture of the ci
-000008d0: 7461 7469 6f6e 2064 6174 612e 0a0a 2323  tation data...##
-000008e0: 2048 6f77 2064 6f20 4920 7573 6520 6974   How do I use it
-000008f0: 3f0a 0a49 7420 6973 2070 6f73 7369 626c  ?..It is possibl
-00000900: 6520 746f 2075 7365 2060 7873 6461 7461  e to use `xsdata
-00000910: 2d70 7964 616e 7469 6360 2061 6e64 2074  -pydantic` and t
-00000920: 6865 2061 7574 6f67 656e 6572 6174 6564  he autogenerated
-00000930: 2063 6c61 7373 6573 2064 6972 6563 746c   classes directl
-00000940: 7920 746f 2070 6172 7365 0a61 6e20 584d  y to parse.an XM
-00000950: 4c20 6669 6c65 2c20 6275 7420 7765 2070  L file, but we p
-00000960: 726f 7669 6465 2061 2063 6f6e 7665 6e69  rovide a conveni
-00000970: 656e 6365 2066 756e 6374 696f 6e20 746f  ence function to
-00000980: 2065 6173 696c 7920 6f70 656e 2050 7562   easily open Pub
-00000990: 4d65 6420 584d 6c20 6369 7461 7469 6f6e  Med XMl citation
-000009a0: 730a 616e 6420 504d 4320 6f70 656e 2061  s.and PMC open a
-000009b0: 6363 6573 7320 6172 7469 636c 6573 2e0a  ccess articles..
-000009c0: 0a23 2323 2045 7861 6d70 6c65 2031 3a20  .### Example 1: 
-000009d0: 4120 504d 4320 4f70 656e 2041 6363 6573  A PMC Open Acces
-000009e0: 7320 4172 7469 636c 650a 0a60 6060 7079  s Article..```py
-000009f0: 7468 6f6e 0a69 6d70 6f72 7420 7461 7266  thon.import tarf
-00000a00: 696c 650a 696d 706f 7274 2075 726c 6c69  ile.import urlli
-00000a10: 622e 7265 7175 6573 7420 6173 2072 6571  b.request as req
-00000a20: 7565 7374 0a66 726f 6d20 636f 6e74 6578  uest.from contex
-00000a30: 746c 6962 2069 6d70 6f72 7420 636c 6f73  tlib import clos
-00000a40: 696e 670a 6672 6f6d 2070 6174 686c 6962  ing.from pathlib
-00000a50: 2069 6d70 6f72 7420 5061 7468 0a0a 6672   import Path..fr
-00000a60: 6f6d 2070 7562 6d65 645f 7479 7065 7320  om pubmed_types 
-00000a70: 696d 706f 7274 2070 6172 7365 5f70 7562  import parse_pub
-00000a80: 6d65 645f 786d 6c0a 0a23 2049 6e70 7574  med_xml..# Input
-00000a90: 2066 696c 6520 736f 7572 6365 2061 6e64   file source and
-00000aa0: 206f 7574 7075 7420 6669 6c65 2064 6573   output file des
-00000ab0: 7469 6e61 7469 6f6e 0a73 6f75 7263 6520  tination.source 
-00000ac0: 3d20 280a 2020 2020 2266 7470 3a2f 2f66  = (.    "ftp://f
-00000ad0: 7470 2e6e 6362 692e 6e6c 6d2e 6e69 682e  tp.ncbi.nlm.nih.
-00000ae0: 676f 7622 0a20 2020 202b 2022 2f70 7562  gov".    + "/pub
-00000af0: 2f70 6d63 2f6f 615f 6275 6c6b 2f6f 615f  /pmc/oa_bulk/oa_
-00000b00: 636f 6d6d 2f78 6d6c 220a 2020 2020 2b20  comm/xml".    + 
-00000b10: 222f 6f61 5f63 6f6d 6d5f 786d 6c2e 696e  "/oa_comm_xml.in
-00000b20: 6372 2e32 3032 332d 3033 2d32 312e 7461  cr.2023-03-21.ta
-00000b30: 722e 677a 220a 290a 6465 7374 696e 6174  r.gz".).destinat
-00000b40: 696f 6e20 3d20 5061 7468 2822 646f 776e  ion = Path("down
-00000b50: 6c6f 6164 7322 290a 6465 7374 696e 6174  loads").destinat
-00000b60: 696f 6e2e 6d6b 6469 7228 6578 6973 745f  ion.mkdir(exist_
-00000b70: 6f6b 3d54 7275 6529 0a0a 2320 312e 2047  ok=True)..# 1. G
-00000b80: 6574 2061 6e20 6f70 656e 2061 6363 6573  et an open acces
-00000b90: 7320 6172 7469 636c 6520 6461 7461 7365  s article datase
-00000ba0: 7420 6672 6f6d 2074 6865 2046 5450 2073  t from the FTP s
-00000bb0: 6572 7665 720a 7769 7468 2063 6c6f 7369  erver.with closi
-00000bc0: 6e67 2872 6571 7565 7374 2e75 726c 6f70  ng(request.urlop
-00000bd0: 656e 2873 6f75 7263 6529 2920 6173 2075  en(source)) as u
-00000be0: 726c 3a0a 2020 2020 7769 7468 2074 6172  rl:.    with tar
-00000bf0: 6669 6c65 2e6f 7065 6e28 6669 6c65 6f62  file.open(fileob
-00000c00: 6a3d 7572 6c2c 206d 6f64 653d 2272 3a67  j=url, mode="r:g
-00000c10: 7a22 2920 6173 2066 723a 0a20 2020 2020  z") as fr:.     
-00000c20: 2020 2066 722e 6578 7472 6163 7461 6c6c     fr.extractall
-00000c30: 2864 6573 7469 6e61 7469 6f6e 290a 0a23  (destination)..#
-00000c40: 2032 2e20 5061 7273 6520 7468 6520 6669   2. Parse the fi
-00000c50: 6c65 0a66 696c 655f 7061 7468 203d 2064  le.file_path = d
-00000c60: 6573 7469 6e61 7469 6f6e 2e6a 6f69 6e70  estination.joinp
-00000c70: 6174 6828 2250 4d43 3030 3978 7878 7878  ath("PMC009xxxxx
-00000c80: 7822 292e 6a6f 696e 7061 7468 2822 504d  x").joinpath("PM
-00000c90: 4339 3937 3036 3632 2e78 6d6c 2229 0a66  C9970662.xml").f
-00000ca0: 756c 6c5f 7465 7874 203d 2070 6172 7365  ull_text = parse
-00000cb0: 5f70 7562 6d65 645f 786d 6c28 6669 6c65  _pubmed_xml(file
-00000cc0: 5f70 6174 6829 0a0a 2320 332e 2050 7269  _path)..# 3. Pri
-00000cd0: 6e74 206f 7574 2074 6865 2061 7274 6963  nt out the artic
-00000ce0: 6c65 2074 6974 6c65 0a70 7269 6e74 2866  le title.print(f
-00000cf0: 2254 6974 6c65 3a20 7b66 756c 6c5f 7465  "Title: {full_te
-00000d00: 7874 2e66 726f 6e74 2e61 7274 6963 6c65  xt.front.article
-00000d10: 5f6d 6574 612e 7469 746c 655f 6772 6f75  _meta.title_grou
-00000d20: 702e 6172 7469 636c 655f 7469 746c 652e  p.article_title.
-00000d30: 636f 6e74 656e 745b 305d 7d22 290a 6060  content[0]}").``
-00000d40: 600a 0a4f 7574 7075 743a 0a0a 6060 6062  `..Output:..```b
-00000d50: 6173 680a 5469 746c 653a 204c 6163 7461  ash.Title: Lacta
-00000d60: 7465 2061 7320 6120 6d79 6f6b 696e 6520  te as a myokine 
-00000d70: 616e 6420 6578 6572 6b69 6e65 3a20 6472  and exerkine: dr
-00000d80: 6976 6572 7320 616e 6420 7369 676e 616c  ivers and signal
-00000d90: 7320 6f66 2070 6879 7369 6f6c 6f67 7920  s of physiology 
-00000da0: 616e 6420 6d65 7461 626f 6c69 736d 0a60  and metabolism.`
-00000db0: 6060 0a0a 2323 2320 4578 616d 706c 6520  ``..### Example 
-00000dc0: 323a 2041 2050 7562 6d65 6420 6261 7365  2: A Pubmed base
-00000dd0: 6c69 6e65 2063 6974 6174 696f 6e20 6669  line citation fi
-00000de0: 6c65 0a0a 2323 2320 4578 616d 706c 6520  le..### Example 
-00000df0: 313a 2041 2050 4d43 204f 7065 6e20 4163  1: A PMC Open Ac
-00000e00: 6365 7373 2041 7274 6963 6c65 0a0a 6060  cess Article..``
-00000e10: 6070 7974 686f 6e0a 696d 706f 7274 2067  `python.import g
-00000e20: 7a69 700a 696d 706f 7274 2075 726c 6c69  zip.import urlli
-00000e30: 622e 7265 7175 6573 7420 6173 2072 6571  b.request as req
-00000e40: 7565 7374 0a66 726f 6d20 636f 6e74 6578  uest.from contex
-00000e50: 746c 6962 2069 6d70 6f72 7420 636c 6f73  tlib import clos
-00000e60: 696e 670a 6672 6f6d 2070 6174 686c 6962  ing.from pathlib
-00000e70: 2069 6d70 6f72 7420 5061 7468 0a0a 6672   import Path..fr
-00000e80: 6f6d 2070 7562 6d65 645f 7479 7065 7320  om pubmed_types 
-00000e90: 696d 706f 7274 2070 6172 7365 5f70 7562  import parse_pub
-00000ea0: 6d65 645f 786d 6c2c 2050 7562 6d65 6441  med_xml, PubmedA
-00000eb0: 7274 6963 6c65 5365 740a 0a23 2049 6e70  rticleSet..# Inp
-00000ec0: 7574 2066 696c 6520 736f 7572 6365 2061  ut file source a
-00000ed0: 6e64 206f 7574 7075 7420 6669 6c65 2064  nd output file d
-00000ee0: 6573 7469 6e61 7469 6f6e 0a73 6f75 7263  estination.sourc
-00000ef0: 6520 3d20 2266 7470 3a2f 2f66 7470 2e6e  e = "ftp://ftp.n
-00000f00: 6362 692e 6e6c 6d2e 6e69 682e 676f 7622  cbi.nlm.nih.gov"
-00000f10: 202b 2022 2f70 7562 6d65 642f 7570 6461   + "/pubmed/upda
-00000f20: 7465 6669 6c65 7322 202b 2022 2f70 7562  tefiles" + "/pub
-00000f30: 6d65 6432 336e 3131 3638 2e78 6d6c 2e67  med23n1168.xml.g
-00000f40: 7a22 0a64 6573 7469 6e61 7469 6f6e 203d  z".destination =
-00000f50: 2050 6174 6828 2264 6f77 6e6c 6f61 6473   Path("downloads
-00000f60: 2229 2e6a 6f69 6e70 6174 6828 2270 7562  ").joinpath("pub
-00000f70: 6d65 6432 336e 3131 3638 2e78 6d6c 2229  med23n1168.xml")
-00000f80: 0a64 6573 7469 6e61 7469 6f6e 2e70 6172  .destination.par
-00000f90: 656e 742e 6d6b 6469 7228 6578 6973 745f  ent.mkdir(exist_
-00000fa0: 6f6b 3d54 7275 6529 0a0a 2320 312e 2047  ok=True)..# 1. G
-00000fb0: 6574 2061 2070 7562 6d65 6420 6369 7461  et a pubmed cita
-00000fc0: 7469 6f6e 2064 6169 6c79 2075 7064 6174  tion daily updat
-00000fd0: 6520 6669 6c65 2066 726f 6d20 7468 6520  e file from the 
-00000fe0: 4654 5020 7365 7276 6572 0a77 6974 6820  FTP server.with 
-00000ff0: 636c 6f73 696e 6728 7265 7175 6573 742e  closing(request.
-00001000: 7572 6c6f 7065 6e28 736f 7572 6365 2929  urlopen(source))
-00001010: 2061 7320 7572 6c3a 0a20 2020 2077 6974   as url:.    wit
-00001020: 6820 677a 6970 2e47 7a69 7046 696c 6528  h gzip.GzipFile(
-00001030: 6669 6c65 6f62 6a3d 7572 6c2c 206d 6f64  fileobj=url, mod
-00001040: 653d 2272 6222 2920 6173 2066 723a 0a20  e="rb") as fr:. 
-00001050: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
-00001060: 2864 6573 7469 6e61 7469 6f6e 2c20 6d6f  (destination, mo
-00001070: 6465 3d22 7762 2229 2061 7320 6677 3a0a  de="wb") as fw:.
-00001080: 2020 2020 2020 2020 2020 2020 6677 2e77              fw.w
-00001090: 7269 7465 2866 722e 7265 6164 2829 290a  rite(fr.read()).
-000010a0: 0a23 2032 2e20 5061 7273 6520 7468 6520  .# 2. Parse the 
-000010b0: 6669 6c65 0a61 7274 6963 6c65 5f73 6574  file.article_set
-000010c0: 203d 2070 6172 7365 5f70 7562 6d65 645f   = parse_pubmed_
-000010d0: 786d 6c28 6465 7374 696e 6174 696f 6e29  xml(destination)
-000010e0: 0a61 7373 6572 7420 6973 696e 7374 616e  .assert isinstan
-000010f0: 6365 2861 7274 6963 6c65 5f73 6574 2c20  ce(article_set, 
-00001100: 5075 626d 6564 4172 7469 636c 6553 6574  PubmedArticleSet
-00001110: 290a 0a23 2033 2e20 4765 7420 7468 6520  )..# 3. Get the 
-00001120: 6e75 6d62 6572 206f 6620 6369 7461 7469  number of citati
-00001130: 6f6e 7320 696e 2074 6865 2066 696c 650a  ons in the file.
-00001140: 7072 696e 7428 6622 4e75 6d62 6572 206f  print(f"Number o
-00001150: 6620 6369 7461 7469 6f6e 733a 207b 6c65  f citations: {le
-00001160: 6e28 6172 7469 636c 655f 7365 742e 7075  n(article_set.pu
-00001170: 626d 6564 5f61 7274 6963 6c65 297d 2229  bmed_article)}")
-00001180: 0a70 7269 6e74 2866 227b 6172 7469 636c  .print(f"{articl
-00001190: 655f 7365 742e 7075 626d 6564 5f61 7274  e_set.pubmed_art
-000011a0: 6963 6c65 5b30 5d2e 6d65 646c 696e 655f  icle[0].medline_
-000011b0: 6369 7461 7469 6f6e 2e61 7274 6963 6c65  citation.article
-000011c0: 2e61 7274 6963 6c65 5f74 6974 6c65 2e63  .article_title.c
-000011d0: 6f6e 7465 6e74 5b30 5d7d 2229 0a60 6060  ontent[0]}").```
-000011e0: 0a0a 4f75 7470 7574 3a0a 0a60 6060 6261  ..Output:..```ba
-000011f0: 7368 0a4e 756d 6265 7220 6f66 2063 6974  sh.Number of cit
-00001200: 6174 696f 6e73 3a20 3235 3433 0a41 2050  ations: 2543.A P
-00001210: 6174 656e 7420 616e 6420 5061 7474 6572  atent and Patter
-00001220: 6e20 4d6f 7468 6572 2e0a 6060 600a 0a23  n Mother..```..#
-00001230: 2320 4641 510a 0a23 2323 2057 6879 2064  # FAQ..### Why d
-00001240: 6f65 7320 6974 2074 616b 6520 736f 206c  oes it take so l
-00001250: 6f6e 6720 746f 2070 6172 7365 2061 2070  ong to parse a p
-00001260: 7562 6d65 6420 6369 7461 7469 6f6e 2073  ubmed citation s
-00001270: 6574 0a0a 5468 6572 6520 6973 2061 206c  et..There is a l
-00001280: 6f74 206f 6620 6461 7461 2c20 616e 6420  ot of data, and 
-00001290: 7468 6520 7363 6865 6d61 2069 7320 6465  the schema is de
-000012a0: 6570 2061 6e64 2063 6f6d 706c 6578 2e0a  ep and complex..
-000012b0: 0a23 2323 2057 6879 2061 7265 2074 6865  .### Why are the
-000012c0: 2072 6574 7572 6e20 7374 7275 6374 7572   return structur
-000012d0: 6573 2073 6f20 636f 6d70 6c69 6361 7465  es so complicate
-000012e0: 643f 0a0a 5468 6520 7265 7475 726e 2073  d?..The return s
-000012f0: 7472 7563 7475 7265 7320 6172 6520 6120  tructures are a 
-00001300: 6469 7265 6374 2072 6566 6c65 6374 696f  direct reflectio
-00001310: 6e20 6f66 2074 6865 2058 4d4c 2066 6f72  n of the XML for
-00001320: 6d61 7420 6465 6669 6e65 6420 6279 2074  mat defined by t
-00001330: 6865 204e 4c4d 2e20 496e 0a74 6865 2066  he NLM. In.the f
-00001340: 7574 7572 6520 736f 6d65 2075 7469 6c69  uture some utili
-00001350: 7479 2063 6c61 7373 6573 206d 6967 6874  ty classes might
-00001360: 2062 6520 6d61 6465 2066 6f72 2063 6f6d   be made for com
-00001370: 6d6f 6e20 636f 6d70 6f6e 656e 7473 2028  mon components (
-00001380: 7469 746c 652c 2061 7574 686f 7273 2c0a  title, authors,.
-00001390: 6574 6329 2c20 6275 7420 666f 7220 6e6f  etc), but for no
-000013a0: 7720 7468 6973 2069 7320 696e 7465 6e64  w this is intend
-000013b0: 6564 2074 6f20 6265 2061 6e20 756e 6269  ed to be an unbi
-000013c0: 6173 6564 2077 6179 206f 6620 7061 7273  ased way of pars
-000013d0: 696e 6720 7468 6520 584d 4c2e 0a0a       ing the XML...
+00000490: 302e 312e 3229 0a0a 3c70 2061 6c69 676e  0.1.2)..<p align
+000004a0: 3d22 6365 6e74 6572 223e 0a20 2020 203c  ="center">.    <
+000004b0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+000004c0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000004d0: 7079 7069 2f64 6d2f 7075 626d 6564 2d74  pypi/dm/pubmed-t
+000004e0: 7970 6573 3f73 7479 6c65 3d66 6c61 742d  ypes?style=flat-
+000004f0: 7371 7561 7265 2220 2f3e 0a20 2020 203c  square" />.    <
+00000500: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000510: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000520: 7079 7069 2f6c 2f70 7562 6d65 642d 7479  pypi/l/pubmed-ty
+00000530: 7065 733f 7374 796c 653d 666c 6174 2d73  pes?style=flat-s
+00000540: 7175 6172 6522 2f3e 0a20 2020 203c 696d  quare"/>.    <im
+00000550: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+00000560: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000570: 7069 2f76 2f70 7562 6d65 642d 7479 7065  pi/v/pubmed-type
+00000580: 733f 7374 796c 653d 666c 6174 2d73 7175  s?style=flat-squ
+00000590: 6172 6522 2f3e 0a20 2020 203c 6120 6872  are"/>.    <a hr
+000005a0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000005b0: 7562 2e63 6f6d 2f74 6566 7261 2f78 7364  ub.com/tefra/xsd
+000005c0: 6174 612d 7079 6461 6e74 6963 223e 3c69  ata-pydantic"><i
+000005d0: 6d67 2061 6c74 3d22 4275 696c 7420 7769  mg alt="Built wi
+000005e0: 7468 3a20 7873 6461 7461 2d70 7964 616e  th: xsdata-pydan
+000005f0: 7469 6322 2073 7263 3d22 6874 7470 733a  tic" src="https:
+00000600: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000610: 2f62 6164 6765 2f63 6f64 6525 3230 7374  /badge/code%20st
+00000620: 796c 652d 626c 6163 6b2d 3030 3030 3030  yle-black-000000
+00000630: 2e73 7667 223e 3c2f 613e 0a3c 2f70 3e0a  .svg"></a>.</p>.
+00000640: 0a23 2320 496e 7472 6f64 7563 7469 6f6e  .## Introduction
+00000650: 0a0a 4120 636f 6d70 6c65 7465 2069 6d70  ..A complete imp
+00000660: 6c65 6d65 6e74 6174 696f 6e20 6f66 2074  lementation of t
+00000670: 6865 2058 4d4c 2073 6368 656d 6120 666f  he XML schema fo
+00000680: 7220 504d 4320 4f70 656e 2041 6363 6573  r PMC Open Acces
+00000690: 7320 6172 7469 636c 6573 2061 6e64 2050  s articles and P
+000006a0: 7562 6d65 640a 6172 7469 636c 6520 7365  ubmed.article se
+000006b0: 7473 2028 6369 7461 7469 6f6e 7329 2e0a  ts (citations)..
+000006c0: 0a54 6869 7320 7061 636b 6167 6520 6865  .This package he
+000006d0: 6c70 7320 746f 2070 6172 7365 2050 7562  lps to parse Pub
+000006e0: 4d65 6420 584d 4c20 6461 7461 2069 6e74  Med XML data int
+000006f0: 6f20 5079 6461 6e74 6963 206d 6f64 656c  o Pydantic model
+00000700: 732e 2054 6869 7320 7661 6c69 6461 7465  s. This validate
+00000710: 7320 7468 650a 696e 7075 7420 786d 6c20  s the.input xml 
+00000720: 6461 7461 2061 6e64 2070 726f 7669 6465  data and provide
+00000730: 7320 7479 7065 6869 6e74 7320 666f 7220  s typehints for 
+00000740: 776f 726b 696e 6720 7769 7468 2074 6865  working with the
+00000750: 2063 6f6d 706c 6578 2058 4d4c 2073 7472   complex XML str
+00000760: 7563 7475 7265 730a 7072 6573 656e 7420  uctures.present 
+00000770: 696e 2050 7562 4d65 6420 6461 7461 2e0a  in PubMed data..
+00000780: 0a23 2320 5768 7920 646f 2049 206e 6565  .## Why do I nee
+00000790: 6420 7468 6973 3f0a 0a50 7562 4d65 6420  d this?..PubMed 
+000007a0: 6b65 6570 7320 7472 6163 6b20 6f66 2031  keeps track of 1
+000007b0: 3073 206f 6620 6d69 6c6c 696f 6e73 206f  0s of millions o
+000007c0: 6620 7265 7365 6172 6368 2064 6174 612c  f research data,
+000007d0: 2061 6e64 2061 2063 6f6d 706c 6578 2058   and a complex X
+000007e0: 4d4c 2073 7472 7563 7475 7265 2069 730a  ML structure is.
+000007f0: 7573 6564 2074 6f20 7374 6f72 6520 6974  used to store it
+00000800: 2e20 5061 7273 696e 6720 584d 4c20 6f6e  . Parsing XML on
+00000810: 2069 7473 206f 776e 2069 7320 6368 616c   its own is chal
+00000820: 6c65 6e67 696e 6720 656e 6f75 6768 2e20  lenging enough. 
+00000830: 4164 6420 746f 2069 7420 7468 6520 6665  Add to it the fe
+00000840: 6174 7572 650a 7269 6368 2064 6174 6120  ature.rich data 
+00000850: 696e 7369 6465 206f 6620 6561 6368 2063  inside of each c
+00000860: 6974 6174 696f 6e2c 2061 6e64 2079 6f75  itation, and you
+00000870: 2077 696c 6c20 6669 6e64 2079 6f75 7273   will find yours
+00000880: 656c 6620 7769 7468 2068 6f75 7273 206f  elf with hours o
+00000890: 7220 6461 7973 206f 660a 6e61 7669 6761  r days of.naviga
+000008a0: 7469 6e67 2074 6865 2058 4d4c 2073 7472  ting the XML str
+000008b0: 7563 7475 7265 2e0a 0a54 6865 2061 7070  ucture...The app
+000008c0: 726f 6163 6820 6865 7265 2077 6173 2074  roach here was t
+000008d0: 6f20 6175 746f 6765 6e65 7261 7465 2050  o autogenerate P
+000008e0: 7964 616e 7469 6320 636c 6173 7365 7320  ydantic classes 
+000008f0: 746f 2070 6172 7365 2074 6865 2058 4d4c  to parse the XML
+00000900: 2075 7369 6e67 2074 6865 0a60 7873 6461   using the.`xsda
+00000910: 7461 2d70 7964 616e 7469 6360 2074 6f6f  ta-pydantic` too
+00000920: 6c2e 2054 6869 7320 6170 7072 6f61 6368  l. This approach
+00000930: 2068 6173 2074 6865 2062 656e 6566 6974   has the benefit
+00000940: 206f 6620 6d61 6b69 6e67 2073 7572 6520   of making sure 
+00000950: 6576 6572 7920 7069 6563 6520 6f66 2064  every piece of d
+00000960: 6174 610a 6973 2070 6172 7365 6420 7072  ata.is parsed pr
+00000970: 6f70 6572 6c79 2c20 616e 6420 616e 2065  operly, and an e
+00000980: 7272 6f72 2069 7320 7468 726f 776e 2069  rror is thrown i
+00000990: 7320 736f 6d65 7468 696e 6720 6973 206d  s something is m
+000009a0: 6973 7369 6e67 206f 7220 696e 636f 7272  issing or incorr
+000009b0: 6563 742e 2049 6e73 7465 6164 0a6f 6620  ect. Instead.of 
+000009c0: 7573 696e 6720 6469 6374 696f 6e61 7269  using dictionari
+000009d0: 6573 2074 6f20 686f 6c64 2074 6865 2064  es to hold the d
+000009e0: 6174 612c 2050 7964 616e 7469 6320 636c  ata, Pydantic cl
+000009f0: 6173 7365 7320 6861 7665 2074 6865 2062  asses have the b
+00000a00: 656e 6566 6974 206f 6620 7072 6f76 6964  enefit of provid
+00000a10: 696e 670a 7479 7065 2068 696e 7473 2077  ing.type hints w
+00000a20: 6974 6820 7461 6220 636f 6d70 6c65 7469  ith tab completi
+00000a30: 6f6e 2066 6f72 2049 4445 732c 206d 616b  on for IDEs, mak
+00000a40: 696e 6720 6974 2065 6173 6965 7220 746f  ing it easier to
+00000a50: 206e 6176 6967 6174 6520 7468 6520 636f   navigate the co
+00000a60: 6d70 6c65 780a 7374 7275 6374 7572 6520  mplex.structure 
+00000a70: 6f66 2074 6865 2063 6974 6174 696f 6e20  of the citation 
+00000a80: 6461 7461 2e0a 0a23 2320 486f 7720 646f  data...## How do
+00000a90: 2049 2075 7365 2069 743f 0a0a 4974 2069   I use it?..It i
+00000aa0: 7320 706f 7373 6962 6c65 2074 6f20 7573  s possible to us
+00000ab0: 6520 6078 7364 6174 612d 7079 6461 6e74  e `xsdata-pydant
+00000ac0: 6963 6020 616e 6420 7468 6520 6175 746f  ic` and the auto
+00000ad0: 6765 6e65 7261 7465 6420 636c 6173 7365  generated classe
+00000ae0: 7320 6469 7265 6374 6c79 2074 6f20 7061  s directly to pa
+00000af0: 7273 650a 616e 2058 4d4c 2066 696c 652c  rse.an XML file,
+00000b00: 2062 7574 2077 6520 7072 6f76 6964 6520   but we provide 
+00000b10: 6120 636f 6e76 656e 6965 6e63 6520 6675  a convenience fu
+00000b20: 6e63 7469 6f6e 2074 6f20 6561 7369 6c79  nction to easily
+00000b30: 206f 7065 6e20 5075 624d 6564 2058 4d6c   open PubMed XMl
+00000b40: 2063 6974 6174 696f 6e73 0a61 6e64 2050   citations.and P
+00000b50: 4d43 206f 7065 6e20 6163 6365 7373 2061  MC open access a
+00000b60: 7274 6963 6c65 732e 0a0a 2323 2320 4578  rticles...### Ex
+00000b70: 616d 706c 6520 313a 2041 2050 4d43 204f  ample 1: A PMC O
+00000b80: 7065 6e20 4163 6365 7373 2041 7274 6963  pen Access Artic
+00000b90: 6c65 0a0a 6060 6070 7974 686f 6e0a 696d  le..```python.im
+00000ba0: 706f 7274 2074 6172 6669 6c65 0a69 6d70  port tarfile.imp
+00000bb0: 6f72 7420 7572 6c6c 6962 2e72 6571 7565  ort urllib.reque
+00000bc0: 7374 2061 7320 7265 7175 6573 740a 6672  st as request.fr
+00000bd0: 6f6d 2063 6f6e 7465 7874 6c69 6220 696d  om contextlib im
+00000be0: 706f 7274 2063 6c6f 7369 6e67 0a66 726f  port closing.fro
+00000bf0: 6d20 7061 7468 6c69 6220 696d 706f 7274  m pathlib import
+00000c00: 2050 6174 680a 0a66 726f 6d20 7075 626d   Path..from pubm
+00000c10: 6564 5f74 7970 6573 2069 6d70 6f72 7420  ed_types import 
+00000c20: 7061 7273 655f 7075 626d 6564 5f78 6d6c  parse_pubmed_xml
+00000c30: 0a0a 2320 496e 7075 7420 6669 6c65 2073  ..# Input file s
+00000c40: 6f75 7263 6520 616e 6420 6f75 7470 7574  ource and output
+00000c50: 2066 696c 6520 6465 7374 696e 6174 696f   file destinatio
+00000c60: 6e0a 736f 7572 6365 203d 2028 0a20 2020  n.source = (.   
+00000c70: 2022 6674 703a 2f2f 6674 702e 6e63 6269   "ftp://ftp.ncbi
+00000c80: 2e6e 6c6d 2e6e 6968 2e67 6f76 220a 2020  .nlm.nih.gov".  
+00000c90: 2020 2b20 222f 7075 622f 706d 632f 6f61    + "/pub/pmc/oa
+00000ca0: 5f62 756c 6b2f 6f61 5f63 6f6d 6d2f 786d  _bulk/oa_comm/xm
+00000cb0: 6c22 0a20 2020 202b 2022 2f6f 615f 636f  l".    + "/oa_co
+00000cc0: 6d6d 5f78 6d6c 2e69 6e63 722e 3230 3233  mm_xml.incr.2023
+00000cd0: 2d30 332d 3231 2e74 6172 2e67 7a22 0a29  -03-21.tar.gz".)
+00000ce0: 0a64 6573 7469 6e61 7469 6f6e 203d 2050  .destination = P
+00000cf0: 6174 6828 2264 6f77 6e6c 6f61 6473 2229  ath("downloads")
+00000d00: 0a64 6573 7469 6e61 7469 6f6e 2e6d 6b64  .destination.mkd
+00000d10: 6972 2865 7869 7374 5f6f 6b3d 5472 7565  ir(exist_ok=True
+00000d20: 290a 0a23 2031 2e20 4765 7420 616e 206f  )..# 1. Get an o
+00000d30: 7065 6e20 6163 6365 7373 2061 7274 6963  pen access artic
+00000d40: 6c65 2064 6174 6173 6574 2066 726f 6d20  le dataset from 
+00000d50: 7468 6520 4654 5020 7365 7276 6572 0a77  the FTP server.w
+00000d60: 6974 6820 636c 6f73 696e 6728 7265 7175  ith closing(requ
+00000d70: 6573 742e 7572 6c6f 7065 6e28 736f 7572  est.urlopen(sour
+00000d80: 6365 2929 2061 7320 7572 6c3a 0a20 2020  ce)) as url:.   
+00000d90: 2077 6974 6820 7461 7266 696c 652e 6f70   with tarfile.op
+00000da0: 656e 2866 696c 656f 626a 3d75 726c 2c20  en(fileobj=url, 
+00000db0: 6d6f 6465 3d22 723a 677a 2229 2061 7320  mode="r:gz") as 
+00000dc0: 6672 3a0a 2020 2020 2020 2020 6672 2e65  fr:.        fr.e
+00000dd0: 7874 7261 6374 616c 6c28 6465 7374 696e  xtractall(destin
+00000de0: 6174 696f 6e29 0a0a 2320 322e 2050 6172  ation)..# 2. Par
+00000df0: 7365 2074 6865 2066 696c 650a 6669 6c65  se the file.file
+00000e00: 5f70 6174 6820 3d20 6465 7374 696e 6174  _path = destinat
+00000e10: 696f 6e2e 6a6f 696e 7061 7468 2822 504d  ion.joinpath("PM
+00000e20: 4330 3039 7878 7878 7878 2229 2e6a 6f69  C009xxxxxx").joi
+00000e30: 6e70 6174 6828 2250 4d43 3939 3730 3636  npath("PMC997066
+00000e40: 322e 786d 6c22 290a 6675 6c6c 5f74 6578  2.xml").full_tex
+00000e50: 7420 3d20 7061 7273 655f 7075 626d 6564  t = parse_pubmed
+00000e60: 5f78 6d6c 2866 696c 655f 7061 7468 290a  _xml(file_path).
+00000e70: 0a23 2033 2e20 5072 696e 7420 6f75 7420  .# 3. Print out 
+00000e80: 7468 6520 6172 7469 636c 6520 7469 746c  the article titl
+00000e90: 650a 7072 696e 7428 6622 5469 746c 653a  e.print(f"Title:
+00000ea0: 207b 6675 6c6c 5f74 6578 742e 6672 6f6e   {full_text.fron
+00000eb0: 742e 6172 7469 636c 655f 6d65 7461 2e74  t.article_meta.t
+00000ec0: 6974 6c65 5f67 726f 7570 2e61 7274 6963  itle_group.artic
+00000ed0: 6c65 5f74 6974 6c65 2e63 6f6e 7465 6e74  le_title.content
+00000ee0: 5b30 5d7d 2229 0a60 6060 0a0a 4f75 7470  [0]}").```..Outp
+00000ef0: 7574 3a0a 0a60 6060 6261 7368 0a54 6974  ut:..```bash.Tit
+00000f00: 6c65 3a20 4c61 6374 6174 6520 6173 2061  le: Lactate as a
+00000f10: 206d 796f 6b69 6e65 2061 6e64 2065 7865   myokine and exe
+00000f20: 726b 696e 653a 2064 7269 7665 7273 2061  rkine: drivers a
+00000f30: 6e64 2073 6967 6e61 6c73 206f 6620 7068  nd signals of ph
+00000f40: 7973 696f 6c6f 6779 2061 6e64 206d 6574  ysiology and met
+00000f50: 6162 6f6c 6973 6d0a 6060 600a 0a23 2323  abolism.```..###
+00000f60: 2045 7861 6d70 6c65 2032 3a20 4120 5075   Example 2: A Pu
+00000f70: 626d 6564 2062 6173 656c 696e 6520 6369  bmed baseline ci
+00000f80: 7461 7469 6f6e 2066 696c 650a 0a23 2323  tation file..###
+00000f90: 2045 7861 6d70 6c65 2031 3a20 4120 504d   Example 1: A PM
+00000fa0: 4320 4f70 656e 2041 6363 6573 7320 4172  C Open Access Ar
+00000fb0: 7469 636c 650a 0a60 6060 7079 7468 6f6e  ticle..```python
+00000fc0: 0a69 6d70 6f72 7420 677a 6970 0a69 6d70  .import gzip.imp
+00000fd0: 6f72 7420 7572 6c6c 6962 2e72 6571 7565  ort urllib.reque
+00000fe0: 7374 2061 7320 7265 7175 6573 740a 6672  st as request.fr
+00000ff0: 6f6d 2063 6f6e 7465 7874 6c69 6220 696d  om contextlib im
+00001000: 706f 7274 2063 6c6f 7369 6e67 0a66 726f  port closing.fro
+00001010: 6d20 7061 7468 6c69 6220 696d 706f 7274  m pathlib import
+00001020: 2050 6174 680a 0a66 726f 6d20 7075 626d   Path..from pubm
+00001030: 6564 5f74 7970 6573 2069 6d70 6f72 7420  ed_types import 
+00001040: 7061 7273 655f 7075 626d 6564 5f78 6d6c  parse_pubmed_xml
+00001050: 2c20 5075 626d 6564 4172 7469 636c 6553  , PubmedArticleS
+00001060: 6574 0a0a 2320 496e 7075 7420 6669 6c65  et..# Input file
+00001070: 2073 6f75 7263 6520 616e 6420 6f75 7470   source and outp
+00001080: 7574 2066 696c 6520 6465 7374 696e 6174  ut file destinat
+00001090: 696f 6e0a 736f 7572 6365 203d 2022 6674  ion.source = "ft
+000010a0: 703a 2f2f 6674 702e 6e63 6269 2e6e 6c6d  p://ftp.ncbi.nlm
+000010b0: 2e6e 6968 2e67 6f76 2220 2b20 222f 7075  .nih.gov" + "/pu
+000010c0: 626d 6564 2f75 7064 6174 6566 696c 6573  bmed/updatefiles
+000010d0: 2220 2b20 222f 7075 626d 6564 3233 6e31  " + "/pubmed23n1
+000010e0: 3136 382e 786d 6c2e 677a 220a 6465 7374  168.xml.gz".dest
+000010f0: 696e 6174 696f 6e20 3d20 5061 7468 2822  ination = Path("
+00001100: 646f 776e 6c6f 6164 7322 292e 6a6f 696e  downloads").join
+00001110: 7061 7468 2822 7075 626d 6564 3233 6e31  path("pubmed23n1
+00001120: 3136 382e 786d 6c22 290a 6465 7374 696e  168.xml").destin
+00001130: 6174 696f 6e2e 7061 7265 6e74 2e6d 6b64  ation.parent.mkd
+00001140: 6972 2865 7869 7374 5f6f 6b3d 5472 7565  ir(exist_ok=True
+00001150: 290a 0a23 2031 2e20 4765 7420 6120 7075  )..# 1. Get a pu
+00001160: 626d 6564 2063 6974 6174 696f 6e20 6461  bmed citation da
+00001170: 696c 7920 7570 6461 7465 2066 696c 6520  ily update file 
+00001180: 6672 6f6d 2074 6865 2046 5450 2073 6572  from the FTP ser
+00001190: 7665 720a 7769 7468 2063 6c6f 7369 6e67  ver.with closing
+000011a0: 2872 6571 7565 7374 2e75 726c 6f70 656e  (request.urlopen
+000011b0: 2873 6f75 7263 6529 2920 6173 2075 726c  (source)) as url
+000011c0: 3a0a 2020 2020 7769 7468 2067 7a69 702e  :.    with gzip.
+000011d0: 477a 6970 4669 6c65 2866 696c 656f 626a  GzipFile(fileobj
+000011e0: 3d75 726c 2c20 6d6f 6465 3d22 7262 2229  =url, mode="rb")
+000011f0: 2061 7320 6672 3a0a 2020 2020 2020 2020   as fr:.        
+00001200: 7769 7468 206f 7065 6e28 6465 7374 696e  with open(destin
+00001210: 6174 696f 6e2c 206d 6f64 653d 2277 6222  ation, mode="wb"
+00001220: 2920 6173 2066 773a 0a20 2020 2020 2020  ) as fw:.       
+00001230: 2020 2020 2066 772e 7772 6974 6528 6672       fw.write(fr
+00001240: 2e72 6561 6428 2929 0a0a 2320 322e 2050  .read())..# 2. P
+00001250: 6172 7365 2074 6865 2066 696c 650a 6172  arse the file.ar
+00001260: 7469 636c 655f 7365 7420 3d20 7061 7273  ticle_set = pars
+00001270: 655f 7075 626d 6564 5f78 6d6c 2864 6573  e_pubmed_xml(des
+00001280: 7469 6e61 7469 6f6e 290a 6173 7365 7274  tination).assert
+00001290: 2069 7369 6e73 7461 6e63 6528 6172 7469   isinstance(arti
+000012a0: 636c 655f 7365 742c 2050 7562 6d65 6441  cle_set, PubmedA
+000012b0: 7274 6963 6c65 5365 7429 0a0a 2320 332e  rticleSet)..# 3.
+000012c0: 2047 6574 2074 6865 206e 756d 6265 7220   Get the number 
+000012d0: 6f66 2063 6974 6174 696f 6e73 2069 6e20  of citations in 
+000012e0: 7468 6520 6669 6c65 0a70 7269 6e74 2866  the file.print(f
+000012f0: 224e 756d 6265 7220 6f66 2063 6974 6174  "Number of citat
+00001300: 696f 6e73 3a20 7b6c 656e 2861 7274 6963  ions: {len(artic
+00001310: 6c65 5f73 6574 2e70 7562 6d65 645f 6172  le_set.pubmed_ar
+00001320: 7469 636c 6529 7d22 290a 7072 696e 7428  ticle)}").print(
+00001330: 6622 7b61 7274 6963 6c65 5f73 6574 2e70  f"{article_set.p
+00001340: 7562 6d65 645f 6172 7469 636c 655b 305d  ubmed_article[0]
+00001350: 2e6d 6564 6c69 6e65 5f63 6974 6174 696f  .medline_citatio
+00001360: 6e2e 6172 7469 636c 652e 6172 7469 636c  n.article.articl
+00001370: 655f 7469 746c 652e 636f 6e74 656e 745b  e_title.content[
+00001380: 305d 7d22 290a 6060 600a 0a4f 7574 7075  0]}").```..Outpu
+00001390: 743a 0a0a 6060 6062 6173 680a 4e75 6d62  t:..```bash.Numb
+000013a0: 6572 206f 6620 6369 7461 7469 6f6e 733a  er of citations:
+000013b0: 2032 3534 330a 4120 5061 7465 6e74 2061   2543.A Patent a
+000013c0: 6e64 2050 6174 7465 726e 204d 6f74 6865  nd Pattern Mothe
+000013d0: 722e 0a60 6060 0a0a 2323 2046 4151 0a0a  r..```..## FAQ..
+000013e0: 2323 2320 5768 7920 646f 6573 2069 7420  ### Why does it 
+000013f0: 7461 6b65 2073 6f20 6c6f 6e67 2074 6f20  take so long to 
+00001400: 7061 7273 6520 6120 7075 626d 6564 2063  parse a pubmed c
+00001410: 6974 6174 696f 6e20 7365 740a 0a54 6865  itation set..The
+00001420: 7265 2069 7320 6120 6c6f 7420 6f66 2064  re is a lot of d
+00001430: 6174 612c 2061 6e64 2074 6865 2073 6368  ata, and the sch
+00001440: 656d 6120 6973 2064 6565 7020 616e 6420  ema is deep and 
+00001450: 636f 6d70 6c65 782e 0a0a 2323 2320 5768  complex...### Wh
+00001460: 7920 6172 6520 7468 6520 7265 7475 726e  y are the return
+00001470: 2073 7472 7563 7475 7265 7320 736f 2063   structures so c
+00001480: 6f6d 706c 6963 6174 6564 3f0a 0a54 6865  omplicated?..The
+00001490: 2072 6574 7572 6e20 7374 7275 6374 7572   return structur
+000014a0: 6573 2061 7265 2061 2064 6972 6563 7420  es are a direct 
+000014b0: 7265 666c 6563 7469 6f6e 206f 6620 7468  reflection of th
+000014c0: 6520 584d 4c20 666f 726d 6174 2064 6566  e XML format def
+000014d0: 696e 6564 2062 7920 7468 6520 4e4c 4d2e  ined by the NLM.
+000014e0: 2049 6e0a 7468 6520 6675 7475 7265 2073   In.the future s
+000014f0: 6f6d 6520 7574 696c 6974 7920 636c 6173  ome utility clas
+00001500: 7365 7320 6d69 6768 7420 6265 206d 6164  ses might be mad
+00001510: 6520 666f 7220 636f 6d6d 6f6e 2063 6f6d  e for common com
+00001520: 706f 6e65 6e74 7320 2874 6974 6c65 2c20  ponents (title, 
+00001530: 6175 7468 6f72 732c 0a65 7463 292c 2062  authors,.etc), b
+00001540: 7574 2066 6f72 206e 6f77 2074 6869 7320  ut for now this 
+00001550: 6973 2069 6e74 656e 6465 6420 746f 2062  is intended to b
+00001560: 6520 616e 2075 6e62 6961 7365 6420 7761  e an unbiased wa
+00001570: 7920 6f66 2070 6172 7369 6e67 2074 6865  y of parsing the
+00001580: 2058 4d4c 2e0a 0a                         XML...
```

