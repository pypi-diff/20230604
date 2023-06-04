# Comparing `tmp/pubmed_types-0.1.0.tar.gz` & `tmp/pubmed_types-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pubmed_types-0.1.0.tar", max compression
+gzip compressed data, was "pubmed_types-0.1.1.tar", max compression
```

## Comparing `pubmed_types-0.1.0.tar` & `pubmed_types-0.1.1.tar`

### file list

```diff
@@ -1,672 +1,673 @@
--rw-r--r--   0        0        0     1072 2023-05-25 16:03:32.757838 pubmed_types-0.1.0/LICENSE
--rw-r--r--   0        0        0      537 2023-06-04 03:06:39.303013 pubmed_types-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      483 2023-06-04 02:35:11.351659 pubmed_types-0.1.0/src/pubmed_types/__init__.py
--rw-r--r--   0        0        0    24766 2023-06-03 02:43:58.380623 pubmed_types-0.1.0/src/pubmed_types/models/__init__.py
--rw-r--r--   0        0        0     7420 2023-06-03 02:44:01.924575 pubmed_types-0.1.0/src/pubmed_types/models/abbrev_journal_title.py
--rw-r--r--   0        0        0      610 2023-06-03 02:44:02.860562 pubmed_types-0.1.0/src/pubmed_types/models/abstract_1.py
--rw-r--r--   0        0        0     1645 2023-06-03 02:44:02.572566 pubmed_types-0.1.0/src/pubmed_types/models/abstract_text.py
--rw-r--r--   0        0        0      229 2023-06-03 02:44:02.832563 pubmed_types-0.1.0/src/pubmed_types/models/abstract_text_nlm_category.py
--rw-r--r--   0        0        0  1064015 2023-06-03 02:44:01.912575 pubmed_types-0.1.0/src/pubmed_types/models/access_date.py
--rw-r--r--   0        0        0      342 2023-06-03 02:44:02.576566 pubmed_types-0.1.0/src/pubmed_types/models/accession_number_list.py
--rw-r--r--   0        0        0      962 2023-06-03 02:44:02.576566 pubmed_types-0.1.0/src/pubmed_types/models/affiliation.py
--rw-r--r--   0        0        0      588 2023-06-03 02:44:02.576566 pubmed_types-0.1.0/src/pubmed_types/models/affiliation_info.py
--rw-r--r--   0        0        0     1373 2023-06-03 02:44:01.924575 pubmed_types-0.1.0/src/pubmed_types/models/alt_text.py
--rw-r--r--   0        0        0     8831 2023-06-03 02:44:01.944575 pubmed_types-0.1.0/src/pubmed_types/models/app.py
--rw-r--r--   0        0        0     8786 2023-06-03 02:44:01.960574 pubmed_types-0.1.0/src/pubmed_types/models/app_group.py
--rw-r--r--   0        0        0      419 2023-06-03 02:18:03.813928 pubmed_types-0.1.0/src/pubmed_types/models/archive_copy_source.py
--rw-r--r--   0        0        0      108 2023-06-03 02:44:02.776564 pubmed_types-0.1.0/src/pubmed_types/models/array_orientation.py
--rw-r--r--   0        0        0     3079 2023-06-03 02:44:02.864562 pubmed_types-0.1.0/src/pubmed_types/models/article_1.py
--rw-r--r--   0        0        0     2649 2023-06-03 02:44:02.876562 pubmed_types-0.1.0/src/pubmed_types/models/article_2.py
--rw-r--r--   0        0        0     1202 2023-06-03 02:44:01.960574 pubmed_types-0.1.0/src/pubmed_types/models/article_categories.py
--rw-r--r--   0        0        0      878 2023-06-03 02:44:02.576566 pubmed_types-0.1.0/src/pubmed_types/models/article_date.py
--rw-r--r--   0        0        0      369 2023-06-03 02:44:02.824563 pubmed_types-0.1.0/src/pubmed_types/models/article_dtd_version.py
--rw-r--r--   0        0        0     1423 2023-06-03 02:44:01.964574 pubmed_types-0.1.0/src/pubmed_types/models/article_id.py
--rw-r--r--   0        0        0      511 2023-06-03 02:44:02.876562 pubmed_types-0.1.0/src/pubmed_types/models/article_id_1.py
--rw-r--r--   0        0        0      303 2023-06-03 02:44:02.848563 pubmed_types-0.1.0/src/pubmed_types/models/article_id_id_type.py
--rw-r--r--   0        0        0      368 2023-06-03 02:44:02.580566 pubmed_types-0.1.0/src/pubmed_types/models/article_id_list.py
--rw-r--r--   0        0        0     9515 2023-06-03 02:44:01.980574 pubmed_types-0.1.0/src/pubmed_types/models/article_meta.py
--rw-r--r--   0        0        0      242 2023-06-03 02:44:02.828563 pubmed_types-0.1.0/src/pubmed_types/models/article_pub_model.py
--rw-r--r--   0        0        0      353 2023-06-03 02:18:03.769929 pubmed_types-0.1.0/src/pubmed_types/models/article_set.py
--rw-r--r--   0        0        0     1495 2023-06-03 02:44:02.880562 pubmed_types-0.1.0/src/pubmed_types/models/article_title_1.py
--rw-r--r--   0        0        0     3823 2023-06-03 02:44:01.988574 pubmed_types-0.1.0/src/pubmed_types/models/article_version.py
--rw-r--r--   0        0        0      827 2023-06-03 02:44:01.992574 pubmed_types-0.1.0/src/pubmed_types/models/article_version_alternatives.py
--rw-r--r--   0        0        0     1938 2023-06-03 02:44:02.580566 pubmed_types-0.1.0/src/pubmed_types/models/author.py
--rw-r--r--   0        0        0       80 2023-06-03 02:44:02.836563 pubmed_types-0.1.0/src/pubmed_types/models/author_equal_contrib.py
--rw-r--r--   0        0        0      838 2023-06-03 02:44:02.584566 pubmed_types-0.1.0/src/pubmed_types/models/author_list.py
--rw-r--r--   0        0        0       82 2023-06-03 02:44:02.832563 pubmed_types-0.1.0/src/pubmed_types/models/author_list_complete_yn.py
--rw-r--r--   0        0        0      100 2023-06-03 02:44:02.832563 pubmed_types-0.1.0/src/pubmed_types/models/author_list_type.py
--rw-r--r--   0        0        0     1720 2023-06-03 02:44:02.000574 pubmed_types-0.1.0/src/pubmed_types/models/author_notes.py
--rw-r--r--   0        0        0       75 2023-06-03 02:44:02.836563 pubmed_types-0.1.0/src/pubmed_types/models/author_valid_yn.py
--rw-r--r--   0        0        0     2449 2023-06-03 02:44:02.004574 pubmed_types-0.1.0/src/pubmed_types/models/award_desc.py
--rw-r--r--   0        0        0     4315 2023-06-03 02:44:02.012574 pubmed_types-0.1.0/src/pubmed_types/models/award_group.py
--rw-r--r--   0        0        0     2442 2023-06-03 02:44:02.016574 pubmed_types-0.1.0/src/pubmed_types/models/award_name.py
--rw-r--r--   0        0        0     2079 2023-06-03 02:44:02.020574 pubmed_types-0.1.0/src/pubmed_types/models/back.py
--rw-r--r--   0        0        0      765 2023-06-03 02:44:02.584566 pubmed_types-0.1.0/src/pubmed_types/models/beginning_date.py
--rw-r--r--   0        0        0     7356 2023-06-03 02:44:02.032574 pubmed_types-0.1.0/src/pubmed_types/models/body.py
--rw-r--r--   0        0        0       78 2023-06-03 02:44:02.768564 pubmed_types-0.1.0/src/pubmed_types/models/bold_toggle.py
--rw-r--r--   0        0        0     3125 2023-06-03 02:44:02.588566 pubmed_types-0.1.0/src/pubmed_types/models/book.py
--rw-r--r--   0        0        0     4185 2023-06-03 02:44:02.560566 pubmed_types-0.1.0/src/pubmed_types/models/book_document.py
--rw-r--r--   0        0        0      587 2023-06-03 02:44:02.556566 pubmed_types-0.1.0/src/pubmed_types/models/book_document_set.py
--rw-r--r--   0        0        0     1444 2023-06-03 02:44:02.592566 pubmed_types-0.1.0/src/pubmed_types/models/book_title.py
--rw-r--r--   0        0        0      112 2023-06-03 02:44:02.784563 pubmed_types-0.1.0/src/pubmed_types/models/boxed_text_orientation.py
--rw-r--r--   0        0        0      149 2023-06-03 02:44:02.788563 pubmed_types-0.1.0/src/pubmed_types/models/boxed_text_position.py
--rw-r--r--   0        0        0      529 2023-06-03 02:44:02.032574 pubmed_types-0.1.0/src/pubmed_types/models/break_mod.py
--rw-r--r--   0        0        0      117 2023-06-03 02:44:02.788563 pubmed_types-0.1.0/src/pubmed_types/models/chem_struct_wrap_orientation.py
--rw-r--r--   0        0        0      154 2023-06-03 02:44:02.788563 pubmed_types-0.1.0/src/pubmed_types/models/chem_struct_wrap_position.py
--rw-r--r--   0        0        0      592 2023-06-03 02:44:02.592566 pubmed_types-0.1.0/src/pubmed_types/models/chemical.py
--rw-r--r--   0        0        0      356 2023-06-03 02:44:02.592566 pubmed_types-0.1.0/src/pubmed_types/models/chemical_list.py
--rw-r--r--   0        0        0     1065 2023-06-03 02:44:02.592566 pubmed_types-0.1.0/src/pubmed_types/models/citation.py
--rw-r--r--   0        0        0     1344 2023-06-03 02:44:02.036574 pubmed_types-0.1.0/src/pubmed_types/models/city.py
--rw-r--r--   0        0        0       82 2023-06-03 02:44:02.788563 pubmed_types-0.1.0/src/pubmed_types/models/code_executable.py
--rw-r--r--   0        0        0      107 2023-06-03 02:44:02.788563 pubmed_types-0.1.0/src/pubmed_types/models/code_orientation.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.788563 pubmed_types-0.1.0/src/pubmed_types/models/code_position.py
--rw-r--r--   0        0        0      963 2023-06-03 02:44:02.596566 pubmed_types-0.1.0/src/pubmed_types/models/coi_statement.py
--rw-r--r--   0        0        0     1574 2023-06-03 02:44:02.036574 pubmed_types-0.1.0/src/pubmed_types/models/col.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.804563 pubmed_types-0.1.0/src/pubmed_types/models/col_align.py
--rw-r--r--   0        0        0      133 2023-06-03 02:44:02.804563 pubmed_types-0.1.0/src/pubmed_types/models/col_valign.py
--rw-r--r--   0        0        0     1765 2023-06-03 02:44:02.040573 pubmed_types-0.1.0/src/pubmed_types/models/colgroup.py
--rw-r--r--   0        0        0      153 2023-06-03 02:44:02.808563 pubmed_types-0.1.0/src/pubmed_types/models/colgroup_align.py
--rw-r--r--   0        0        0      138 2023-06-03 02:44:02.808563 pubmed_types-0.1.0/src/pubmed_types/models/colgroup_valign.py
--rw-r--r--   0        0        0     1450 2023-06-03 02:44:02.596566 pubmed_types-0.1.0/src/pubmed_types/models/collection_title.py
--rw-r--r--   0        0        0      965 2023-06-03 02:44:02.600566 pubmed_types-0.1.0/src/pubmed_types/models/collective_name.py
--rw-r--r--   0        0        0      934 2023-06-03 02:44:02.600566 pubmed_types-0.1.0/src/pubmed_types/models/comments_corrections.py
--rw-r--r--   0        0        0      424 2023-06-03 02:44:02.600566 pubmed_types-0.1.0/src/pubmed_types/models/comments_corrections_list.py
--rw-r--r--   0        0        0     1025 2023-06-03 02:44:02.840563 pubmed_types-0.1.0/src/pubmed_types/models/comments_corrections_ref_type.py
--rw-r--r--   0        0        0     7391 2023-06-03 02:44:02.052573 pubmed_types-0.1.0/src/pubmed_types/models/conf_num.py
--rw-r--r--   0        0        0     7394 2023-06-03 02:44:02.064573 pubmed_types-0.1.0/src/pubmed_types/models/conf_theme.py
--rw-r--r--   0        0        0     4292 2023-06-03 02:44:02.068573 pubmed_types-0.1.0/src/pubmed_types/models/conference.py
--rw-r--r--   0        0        0       82 2023-06-03 02:44:02.780563 pubmed_types-0.1.0/src/pubmed_types/models/contrib_corresp.py
--rw-r--r--   0        0        0       83 2023-06-03 02:44:02.784563 pubmed_types-0.1.0/src/pubmed_types/models/contrib_deceased.py
--rw-r--r--   0        0        0       87 2023-06-03 02:44:02.784563 pubmed_types-0.1.0/src/pubmed_types/models/contrib_equal_contrib.py
--rw-r--r--   0        0        0     1940 2023-06-03 02:44:02.072573 pubmed_types-0.1.0/src/pubmed_types/models/contrib_id.py
--rw-r--r--   0        0        0       98 2023-06-03 02:44:02.784563 pubmed_types-0.1.0/src/pubmed_types/models/contrib_id_authenticated.py
--rw-r--r--   0        0        0     1889 2023-06-03 02:44:02.076573 pubmed_types-0.1.0/src/pubmed_types/models/contributed_resource_group.py
--rw-r--r--   0        0        0      768 2023-06-03 02:44:02.600566 pubmed_types-0.1.0/src/pubmed_types/models/contribution_date.py
--rw-r--r--   0        0        0     1083 2023-06-03 02:44:02.080573 pubmed_types-0.1.0/src/pubmed_types/models/copyright_year.py
--rw-r--r--   0        0        0     8856 2023-06-03 02:44:02.092573 pubmed_types-0.1.0/src/pubmed_types/models/corresp.py
--rw-r--r--   0        0        0      871 2023-06-03 02:44:02.096573 pubmed_types-0.1.0/src/pubmed_types/models/count.py
--rw-r--r--   0        0        0     1907 2023-06-03 02:44:02.100573 pubmed_types-0.1.0/src/pubmed_types/models/counts.py
--rw-r--r--   0        0        0     3702 2023-06-03 02:44:02.104573 pubmed_types-0.1.0/src/pubmed_types/models/custom_meta.py
--rw-r--r--   0        0        0     1389 2023-06-03 02:44:02.108573 pubmed_types-0.1.0/src/pubmed_types/models/custom_meta_group.py
--rw-r--r--   0        0        0      579 2023-06-03 02:44:02.604566 pubmed_types-0.1.0/src/pubmed_types/models/data_bank.py
--rw-r--r--   0        0        0      644 2023-06-03 02:44:02.604566 pubmed_types-0.1.0/src/pubmed_types/models/data_bank_list.py
--rw-r--r--   0        0        0       84 2023-06-03 02:44:02.836563 pubmed_types-0.1.0/src/pubmed_types/models/data_bank_list_complete_yn.py
--rw-r--r--   0        0        0      672 2023-06-03 02:44:02.604566 pubmed_types-0.1.0/src/pubmed_types/models/date_completed.py
--rw-r--r--   0        0        0      670 2023-06-03 02:44:02.604566 pubmed_types-0.1.0/src/pubmed_types/models/date_revised.py
--rw-r--r--   0        0        0     1328 2023-06-03 02:44:02.108573 pubmed_types-0.1.0/src/pubmed_types/models/day.py
--rw-r--r--   0        0        0      338 2023-06-03 02:44:02.564566 pubmed_types-0.1.0/src/pubmed_types/models/delete_citation.py
--rw-r--r--   0        0        0      309 2023-06-03 02:44:02.564566 pubmed_types-0.1.0/src/pubmed_types/models/delete_document.py
--rw-r--r--   0        0        0      948 2023-06-03 02:44:02.608566 pubmed_types-0.1.0/src/pubmed_types/models/descriptor_name.py
--rw-r--r--   0        0        0       88 2023-06-03 02:44:02.840563 pubmed_types-0.1.0/src/pubmed_types/models/descriptor_name_major_topic_yn.py
--rw-r--r--   0        0        0       86 2023-06-03 02:44:02.840563 pubmed_types-0.1.0/src/pubmed_types/models/descriptor_name_type.py
--rw-r--r--   0        0        0      331 2023-06-03 02:44:02.884562 pubmed_types-0.1.0/src/pubmed_types/models/disp_formula_1.py
--rw-r--r--   0        0        0     1217 2023-06-03 02:44:02.112573 pubmed_types-0.1.0/src/pubmed_types/models/elocation_id.py
--rw-r--r--   0        0        0      809 2023-06-03 02:44:02.884562 pubmed_types-0.1.0/src/pubmed_types/models/elocation_id_1.py
--rw-r--r--   0        0        0       88 2023-06-03 02:44:02.832563 pubmed_types-0.1.0/src/pubmed_types/models/elocation_id_eid_type.py
--rw-r--r--   0        0        0       80 2023-06-03 02:44:02.832563 pubmed_types-0.1.0/src/pubmed_types/models/elocation_id_valid_yn.py
--rw-r--r--   0        0        0      762 2023-06-03 02:44:02.608566 pubmed_types-0.1.0/src/pubmed_types/models/ending_date.py
--rw-r--r--   0        0        0      704 2023-06-03 02:44:02.116572 pubmed_types-0.1.0/src/pubmed_types/models/equation_count.py
--rw-r--r--   0        0        0     1328 2023-06-03 02:44:02.116572 pubmed_types-0.1.0/src/pubmed_types/models/era.py
--rw-r--r--   0        0        0     3816 2023-06-03 02:44:02.124572 pubmed_types-0.1.0/src/pubmed_types/models/event.py
--rw-r--r--   0        0        0     3116 2023-06-03 02:44:02.132572 pubmed_types-0.1.0/src/pubmed_types/models/event_desc.py
--rw-r--r--   0        0        0     3131 2023-06-03 02:44:02.136572 pubmed_types-0.1.0/src/pubmed_types/models/extended_by.py
--rw-r--r--   0        0        0      692 2023-06-03 02:44:02.140572 pubmed_types-0.1.0/src/pubmed_types/models/fig_count.py
--rw-r--r--   0        0        0      111 2023-06-03 02:44:02.796563 pubmed_types-0.1.0/src/pubmed_types/models/fig_group_orientation.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.796563 pubmed_types-0.1.0/src/pubmed_types/models/fig_group_position.py
--rw-r--r--   0        0        0      106 2023-06-03 02:44:02.792563 pubmed_types-0.1.0/src/pubmed_types/models/fig_orientation.py
--rw-r--r--   0        0        0      143 2023-06-03 02:44:02.792563 pubmed_types-0.1.0/src/pubmed_types/models/fig_position.py
--rw-r--r--   0        0        0      467 2023-06-03 02:18:03.781929 pubmed_types-0.1.0/src/pubmed_types/models/first_name.py
--rw-r--r--   0        0        0       78 2023-06-03 02:18:04.049925 pubmed_types-0.1.0/src/pubmed_types/models/first_name_empty_yn.py
--rw-r--r--   0        0        0      458 2023-06-03 02:18:03.777929 pubmed_types-0.1.0/src/pubmed_types/models/first_page.py
--rw-r--r--   0        0        0      112 2023-06-03 02:18:04.045925 pubmed_types-0.1.0/src/pubmed_types/models/first_page_lzero.py
--rw-r--r--   0        0        0     2865 2023-06-03 02:44:02.144572 pubmed_types-0.1.0/src/pubmed_types/models/floats_group.py
--rw-r--r--   0        0        0     1461 2023-06-03 02:44:02.148572 pubmed_types-0.1.0/src/pubmed_types/models/fpage.py
--rw-r--r--   0        0        0     2105 2023-06-03 02:44:02.156572 pubmed_types-0.1.0/src/pubmed_types/models/front.py
--rw-r--r--   0        0        0     9514 2023-06-03 02:44:02.168572 pubmed_types-0.1.0/src/pubmed_types/models/front_stub.py
--rw-r--r--   0        0        0     1657 2023-06-03 02:44:02.168572 pubmed_types-0.1.0/src/pubmed_types/models/funding_group.py
--rw-r--r--   0        0        0     9232 2023-06-03 02:44:02.184572 pubmed_types-0.1.0/src/pubmed_types/models/funding_statement.py
--rw-r--r--   0        0        0      327 2023-06-03 02:44:02.608566 pubmed_types-0.1.0/src/pubmed_types/models/gene_symbol_list.py
--rw-r--r--   0        0        0      465 2023-06-03 02:44:02.612566 pubmed_types-0.1.0/src/pubmed_types/models/general_note.py
--rw-r--r--   0        0        0      152 2023-06-03 02:44:02.844563 pubmed_types-0.1.0/src/pubmed_types/models/general_note_owner.py
--rw-r--r--   0        0        0     1866 2023-06-03 02:44:02.184572 pubmed_types-0.1.0/src/pubmed_types/models/glyph_data.py
--rw-r--r--   0        0        0      728 2023-06-03 02:44:02.188572 pubmed_types-0.1.0/src/pubmed_types/models/glyph_ref.py
--rw-r--r--   0        0        0      806 2023-06-03 02:44:02.612566 pubmed_types-0.1.0/src/pubmed_types/models/grant.py
--rw-r--r--   0        0        0      611 2023-06-03 02:44:02.612566 pubmed_types-0.1.0/src/pubmed_types/models/grant_list.py
--rw-r--r--   0        0        0       81 2023-06-03 02:44:02.836563 pubmed_types-0.1.0/src/pubmed_types/models/grant_list_complete_yn.py
--rw-r--r--   0        0        0      110 2023-06-03 02:44:02.792563 pubmed_types-0.1.0/src/pubmed_types/models/graphic_orientation.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.792563 pubmed_types-0.1.0/src/pubmed_types/models/graphic_position.py
--rw-r--r--   0        0        0      551 2023-06-03 02:18:03.805928 pubmed_types-0.1.0/src/pubmed_types/models/group.py
--rw-r--r--   0        0        0      338 2023-06-03 02:18:03.805928 pubmed_types-0.1.0/src/pubmed_types/models/group_list.py
--rw-r--r--   0        0        0      425 2023-06-03 02:44:02.888562 pubmed_types-0.1.0/src/pubmed_types/models/history_1.py
--rw-r--r--   0        0        0     7177 2023-06-03 02:44:02.908562 pubmed_types-0.1.0/src/pubmed_types/models/history_2.py
--rw-r--r--   0        0        0      528 2023-06-03 02:44:02.192571 pubmed_types-0.1.0/src/pubmed_types/models/hr.py
--rw-r--r--   0        0        0     3870 2023-06-03 02:18:03.805928 pubmed_types-0.1.0/src/pubmed_types/models/i.py
--rw-r--r--   0        0        0      426 2023-06-03 02:44:02.616566 pubmed_types-0.1.0/src/pubmed_types/models/identifier.py
--rw-r--r--   0        0        0      718 2023-06-03 02:44:02.192571 pubmed_types-0.1.0/src/pubmed_types/models/index_term_range_end.py
--rw-r--r--   0        0        0     1475 2023-06-03 02:18:03.809928 pubmed_types-0.1.0/src/pubmed_types/models/individual_name.py
--rw-r--r--   0        0        0     2029 2023-06-03 02:44:02.200571 pubmed_types-0.1.0/src/pubmed_types/models/institution_id.py
--rw-r--r--   0        0        0     1537 2023-06-03 02:44:02.616566 pubmed_types-0.1.0/src/pubmed_types/models/investigator.py
--rw-r--r--   0        0        0      380 2023-06-03 02:44:02.616566 pubmed_types-0.1.0/src/pubmed_types/models/investigator_list.py
--rw-r--r--   0        0        0       81 2023-06-03 02:44:02.844563 pubmed_types-0.1.0/src/pubmed_types/models/investigator_valid_yn.py
--rw-r--r--   0        0        0      515 2023-06-03 02:44:02.908562 pubmed_types-0.1.0/src/pubmed_types/models/issn_1.py
--rw-r--r--   0        0        0      100 2023-06-03 02:44:02.828563 pubmed_types-0.1.0/src/pubmed_types/models/issn_issn_type.py
--rw-r--r--   0        0        0     3124 2023-06-03 02:44:02.204571 pubmed_types-0.1.0/src/pubmed_types/models/issue_id.py
--rw-r--r--   0        0        0     7395 2023-06-03 02:44:02.216571 pubmed_types-0.1.0/src/pubmed_types/models/issue_sponsor.py
--rw-r--r--   0        0        0     7400 2023-06-03 02:44:02.228571 pubmed_types-0.1.0/src/pubmed_types/models/issue_subtitle.py
--rw-r--r--   0        0        0     1874 2023-06-03 02:44:02.228571 pubmed_types-0.1.0/src/pubmed_types/models/issue_title_group.py
--rw-r--r--   0        0        0       80 2023-06-03 02:44:02.768564 pubmed_types-0.1.0/src/pubmed_types/models/italic_toggle.py
--rw-r--r--   0        0        0      508 2023-06-03 02:44:02.620566 pubmed_types-0.1.0/src/pubmed_types/models/item_list.py
--rw-r--r--   0        0        0      873 2023-06-03 02:44:02.620566 pubmed_types-0.1.0/src/pubmed_types/models/journal.py
--rw-r--r--   0        0        0     1543 2023-06-03 02:44:02.232571 pubmed_types-0.1.0/src/pubmed_types/models/journal_id.py
--rw-r--r--   0        0        0      942 2023-06-03 02:44:02.620566 pubmed_types-0.1.0/src/pubmed_types/models/journal_issue.py
--rw-r--r--   0        0        0      107 2023-06-03 02:44:02.832563 pubmed_types-0.1.0/src/pubmed_types/models/journal_issue_cited_medium.py
--rw-r--r--   0        0        0     2752 2023-06-03 02:44:02.236571 pubmed_types-0.1.0/src/pubmed_types/models/journal_meta.py
--rw-r--r--   0        0        0     7406 2023-06-03 02:44:02.252570 pubmed_types-0.1.0/src/pubmed_types/models/journal_subtitle.py
--rw-r--r--   0        0        0     7404 2023-06-03 02:44:02.264570 pubmed_types-0.1.0/src/pubmed_types/models/journal_title.py
--rw-r--r--   0        0        0     1683 2023-06-03 02:44:02.268570 pubmed_types-0.1.0/src/pubmed_types/models/journal_title_group.py
--rw-r--r--   0        0        0     1342 2023-06-03 02:44:02.624565 pubmed_types-0.1.0/src/pubmed_types/models/keyword.py
--rw-r--r--   0        0        0      601 2023-06-03 02:44:02.624565 pubmed_types-0.1.0/src/pubmed_types/models/keyword_list.py
--rw-r--r--   0        0        0      184 2023-06-03 02:44:02.844563 pubmed_types-0.1.0/src/pubmed_types/models/keyword_list_owner.py
--rw-r--r--   0        0        0       81 2023-06-03 02:44:02.844563 pubmed_types-0.1.0/src/pubmed_types/models/keyword_major_topic_yn.py
--rw-r--r--   0        0        0      460 2023-06-03 02:44:02.624565 pubmed_types-0.1.0/src/pubmed_types/models/location_label.py
--rw-r--r--   0        0        0      205 2023-06-03 02:44:02.852563 pubmed_types-0.1.0/src/pubmed_types/models/location_label_type.py
--rw-r--r--   0        0        0     1338 2023-06-03 02:44:02.272570 pubmed_types-0.1.0/src/pubmed_types/models/lpage.py
--rw-r--r--   0        0        0      108 2023-06-03 02:44:02.792563 pubmed_types-0.1.0/src/pubmed_types/models/media_orientation.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.796563 pubmed_types-0.1.0/src/pubmed_types/models/media_position.py
--rw-r--r--   0        0        0     5578 2023-06-03 02:44:02.568566 pubmed_types-0.1.0/src/pubmed_types/models/medline_citation.py
--rw-r--r--   0        0        0      178 2023-06-03 02:44:02.828563 pubmed_types-0.1.0/src/pubmed_types/models/medline_citation_owner.py
--rw-r--r--   0        0        0      284 2023-06-03 02:44:02.828563 pubmed_types-0.1.0/src/pubmed_types/models/medline_citation_status.py
--rw-r--r--   0        0        0      813 2023-06-03 02:44:02.624565 pubmed_types-0.1.0/src/pubmed_types/models/medline_journal_info.py
--rw-r--r--   0        0        0      618 2023-06-03 02:44:02.628565 pubmed_types-0.1.0/src/pubmed_types/models/mesh_heading.py
--rw-r--r--   0        0        0      376 2023-06-03 02:44:02.628565 pubmed_types-0.1.0/src/pubmed_types/models/mesh_heading_list.py
--rw-r--r--   0        0        0     6803 2023-06-03 02:44:02.284570 pubmed_types-0.1.0/src/pubmed_types/models/meta_name.py
--rw-r--r--   0        0        0     6806 2023-06-03 02:44:02.296570 pubmed_types-0.1.0/src/pubmed_types/models/meta_value.py
--rw-r--r--   0        0        0     1408 2023-06-03 02:44:02.300570 pubmed_types-0.1.0/src/pubmed_types/models/milestone_end.py
--rw-r--r--   0        0        0     1414 2023-06-03 02:44:02.304570 pubmed_types-0.1.0/src/pubmed_types/models/milestone_start.py
--rw-r--r--   0        0        0       83 2023-06-03 02:44:02.772564 pubmed_types-0.1.0/src/pubmed_types/models/monospace_toggle.py
--rw-r--r--   0        0        0     1334 2023-06-03 02:44:02.304570 pubmed_types-0.1.0/src/pubmed_types/models/month.py
--rw-r--r--   0        0        0      153 2023-06-03 02:44:02.784563 pubmed_types-0.1.0/src/pubmed_types/models/name_name_style.py
--rw-r--r--   0        0        0      423 2023-06-03 02:44:02.628565 pubmed_types-0.1.0/src/pubmed_types/models/name_of_substance.py
--rw-r--r--   0        0        0     1422 2023-06-03 02:44:02.308570 pubmed_types-0.1.0/src/pubmed_types/models/object_id.py
--rw-r--r--   0        0        0      354 2023-06-03 02:44:02.632565 pubmed_types-0.1.0/src/pubmed_types/models/object_list.py
--rw-r--r--   0        0        0      497 2023-06-03 02:44:02.632565 pubmed_types-0.1.0/src/pubmed_types/models/object_mod.py
--rw-r--r--   0        0        0       81 2023-06-03 02:44:02.820563 pubmed_types-0.1.0/src/pubmed_types/models/option_correct.py
--rw-r--r--   0        0        0       15 2023-06-03 02:17:59.961981 pubmed_types-0.1.0/src/pubmed_types/models/org/__init__.py
--rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.0/src/pubmed_types/models/org/niso/__init__.py
--rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.0/src/pubmed_types/models/org/niso/schemas/__init__.py
--rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.0/src/pubmed_types/models/org/niso/schemas/ali/__init__.py
--rw-r--r--   0        0        0      124 2023-06-03 02:43:58.380623 pubmed_types-0.1.0/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/__init__.py
--rw-r--r--   0        0        0      631 2023-06-03 02:44:02.552566 pubmed_types-0.1.0/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/free_to_read.py
--rw-r--r--   0        0        0      578 2023-06-03 02:44:02.552566 pubmed_types-0.1.0/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/license_ref.py
--rw-r--r--   0        0        0       15 2023-06-03 02:17:59.961981 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/__init__.py
--rw-r--r--   0        0        0       15 2023-06-03 02:17:59.989981 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/__init__.py
--rw-r--r--   0        0        0       15 2023-06-03 02:17:59.989981 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/__init__.py
--rw-r--r--   0        0        0    18558 2023-06-03 02:43:58.344624 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/__init__.py
--rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.116600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/abs.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.132599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/and_mod.py
--rw-r--r--   0        0        0     2149 2023-06-03 02:44:00.364596 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/annotation.py
--rw-r--r--   0        0        0     1582 2023-06-03 02:44:00.148599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/approx.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.184599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccos.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.184599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccosh.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.184599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccot.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.188599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccoth.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.188599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccsc.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.188599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccsch.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.188599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arcsec.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.188599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arcsech.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.180599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arcsin.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.192599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arcsinh.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.184599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arctan.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.192599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arctanh.py
--rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.120600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arg.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.164599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/card.py
--rw-r--r--   0        0        0      466 2023-06-03 02:44:00.160599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cartesianproduct.py
--rw-r--r--   0        0        0     1737 2023-06-03 02:44:00.092600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cbytes.py
--rw-r--r--   0        0        0     1584 2023-06-03 02:44:00.128600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ceiling.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.096600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/codomain.py
--rw-r--r--   0        0        0      168 2023-06-03 02:44:00.224598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/columnalignstyle.py
--rw-r--r--   0        0        0      452 2023-06-03 02:44:00.208598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/complexes.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.104600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/compose.py
--rw-r--r--   0        0        0  1555308 2023-06-03 02:44:00.088600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/condition.py
--rw-r--r--   0        0        0     1588 2023-06-03 02:44:00.120600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/conjugate.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cos.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.176599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cosh.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.176599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cot.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.180599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/coth.py
--rw-r--r--   0        0        0     1767 2023-06-03 02:44:00.092600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cs.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/csc.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.180599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/csch.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.156599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/curl.py
--rw-r--r--   0        0        0      189 2023-06-03 02:44:02.664565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/declare_occurrence.py
--rw-r--r--   0        0        0      456 2023-06-03 02:44:00.196599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/determinant.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.152599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/diff.py
--rw-r--r--   0        0        0      454 2023-06-03 02:44:00.156599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/divergence.py
--rw-r--r--   0        0        0     1582 2023-06-03 02:44:00.108600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/divide.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.096600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/domain.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.208598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/emptyset.py
--rw-r--r--   0        0        0      438 2023-06-03 02:44:00.140599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/eq.py
--rw-r--r--   0        0        0      454 2023-06-03 02:44:00.140599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/equivalent.py
--rw-r--r--   0        0        0      454 2023-06-03 02:44:00.216598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/eulergamma.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.140599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/exists.py
--rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.128600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/exp.py
--rw-r--r--   0        0        0      458 2023-06-03 02:44:00.208598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/exponentiale.py
--rw-r--r--   0        0        0     1588 2023-06-03 02:44:00.116600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/factorial.py
--rw-r--r--   0        0        0     1586 2023-06-03 02:44:00.148599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/factorof.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.212598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/false.py
--rw-r--r--   0        0        0     1580 2023-06-03 02:44:00.124600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/floor.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.140599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/forall.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.132599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/gcd.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.144599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/geq.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.156599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/grad.py
--rw-r--r--   0        0        0      438 2023-06-03 02:44:00.140599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/gt.py
--rw-r--r--   0        0        0      444 2023-06-03 02:44:00.096600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ident.py
--rw-r--r--   0        0        0      444 2023-06-03 02:44:00.100600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/image.py
--rw-r--r--   0        0        0     1588 2023-06-03 02:44:00.124600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/imaginary.py
--rw-r--r--   0        0        0      454 2023-06-03 02:44:00.212598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/imaginaryi.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.136599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/implies.py
--rw-r--r--   0        0        0      438 2023-06-03 02:44:00.160599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/in_mod.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.216598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/infinity.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.152599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/int_mod.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.204599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/integers.py
--rw-r--r--   0        0        0      452 2023-06-03 02:44:00.160599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/intersect.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.096600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/interval.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.096600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/inverse.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.100600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/lambda_mod.py
--rw-r--r--   0        0        0      452 2023-06-03 02:44:00.156599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/laplacian.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.132599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/lcm.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.144599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/leq.py
--rw-r--r--   0        0        0      444 2023-06-03 02:44:00.168599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/limit.py
--rw-r--r--   0        0        0      161 2023-06-03 02:44:00.224598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/linestyle.py
--rw-r--r--   0        0        0      161 2023-06-03 02:44:02.664565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/list_order.py
--rw-r--r--   0        0        0      438 2023-06-03 02:44:00.100600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ln.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.100600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/log.py
--rw-r--r--   0        0        0      438 2023-06-03 02:44:00.140599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/lt.py
--rw-r--r--   0        0        0      136 2023-06-03 02:44:02.664565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maction_value.py
--rw-r--r--   0        0        0     2637 2023-06-03 02:44:00.268597 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maligngroup.py
--rw-r--r--   0        0        0      207 2023-06-03 02:44:02.708564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maligngroup_groupalign.py
--rw-r--r--   0        0        0      140 2023-06-03 02:44:02.708564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maligngroup_value.py
--rw-r--r--   0        0        0     2605 2023-06-03 02:44:00.264598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/malignmark.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.708564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/malignmark_edge.py
--rw-r--r--   0        0        0      139 2023-06-03 02:44:02.708564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/malignmark_value.py
--rw-r--r--   0        0        0    74524 2023-06-03 02:44:00.364596 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math.py
--rw-r--r--   0        0        0      140 2023-06-03 02:44:02.744564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_accent.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.744564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_accentunder.py
--rw-r--r--   0        0        0      161 2023-06-03 02:44:02.744564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_align.py
--rw-r--r--   0        0        0      142 2023-06-03 02:44:02.744564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_bevelled.py
--rw-r--r--   0        0        0      165 2023-06-03 02:44:02.744564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_charalign.py
--rw-r--r--   0        0        0      166 2023-06-03 02:44:02.744564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_denomalign.py
--rw-r--r--   0        0        0      131 2023-06-03 02:44:02.748564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_dir.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.768564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_display.py
--rw-r--r--   0        0        0      146 2023-06-03 02:44:02.744564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_displaystyle.py
--rw-r--r--   0        0        0      138 2023-06-03 02:44:02.748564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_edge.py
--rw-r--r--   0        0        0      146 2023-06-03 02:44:02.748564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_equalcolumns.py
--rw-r--r--   0        0        0      143 2023-06-03 02:44:02.748564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_equalrows.py
--rw-r--r--   0        0        0      139 2023-06-03 02:44:02.748564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_fence.py
--rw-r--r--   0        0        0      166 2023-06-03 02:44:02.748564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_form.py
--rw-r--r--   0        0        0      199 2023-06-03 02:44:02.752564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_indentalign.py
--rw-r--r--   0        0        0      236 2023-06-03 02:44:02.752564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_indentalignfirst.py
--rw-r--r--   0        0        0      235 2023-06-03 02:44:02.752564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_indentalignlast.py
--rw-r--r--   0        0        0      185 2023-06-03 02:44:02.744564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_infixlinebreakstyle.py
--rw-r--r--   0        0        0      141 2023-06-03 02:44:02.752564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_largeop.py
--rw-r--r--   0        0        0      225 2023-06-03 02:44:02.752564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_linebreak.py
--rw-r--r--   0        0        0      228 2023-06-03 02:44:02.756564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_linebreakstyle.py
--rw-r--r--   0        0        0      208 2023-06-03 02:44:02.756564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_location.py
--rw-r--r--   0        0        0      495 2023-06-03 02:44:02.756564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_longdivstyle.py
--rw-r--r--   0        0        0      641 2023-06-03 02:44:02.760564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_mathvariant.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.760564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_movablelimits.py
--rw-r--r--   0        0        0      164 2023-06-03 02:44:02.760564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_numalign.py
--rw-r--r--   0        0        0      220 2023-06-03 02:44:02.768564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_overflow.py
--rw-r--r--   0        0        0      143 2023-06-03 02:44:02.760564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_separator.py
--rw-r--r--   0        0        0      204 2023-06-03 02:44:02.760564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_side.py
--rw-r--r--   0        0        0      200 2023-06-03 02:44:02.764564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_stackalign.py
--rw-r--r--   0        0        0      142 2023-06-03 02:44:02.764564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_stretchy.py
--rw-r--r--   0        0        0      143 2023-06-03 02:44:02.764564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_symmetric.py
--rw-r--r--   0        0        0      117 2023-06-03 02:44:02.740564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_value.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.196599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/matrix.py
--rw-r--r--   0        0        0      452 2023-06-03 02:44:00.196599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/matrixrow.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.128600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/max.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.192599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mean.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.192599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/median.py
--rw-r--r--   0        0        0      137 2023-06-03 02:44:02.680565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/menclose_value.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.680565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/merror_value.py
--rw-r--r--   0        0        0      136 2023-06-03 02:44:02.680565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfenced_value.py
--rw-r--r--   0        0        0      143 2023-06-03 02:44:02.704564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfrac_bevelled.py
--rw-r--r--   0        0        0      167 2023-06-03 02:44:02.704564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfrac_denomalign.py
--rw-r--r--   0        0        0      165 2023-06-03 02:44:02.704564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfrac_numalign.py
--rw-r--r--   0        0        0      120 2023-06-03 02:44:02.704564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfrac_value.py
--rw-r--r--   0        0        0     5862 2023-06-03 02:44:00.256598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph.py
--rw-r--r--   0        0        0      151 2023-06-03 02:44:02.660565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_fontstyle.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.660565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_fontweight.py
--rw-r--r--   0        0        0      643 2023-06-03 02:44:02.660565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_mathvariant.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.660565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_value.py
--rw-r--r--   0        0        0     5329 2023-06-03 02:44:00.228598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi.py
--rw-r--r--   0        0        0      129 2023-06-03 02:44:02.732564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_dir.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.736564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_fontstyle.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.732564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_fontweight.py
--rw-r--r--   0        0        0      639 2023-06-03 02:44:02.732564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_mathvariant.py
--rw-r--r--   0        0        0      131 2023-06-03 02:44:02.732564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_value.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.132599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/min.py
--rw-r--r--   0        0        0     1580 2023-06-03 02:44:00.108600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/minus.py
--rw-r--r--   0        0        0     3231 2023-06-03 02:44:00.276597 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlabeledtr.py
--rw-r--r--   0        0        0      214 2023-06-03 02:44:02.736564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlabeledtr_rowalign.py
--rw-r--r--   0        0        0      139 2023-06-03 02:44:02.736564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlabeledtr_value.py
--rw-r--r--   0        0        0      499 2023-06-03 02:44:02.664565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlongdiv_longdivstyle.py
--rw-r--r--   0        0        0      137 2023-06-03 02:44:02.664565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlongdiv_value.py
--rw-r--r--   0        0        0      142 2023-06-03 02:44:02.672565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mmultiscripts_value.py
--rw-r--r--   0        0        0     5329 2023-06-03 02:44:00.232598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn.py
--rw-r--r--   0        0        0      129 2023-06-03 02:44:02.732564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_dir.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.732564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_fontstyle.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.732564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_fontweight.py
--rw-r--r--   0        0        0      639 2023-06-03 02:44:02.732564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_mathvariant.py
--rw-r--r--   0        0        0      131 2023-06-03 02:44:02.728564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_value.py
--rw-r--r--   0        0        0    10043 2023-06-03 02:44:00.240598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo.py
--rw-r--r--   0        0        0      138 2023-06-03 02:44:02.724564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_accent.py
--rw-r--r--   0        0        0      129 2023-06-03 02:44:02.720564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_dir.py
--rw-r--r--   0        0        0      137 2023-06-03 02:44:02.724564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_fence.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.720564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_fontstyle.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.720564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_fontweight.py
--rw-r--r--   0        0        0      164 2023-06-03 02:44:02.724564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_form.py
--rw-r--r--   0        0        0      197 2023-06-03 02:44:02.728564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_indentalign.py
--rw-r--r--   0        0        0      234 2023-06-03 02:44:02.728564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_indentalignfirst.py
--rw-r--r--   0        0        0      233 2023-06-03 02:44:02.728564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_indentalignlast.py
--rw-r--r--   0        0        0      139 2023-06-03 02:44:02.724564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_largeop.py
--rw-r--r--   0        0        0      223 2023-06-03 02:44:02.728564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_linebreak.py
--rw-r--r--   0        0        0      226 2023-06-03 02:44:02.728564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_linebreakstyle.py
--rw-r--r--   0        0        0      639 2023-06-03 02:44:02.720564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_mathvariant.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.724564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_movablelimits.py
--rw-r--r--   0        0        0      141 2023-06-03 02:44:02.724564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_separator.py
--rw-r--r--   0        0        0      140 2023-06-03 02:44:02.724564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_stretchy.py
--rw-r--r--   0        0        0      141 2023-06-03 02:44:02.724564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_symmetric.py
--rw-r--r--   0        0        0      125 2023-06-03 02:44:02.720564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_value.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.196599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mode.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.100600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/moment.py
--rw-r--r--   0        0        0      141 2023-06-03 02:44:02.676565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mover_accent.py
--rw-r--r--   0        0        0      162 2023-06-03 02:44:02.676565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mover_align.py
--rw-r--r--   0        0        0      134 2023-06-03 02:44:02.676565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mover_value.py
--rw-r--r--   0        0        0      136 2023-06-03 02:44:02.680565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mpadded_value.py
--rw-r--r--   0        0        0      137 2023-06-03 02:44:02.680565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mphantom_value.py
--rw-r--r--   0        0        0     2432 2023-06-03 02:44:00.264598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mprescripts.py
--rw-r--r--   0        0        0      140 2023-06-03 02:44:02.736564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mprescripts_value.py
--rw-r--r--   0        0        0      134 2023-06-03 02:44:02.700564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mroot_value.py
--rw-r--r--   0        0        0      131 2023-06-03 02:44:02.708564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mrow_dir.py
--rw-r--r--   0        0        0      133 2023-06-03 02:44:02.704564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mrow_value.py
--rw-r--r--   0        0        0     5585 2023-06-03 02:44:00.252598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms.py
--rw-r--r--   0        0        0      129 2023-06-03 02:44:02.712564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_dir.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.712564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_fontstyle.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.712564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_fontweight.py
--rw-r--r--   0        0        0      639 2023-06-03 02:44:02.708564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_mathvariant.py
--rw-r--r--   0        0        0      131 2023-06-03 02:44:02.708564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_value.py
--rw-r--r--   0        0        0      213 2023-06-03 02:44:02.740564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mscarries_location.py
--rw-r--r--   0        0        0      292 2023-06-03 02:44:02.740564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mscarries_value.py
--rw-r--r--   0        0        0      211 2023-06-03 02:44:02.740564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mscarry_location.py
--rw-r--r--   0        0        0      290 2023-06-03 02:44:02.740564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mscarry_value.py
--rw-r--r--   0        0        0      136 2023-06-03 02:44:02.740564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msgroup_value.py
--rw-r--r--   0        0        0     3475 2023-06-03 02:44:00.260598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msline.py
--rw-r--r--   0        0        0      121 2023-06-03 02:44:02.740564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msline_value.py
--rw-r--r--   0        0        0     5838 2023-06-03 02:44:00.248598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace.py
--rw-r--r--   0        0        0      133 2023-06-03 02:44:02.712564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_dir.py
--rw-r--r--   0        0        0      151 2023-06-03 02:44:02.716564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_fontstyle.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.716564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_fontweight.py
--rw-r--r--   0        0        0      269 2023-06-03 02:44:02.716564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_linebreak.py
--rw-r--r--   0        0        0      643 2023-06-03 02:44:02.712564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_mathvariant.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.712564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_value.py
--rw-r--r--   0        0        0      134 2023-06-03 02:44:02.700564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msqrt_value.py
--rw-r--r--   0        0        0      134 2023-06-03 02:44:02.740564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msrow_value.py
--rw-r--r--   0        0        0      167 2023-06-03 02:44:02.664565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstack_charalign.py
--rw-r--r--   0        0        0      202 2023-06-03 02:44:02.664565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstack_stackalign.py
--rw-r--r--   0        0        0      123 2023-06-03 02:44:02.664565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstack_value.py
--rw-r--r--   0        0        0      142 2023-06-03 02:44:02.684565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_accent.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.684565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_accentunder.py
--rw-r--r--   0        0        0      163 2023-06-03 02:44:02.684565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_align.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.684565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_bevelled.py
--rw-r--r--   0        0        0      167 2023-06-03 02:44:02.684565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_charalign.py
--rw-r--r--   0        0        0      168 2023-06-03 02:44:02.684565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_denomalign.py
--rw-r--r--   0        0        0      133 2023-06-03 02:44:02.688565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_dir.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.680565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_displaystyle.py
--rw-r--r--   0        0        0      140 2023-06-03 02:44:02.688565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_edge.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.688565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_equalcolumns.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.688565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_equalrows.py
--rw-r--r--   0        0        0      141 2023-06-03 02:44:02.688565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_fence.py
--rw-r--r--   0        0        0      151 2023-06-03 02:44:02.700564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_fontstyle.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.700564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_fontweight.py
--rw-r--r--   0        0        0      168 2023-06-03 02:44:02.688565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_form.py
--rw-r--r--   0        0        0      201 2023-06-03 02:44:02.692565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_indentalign.py
--rw-r--r--   0        0        0      238 2023-06-03 02:44:02.692565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_indentalignfirst.py
--rw-r--r--   0        0        0      237 2023-06-03 02:44:02.692565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_indentalignlast.py
--rw-r--r--   0        0        0      187 2023-06-03 02:44:02.684565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_infixlinebreakstyle.py
--rw-r--r--   0        0        0      143 2023-06-03 02:44:02.692565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_largeop.py
--rw-r--r--   0        0        0      227 2023-06-03 02:44:02.692565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_linebreak.py
--rw-r--r--   0        0        0      230 2023-06-03 02:44:02.692565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_linebreakstyle.py
--rw-r--r--   0        0        0      210 2023-06-03 02:44:02.692565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_location.py
--rw-r--r--   0        0        0      497 2023-06-03 02:44:02.696565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_longdivstyle.py
--rw-r--r--   0        0        0      643 2023-06-03 02:44:02.696565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_mathvariant.py
--rw-r--r--   0        0        0      149 2023-06-03 02:44:02.696565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_movablelimits.py
--rw-r--r--   0        0        0      166 2023-06-03 02:44:02.696565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_numalign.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.696565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_separator.py
--rw-r--r--   0        0        0      206 2023-06-03 02:44:02.700564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_side.py
--rw-r--r--   0        0        0      202 2023-06-03 02:44:02.700564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_stackalign.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.700564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_stretchy.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.700564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_symmetric.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.680565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_value.py
--rw-r--r--   0        0        0      133 2023-06-03 02:44:02.680565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msub_value.py
--rw-r--r--   0        0        0      136 2023-06-03 02:44:02.676565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msubsup_value.py
--rw-r--r--   0        0        0      133 2023-06-03 02:44:02.676565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msup_value.py
--rw-r--r--   0        0        0     6510 2023-06-03 02:44:00.272597 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.668565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_displaystyle.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.668565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_equalcolumns.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.668565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_equalrows.py
--rw-r--r--   0        0        0      206 2023-06-03 02:44:02.668565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_side.py
--rw-r--r--   0        0        0      141 2023-06-03 02:44:02.668565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_value.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.280597 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtd.py
--rw-r--r--   0        0        0     5386 2023-06-03 02:44:00.244598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext.py
--rw-r--r--   0        0        0      132 2023-06-03 02:44:02.716564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_dir.py
--rw-r--r--   0        0        0      150 2023-06-03 02:44:02.716564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_fontstyle.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.716564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_fontweight.py
--rw-r--r--   0        0        0      642 2023-06-03 02:44:02.716564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_mathvariant.py
--rw-r--r--   0        0        0      134 2023-06-03 02:44:02.716564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_value.py
--rw-r--r--   0        0        0     3175 2023-06-03 02:44:00.280597 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtr.py
--rw-r--r--   0        0        0      207 2023-06-03 02:44:02.672565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtr_rowalign.py
--rw-r--r--   0        0        0      132 2023-06-03 02:44:02.668565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtr_value.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.676565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munder_accentunder.py
--rw-r--r--   0        0        0      163 2023-06-03 02:44:02.676565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munder_align.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.676565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munder_value.py
--rw-r--r--   0        0        0      146 2023-06-03 02:44:02.672565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munderover_accent.py
--rw-r--r--   0        0        0      151 2023-06-03 02:44:02.672565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munderover_accentunder.py
--rw-r--r--   0        0        0      167 2023-06-03 02:44:02.672565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munderover_align.py
--rw-r--r--   0        0        0      139 2023-06-03 02:44:02.672565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munderover_value.py
--rw-r--r--   0        0        0      462 2023-06-03 02:44:00.204599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/naturalnumbers.py
--rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.144599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/neq.py
--rw-r--r--   0        0        0     2401 2023-06-03 02:44:00.260598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/none.py
--rw-r--r--   0        0        0      133 2023-06-03 02:44:02.736564 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/none_value.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.136599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/not_mod.py
--rw-r--r--   0        0        0      454 2023-06-03 02:44:00.212598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/notanumber.py
--rw-r--r--   0        0        0      444 2023-06-03 02:44:00.160599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/notin.py
--rw-r--r--   0        0        0      456 2023-06-03 02:44:00.164599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/notprsubset.py
--rw-r--r--   0        0        0      452 2023-06-03 02:44:00.164599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/notsubset.py
--rw-r--r--   0        0        0      438 2023-06-03 02:44:00.136599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/or_mod.py
--rw-r--r--   0        0        0      458 2023-06-03 02:44:00.204599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/outerproduct.py
--rw-r--r--   0        0        0      456 2023-06-03 02:44:00.156599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/partialdiff.py
--rw-r--r--   0        0        0      438 2023-06-03 02:44:00.216598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/pi.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.132599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/plus.py
--rw-r--r--   0        0        0     1580 2023-06-03 02:44:00.108600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/power.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.208598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/primes.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.168599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/product.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.164599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/prsubset.py
--rw-r--r--   0        0        0     1586 2023-06-03 02:44:00.104600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/quotient.py
--rw-r--r--   0        0        0      452 2023-06-03 02:44:00.204599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/rationals.py
--rw-r--r--   0        0        0     1578 2023-06-03 02:44:00.124600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/real.py
--rw-r--r--   0        0        0      444 2023-06-03 02:44:00.204599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/reals.py
--rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.112600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/rem.py
--rw-r--r--   0        0        0     1578 2023-06-03 02:44:00.112600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/root.py
--rw-r--r--   0        0        0      460 2023-06-03 02:44:00.200599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/scalarproduct.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.192599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sdev.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sec.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.180599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sech.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.200599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/selector.py
--rw-r--r--   0        0        0      215 2023-06-03 02:44:00.092600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sep.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.164599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/setdiff.py
--rw-r--r--   0        0        0     1405 2023-06-03 02:44:00.088600 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/share.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sin.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.176599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sinh.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.164599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/subset.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.168599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sum.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/tan.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.176599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/tanh.py
--rw-r--r--   0        0        0     1710 2023-06-03 02:44:00.152599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/tendsto.py
--rw-r--r--   0        0        0      444 2023-06-03 02:44:00.132599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/times.py
--rw-r--r--   0        0        0      452 2023-06-03 02:44:00.200599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/transpose.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.212598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/true.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.160599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/union.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.192599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/variance.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.196599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/vector.py
--rw-r--r--   0        0        0      460 2023-06-03 02:44:00.200599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/vectorproduct.py
--rw-r--r--   0        0        0      209 2023-06-03 02:44:00.224598 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/verticalalign.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.136599 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/xor.py
--rw-r--r--   0        0        0       15 2023-06-03 02:17:59.961981 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1999/__init__.py
--rw-r--r--   0        0        0      488 2023-06-03 02:43:58.316624 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1999/xlink/__init__.py
--rw-r--r--   0        0        0      188 2023-06-03 02:44:02.660565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1999/xlink/actuate_value.py
--rw-r--r--   0        0        0     1893 2023-06-03 02:43:58.428623 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1999/xlink/arc_type.py
--rw-r--r--   0        0        0     1169 2023-06-03 02:43:58.420623 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1999/xlink/extended.py
--rw-r--r--   0        0        0     1453 2023-06-03 02:43:58.428623 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1999/xlink/locator_type.py
--rw-r--r--   0        0        0     1244 2023-06-03 02:43:58.424623 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1999/xlink/resource_type.py
--rw-r--r--   0        0        0      193 2023-06-03 02:44:02.660565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1999/xlink/show_value.py
--rw-r--r--   0        0        0     1940 2023-06-03 02:43:58.416623 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1999/xlink/simple.py
--rw-r--r--   0        0        0     1203 2023-06-03 02:43:58.424623 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1999/xlink/title_elt_type.py
--rw-r--r--   0        0        0      247 2023-06-03 02:44:02.660565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1999/xlink/type_value.py
--rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/xml/__init__.py
--rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/xml/pkg_1998/__init__.py
--rw-r--r--   0        0        0      120 2023-06-03 02:43:58.380623 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/xml/pkg_1998/namespace/__init__.py
--rw-r--r--   0        0        0      118 2023-06-03 02:44:02.656565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/xml/pkg_1998/namespace/lang_value.py
--rw-r--r--   0        0        0      154 2023-06-03 02:44:02.656565 pubmed_types-0.1.0/src/pubmed_types/models/org/w3/xml/pkg_1998/namespace/space_value.py
--rw-r--r--   0        0        0      997 2023-06-03 02:44:02.632565 pubmed_types-0.1.0/src/pubmed_types/models/other_abstract.py
--rw-r--r--   0        0        0      223 2023-06-03 02:44:02.844563 pubmed_types-0.1.0/src/pubmed_types/models/other_abstract_type.py
--rw-r--r--   0        0        0      518 2023-06-03 02:44:02.632565 pubmed_types-0.1.0/src/pubmed_types/models/other_id.py
--rw-r--r--   0        0        0      257 2023-06-03 02:44:02.840563 pubmed_types-0.1.0/src/pubmed_types/models/other_id_source.py
--rw-r--r--   0        0        0      863 2023-06-03 02:44:02.312570 pubmed_types-0.1.0/src/pubmed_types/models/overline_end.py
--rw-r--r--   0        0        0      747 2023-06-03 02:44:02.312570 pubmed_types-0.1.0/src/pubmed_types/models/overline_start.py
--rw-r--r--   0        0        0       82 2023-06-03 02:44:02.772564 pubmed_types-0.1.0/src/pubmed_types/models/overline_toggle.py
--rw-r--r--   0        0        0      692 2023-06-03 02:44:02.316570 pubmed_types-0.1.0/src/pubmed_types/models/page_count.py
--rw-r--r--   0        0        0     1349 2023-06-03 02:44:02.320570 pubmed_types-0.1.0/src/pubmed_types/models/page_range.py
--rw-r--r--   0        0        0      649 2023-06-03 02:44:02.636565 pubmed_types-0.1.0/src/pubmed_types/models/pagination.py
--rw-r--r--   0        0        0     1147 2023-06-03 02:44:02.636565 pubmed_types-0.1.0/src/pubmed_types/models/param.py
--rw-r--r--   0        0        0      831 2023-06-03 02:44:02.640565 pubmed_types-0.1.0/src/pubmed_types/models/personal_name_subject.py
--rw-r--r--   0        0        0      426 2023-06-03 02:44:02.640565 pubmed_types-0.1.0/src/pubmed_types/models/personal_name_subject_list.py
--rw-r--r--   0        0        0      461 2023-06-03 02:44:02.632565 pubmed_types-0.1.0/src/pubmed_types/models/pmid.py
--rw-r--r--   0        0        0     1366 2023-06-03 02:44:02.320570 pubmed_types-0.1.0/src/pubmed_types/models/postal_code.py
--rw-r--r--   0        0        0      112 2023-06-03 02:44:02.796563 pubmed_types-0.1.0/src/pubmed_types/models/preformat_orientation.py
--rw-r--r--   0        0        0      149 2023-06-03 02:44:02.796563 pubmed_types-0.1.0/src/pubmed_types/models/preformat_position.py
--rw-r--r--   0        0        0     2142 2023-06-03 02:44:02.324570 pubmed_types-0.1.0/src/pubmed_types/models/principal_award_recipient.py
--rw-r--r--   0        0        0     1855 2023-06-03 02:44:02.328570 pubmed_types-0.1.0/src/pubmed_types/models/principal_investigator.py
--rw-r--r--   0        0        0     2483 2023-06-03 02:44:02.332569 pubmed_types-0.1.0/src/pubmed_types/models/processing_meta.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.824563 pubmed_types-0.1.0/src/pubmed_types/models/processing_meta_base_tagset.py
--rw-r--r--   0        0        0      109 2023-06-03 02:44:02.824563 pubmed_types-0.1.0/src/pubmed_types/models/processing_meta_mathml_version.py
--rw-r--r--   0        0        0      138 2023-06-03 02:44:02.824563 pubmed_types-0.1.0/src/pubmed_types/models/processing_meta_table_model.py
--rw-r--r--   0        0        0      116 2023-06-03 02:44:02.828563 pubmed_types-0.1.0/src/pubmed_types/models/processing_meta_tagset_family.py
--rw-r--r--   0        0        0      936 2023-06-03 02:44:02.912562 pubmed_types-0.1.0/src/pubmed_types/models/pub_date_1.py
--rw-r--r--   0        0        0     2895 2023-06-03 02:44:02.916561 pubmed_types-0.1.0/src/pubmed_types/models/pub_date_2.py
--rw-r--r--   0        0        0      740 2023-06-03 02:44:02.332569 pubmed_types-0.1.0/src/pubmed_types/models/pub_date_not_available.py
--rw-r--r--   0        0        0      408 2023-06-03 02:18:04.041925 pubmed_types-0.1.0/src/pubmed_types/models/pub_date_pub_status.py
--rw-r--r--   0        0        0      708 2023-06-03 02:44:02.336569 pubmed_types-0.1.0/src/pubmed_types/models/pub_history.py
--rw-r--r--   0        0        0     2871 2023-06-03 02:44:02.340569 pubmed_types-0.1.0/src/pubmed_types/models/pub_id.py
--rw-r--r--   0        0        0     1462 2023-06-03 02:44:02.644565 pubmed_types-0.1.0/src/pubmed_types/models/pub_med_pub_date.py
--rw-r--r--   0        0        0      496 2023-06-03 02:44:02.848563 pubmed_types-0.1.0/src/pubmed_types/models/pub_med_pub_date_pub_status.py
--rw-r--r--   0        0        0      423 2023-06-03 02:44:02.640565 pubmed_types-0.1.0/src/pubmed_types/models/publication_type.py
--rw-r--r--   0        0        0      400 2023-06-03 02:44:02.640565 pubmed_types-0.1.0/src/pubmed_types/models/publication_type_list.py
--rw-r--r--   0        0        0     1192 2023-06-03 02:18:03.561932 pubmed_types-0.1.0/src/pubmed_types/models/publisher.py
--rw-r--r--   0        0        0      606 2023-06-03 02:44:02.920561 pubmed_types-0.1.0/src/pubmed_types/models/publisher_1.py
--rw-r--r--   0        0        0     1193 2023-06-03 02:44:02.920561 pubmed_types-0.1.0/src/pubmed_types/models/publisher_2.py
--rw-r--r--   0        0        0     1013 2023-06-03 02:44:02.924561 pubmed_types-0.1.0/src/pubmed_types/models/publisher_name_1.py
--rw-r--r--   0        0        0      600 2023-06-03 02:44:02.556566 pubmed_types-0.1.0/src/pubmed_types/models/pubmed_article.py
--rw-r--r--   0        0        0      839 2023-06-03 02:44:02.552566 pubmed_types-0.1.0/src/pubmed_types/models/pubmed_article_set.py
--rw-r--r--   0        0        0      611 2023-06-03 02:44:02.556566 pubmed_types-0.1.0/src/pubmed_types/models/pubmed_book_article.py
--rw-r--r--   0        0        0      384 2023-06-03 02:44:02.556566 pubmed_types-0.1.0/src/pubmed_types/models/pubmed_book_article_set.py
--rw-r--r--   0        0        0      991 2023-06-03 02:44:02.572566 pubmed_types-0.1.0/src/pubmed_types/models/pubmed_book_data.py
--rw-r--r--   0        0        0     1217 2023-06-03 02:44:02.572566 pubmed_types-0.1.0/src/pubmed_types/models/pubmed_data.py
--rw-r--r--   0        0        0      724 2023-06-03 02:44:02.644565 pubmed_types-0.1.0/src/pubmed_types/models/qualifier_name.py
--rw-r--r--   0        0        0       87 2023-06-03 02:44:02.840563 pubmed_types-0.1.0/src/pubmed_types/models/qualifier_name_major_topic_yn.py
--rw-r--r--   0        0        0      268 2023-06-03 02:44:02.800563 pubmed_types-0.1.0/src/pubmed_types/models/question_question_response_type.py
--rw-r--r--   0        0        0      695 2023-06-03 02:44:02.344569 pubmed_types-0.1.0/src/pubmed_types/models/ref_count.py
--rw-r--r--   0        0        0      576 2023-06-03 02:44:02.644565 pubmed_types-0.1.0/src/pubmed_types/models/reference.py
--rw-r--r--   0        0        0      678 2023-06-03 02:44:02.644565 pubmed_types-0.1.0/src/pubmed_types/models/reference_list.py
--rw-r--r--   0        0        0      460 2023-06-03 02:18:03.773929 pubmed_types-0.1.0/src/pubmed_types/models/replaces.py
--rw-r--r--   0        0        0      192 2023-06-03 02:18:04.045925 pubmed_types-0.1.0/src/pubmed_types/models/replaces_id_type.py
--rw-r--r--   0        0        0     1440 2023-06-03 02:44:02.348569 pubmed_types-0.1.0/src/pubmed_types/models/resource_group.py
--rw-r--r--   0        0        0     2014 2023-06-03 02:44:02.348569 pubmed_types-0.1.0/src/pubmed_types/models/resource_id.py
--rw-r--r--   0        0        0     4999 2023-06-03 02:44:02.356569 pubmed_types-0.1.0/src/pubmed_types/models/resource_name.py
--rw-r--r--   0        0        0     1009 2023-06-03 02:44:02.360569 pubmed_types-0.1.0/src/pubmed_types/models/resource_wrap.py
--rw-r--r--   0        0        0     2223 2023-06-03 02:44:02.364569 pubmed_types-0.1.0/src/pubmed_types/models/response.py
--rw-r--r--   0        0        0     3137 2023-06-03 02:44:02.368569 pubmed_types-0.1.0/src/pubmed_types/models/restricted_by.py
--rw-r--r--   0        0        0       79 2023-06-03 02:44:02.772564 pubmed_types-0.1.0/src/pubmed_types/models/roman_toggle.py
--rw-r--r--   0        0        0      728 2023-06-03 02:44:02.368569 pubmed_types-0.1.0/src/pubmed_types/models/rp.py
--rw-r--r--   0        0        0     1346 2023-06-03 02:44:02.372569 pubmed_types-0.1.0/src/pubmed_types/models/rt.py
--rw-r--r--   0        0        0       83 2023-06-03 02:44:02.772564 pubmed_types-0.1.0/src/pubmed_types/models/sans_serif_toggle.py
--rw-r--r--   0        0        0       76 2023-06-03 02:44:02.776564 pubmed_types-0.1.0/src/pubmed_types/models/sc_toggle.py
--rw-r--r--   0        0        0     1337 2023-06-03 02:44:02.376569 pubmed_types-0.1.0/src/pubmed_types/models/season.py
--rw-r--r--   0        0        0      765 2023-06-03 02:44:02.648565 pubmed_types-0.1.0/src/pubmed_types/models/section.py
--rw-r--r--   0        0        0     1341 2023-06-03 02:44:02.648565 pubmed_types-0.1.0/src/pubmed_types/models/section_title.py
--rw-r--r--   0        0        0      347 2023-06-03 02:44:02.648565 pubmed_types-0.1.0/src/pubmed_types/models/sections.py
--rw-r--r--   0        0        0     9015 2023-06-03 02:44:02.388569 pubmed_types-0.1.0/src/pubmed_types/models/self_uri.py
--rw-r--r--   0        0        0     7416 2023-06-03 02:44:02.400569 pubmed_types-0.1.0/src/pubmed_types/models/series_text.py
--rw-r--r--   0        0        0     7394 2023-06-03 02:44:02.412568 pubmed_types-0.1.0/src/pubmed_types/models/series_title.py
--rw-r--r--   0        0        0     7912 2023-06-03 02:44:02.424568 pubmed_types-0.1.0/src/pubmed_types/models/sig.py
--rw-r--r--   0        0        0     8403 2023-06-03 02:44:02.440568 pubmed_types-0.1.0/src/pubmed_types/models/sig_block.py
--rw-r--r--   0        0        0     1361 2023-06-03 02:44:02.444568 pubmed_types-0.1.0/src/pubmed_types/models/state.py
--rw-r--r--   0        0        0       80 2023-06-03 02:44:02.776564 pubmed_types-0.1.0/src/pubmed_types/models/strike_toggle.py
--rw-r--r--   0        0        0     8497 2023-06-03 02:44:02.460568 pubmed_types-0.1.0/src/pubmed_types/models/string_conf.py
--rw-r--r--   0        0        0      159 2023-06-03 02:44:02.784563 pubmed_types-0.1.0/src/pubmed_types/models/string_name_name_style.py
--rw-r--r--   0        0        0       87 2023-06-03 02:44:02.780563 pubmed_types-0.1.0/src/pubmed_types/models/styled_content_toggle.py
--rw-r--r--   0        0        0      993 2023-06-03 02:44:02.924561 pubmed_types-0.1.0/src/pubmed_types/models/sub_1.py
--rw-r--r--   0        0        0       92 2023-06-03 02:44:02.780563 pubmed_types-0.1.0/src/pubmed_types/models/sub_arrange.py
--rw-r--r--   0        0        0     2576 2023-06-03 02:44:02.468568 pubmed_types-0.1.0/src/pubmed_types/models/sub_article.py
--rw-r--r--   0        0        0      999 2023-06-03 02:44:02.924561 pubmed_types-0.1.0/src/pubmed_types/models/suffix_1.py
--rw-r--r--   0        0        0      993 2023-06-03 02:44:02.928561 pubmed_types-0.1.0/src/pubmed_types/models/sup_1.py
--rw-r--r--   0        0        0       92 2023-06-03 02:44:02.780563 pubmed_types-0.1.0/src/pubmed_types/models/sup_arrange.py
--rw-r--r--   0        0        0      386 2023-06-03 02:44:02.648565 pubmed_types-0.1.0/src/pubmed_types/models/suppl_mesh_list.py
--rw-r--r--   0        0        0      668 2023-06-03 02:44:02.652565 pubmed_types-0.1.0/src/pubmed_types/models/suppl_mesh_name.py
--rw-r--r--   0        0        0      185 2023-06-03 02:44:02.836563 pubmed_types-0.1.0/src/pubmed_types/models/suppl_mesh_name_type.py
--rw-r--r--   0        0        0      124 2023-06-03 02:44:02.800563 pubmed_types-0.1.0/src/pubmed_types/models/supplementary_material_orientation.py
--rw-r--r--   0        0        0      161 2023-06-03 02:44:02.800563 pubmed_types-0.1.0/src/pubmed_types/models/supplementary_material_position.py
--rw-r--r--   0        0        0     1316 2023-06-03 02:44:02.472568 pubmed_types-0.1.0/src/pubmed_types/models/support_description.py
--rw-r--r--   0        0        0     1500 2023-06-03 02:44:02.476568 pubmed_types-0.1.0/src/pubmed_types/models/support_group.py
--rw-r--r--   0        0        0     9397 2023-06-03 02:44:02.500567 pubmed_types-0.1.0/src/pubmed_types/models/support_source.py
--rw-r--r--   0        0        0      695 2023-06-03 02:44:02.500567 pubmed_types-0.1.0/src/pubmed_types/models/table_count.py
--rw-r--r--   0        0        0      220 2023-06-03 02:44:02.804563 pubmed_types-0.1.0/src/pubmed_types/models/table_frame.py
--rw-r--r--   0        0        0      140 2023-06-03 02:44:02.804563 pubmed_types-0.1.0/src/pubmed_types/models/table_rules.py
--rw-r--r--   0        0        0      117 2023-06-03 02:44:02.820563 pubmed_types-0.1.0/src/pubmed_types/models/table_wrap_group_orientation.py
--rw-r--r--   0        0        0      154 2023-06-03 02:44:02.820563 pubmed_types-0.1.0/src/pubmed_types/models/table_wrap_group_position.py
--rw-r--r--   0        0        0      112 2023-06-03 02:44:02.800563 pubmed_types-0.1.0/src/pubmed_types/models/table_wrap_orientation.py
--rw-r--r--   0        0        0      149 2023-06-03 02:44:02.800563 pubmed_types-0.1.0/src/pubmed_types/models/table_wrap_position.py
--rw-r--r--   0        0        0      150 2023-06-03 02:44:02.816563 pubmed_types-0.1.0/src/pubmed_types/models/tbody_align.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.820563 pubmed_types-0.1.0/src/pubmed_types/models/tbody_valign.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.812563 pubmed_types-0.1.0/src/pubmed_types/models/td_align.py
--rw-r--r--   0        0        0      129 2023-06-03 02:44:02.812563 pubmed_types-0.1.0/src/pubmed_types/models/td_scope.py
--rw-r--r--   0        0        0      132 2023-06-03 02:44:02.816563 pubmed_types-0.1.0/src/pubmed_types/models/td_valign.py
--rw-r--r--   0        0        0     1386 2023-06-03 02:44:02.504567 pubmed_types-0.1.0/src/pubmed_types/models/tex_math.py
--rw-r--r--   0        0        0      128 2023-06-03 02:44:02.780563 pubmed_types-0.1.0/src/pubmed_types/models/tex_math_notation.py
--rw-r--r--   0        0        0      150 2023-06-03 02:44:02.816563 pubmed_types-0.1.0/src/pubmed_types/models/tfoot_align.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.816563 pubmed_types-0.1.0/src/pubmed_types/models/tfoot_valign.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.812563 pubmed_types-0.1.0/src/pubmed_types/models/th_align.py
--rw-r--r--   0        0        0      129 2023-06-03 02:44:02.812563 pubmed_types-0.1.0/src/pubmed_types/models/th_scope.py
--rw-r--r--   0        0        0      132 2023-06-03 02:44:02.812563 pubmed_types-0.1.0/src/pubmed_types/models/th_valign.py
--rw-r--r--   0        0        0      150 2023-06-03 02:44:02.808563 pubmed_types-0.1.0/src/pubmed_types/models/thead_align.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.808563 pubmed_types-0.1.0/src/pubmed_types/models/thead_valign.py
--rw-r--r--   0        0        0     1542 2023-06-03 02:44:02.508567 pubmed_types-0.1.0/src/pubmed_types/models/title_group.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.808563 pubmed_types-0.1.0/src/pubmed_types/models/tr_align.py
--rw-r--r--   0        0        0      132 2023-06-03 02:44:02.808563 pubmed_types-0.1.0/src/pubmed_types/models/tr_valign.py
--rw-r--r--   0        0        0     8912 2023-06-03 02:44:02.520567 pubmed_types-0.1.0/src/pubmed_types/models/trans_abstract.py
--rw-r--r--   0        0        0     7376 2023-06-03 02:44:02.532567 pubmed_types-0.1.0/src/pubmed_types/models/trans_subtitle.py
--rw-r--r--   0        0        0     1641 2023-06-03 02:44:02.536567 pubmed_types-0.1.0/src/pubmed_types/models/trans_title_group.py
--rw-r--r--   0        0        0     2610 2023-06-03 02:44:02.584566 pubmed_types-0.1.0/src/pubmed_types/models/u.py
--rw-r--r--   0        0        0      866 2023-06-03 02:44:02.536567 pubmed_types-0.1.0/src/pubmed_types/models/underline_end.py
--rw-r--r--   0        0        0      750 2023-06-03 02:44:02.540567 pubmed_types-0.1.0/src/pubmed_types/models/underline_start.py
--rw-r--r--   0        0        0       83 2023-06-03 02:44:02.776564 pubmed_types-0.1.0/src/pubmed_types/models/underline_toggle.py
--rw-r--r--   0        0        0      614 2023-06-03 02:44:02.652565 pubmed_types-0.1.0/src/pubmed_types/models/url.py
--rw-r--r--   0        0        0      661 2023-06-03 02:44:02.856562 pubmed_types-0.1.0/src/pubmed_types/models/url_lang.py
--rw-r--r--   0        0        0      150 2023-06-03 02:44:02.856562 pubmed_types-0.1.0/src/pubmed_types/models/url_type.py
--rw-r--r--   0        0        0     1072 2023-06-03 02:44:02.656565 pubmed_types-0.1.0/src/pubmed_types/models/vernacular_title.py
--rw-r--r--   0        0        0     2893 2023-06-03 02:44:02.544567 pubmed_types-0.1.0/src/pubmed_types/models/volume_issue_group.py
--rw-r--r--   0        0        0      962 2023-06-03 02:44:02.656565 pubmed_types-0.1.0/src/pubmed_types/models/volume_title.py
--rw-r--r--   0        0        0      692 2023-06-03 02:44:02.548566 pubmed_types-0.1.0/src/pubmed_types/models/word_count.py
--rw-r--r--   0        0        0      330 2023-06-03 02:44:02.656565 pubmed_types-0.1.0/src/pubmed_types/models/xs_pattern.py
--rw-r--r--   0        0        0     1627 2023-06-03 02:44:02.552566 pubmed_types-0.1.0/src/pubmed_types/models/year.py
--rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 pubmed_types-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-25 16:03:32.757838 pubmed_types-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3934 2023-06-04 13:47:52.792647 pubmed_types-0.1.1/README.md
+-rw-r--r--   0        0        0     1444 2023-06-04 13:48:30.592052 pubmed_types-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      483 2023-06-04 13:47:52.792647 pubmed_types-0.1.1/src/pubmed_types/__init__.py
+-rw-r--r--   0        0        0    24766 2023-06-03 02:43:58.380623 pubmed_types-0.1.1/src/pubmed_types/models/__init__.py
+-rw-r--r--   0        0        0     7420 2023-06-03 02:44:01.924575 pubmed_types-0.1.1/src/pubmed_types/models/abbrev_journal_title.py
+-rw-r--r--   0        0        0      610 2023-06-03 02:44:02.860562 pubmed_types-0.1.1/src/pubmed_types/models/abstract_1.py
+-rw-r--r--   0        0        0     1645 2023-06-03 02:44:02.572566 pubmed_types-0.1.1/src/pubmed_types/models/abstract_text.py
+-rw-r--r--   0        0        0      229 2023-06-03 02:44:02.832563 pubmed_types-0.1.1/src/pubmed_types/models/abstract_text_nlm_category.py
+-rw-r--r--   0        0        0  1064015 2023-06-03 02:44:01.912575 pubmed_types-0.1.1/src/pubmed_types/models/access_date.py
+-rw-r--r--   0        0        0      342 2023-06-03 02:44:02.576566 pubmed_types-0.1.1/src/pubmed_types/models/accession_number_list.py
+-rw-r--r--   0        0        0      962 2023-06-03 02:44:02.576566 pubmed_types-0.1.1/src/pubmed_types/models/affiliation.py
+-rw-r--r--   0        0        0      588 2023-06-03 02:44:02.576566 pubmed_types-0.1.1/src/pubmed_types/models/affiliation_info.py
+-rw-r--r--   0        0        0     1373 2023-06-03 02:44:01.924575 pubmed_types-0.1.1/src/pubmed_types/models/alt_text.py
+-rw-r--r--   0        0        0     8831 2023-06-03 02:44:01.944575 pubmed_types-0.1.1/src/pubmed_types/models/app.py
+-rw-r--r--   0        0        0     8786 2023-06-03 02:44:01.960574 pubmed_types-0.1.1/src/pubmed_types/models/app_group.py
+-rw-r--r--   0        0        0      419 2023-06-03 02:18:03.813928 pubmed_types-0.1.1/src/pubmed_types/models/archive_copy_source.py
+-rw-r--r--   0        0        0      108 2023-06-03 02:44:02.776564 pubmed_types-0.1.1/src/pubmed_types/models/array_orientation.py
+-rw-r--r--   0        0        0     3079 2023-06-03 02:44:02.864562 pubmed_types-0.1.1/src/pubmed_types/models/article_1.py
+-rw-r--r--   0        0        0     2649 2023-06-03 02:44:02.876562 pubmed_types-0.1.1/src/pubmed_types/models/article_2.py
+-rw-r--r--   0        0        0     1202 2023-06-03 02:44:01.960574 pubmed_types-0.1.1/src/pubmed_types/models/article_categories.py
+-rw-r--r--   0        0        0      878 2023-06-03 02:44:02.576566 pubmed_types-0.1.1/src/pubmed_types/models/article_date.py
+-rw-r--r--   0        0        0      369 2023-06-03 02:44:02.824563 pubmed_types-0.1.1/src/pubmed_types/models/article_dtd_version.py
+-rw-r--r--   0        0        0     1423 2023-06-03 02:44:01.964574 pubmed_types-0.1.1/src/pubmed_types/models/article_id.py
+-rw-r--r--   0        0        0      511 2023-06-03 02:44:02.876562 pubmed_types-0.1.1/src/pubmed_types/models/article_id_1.py
+-rw-r--r--   0        0        0      303 2023-06-03 02:44:02.848563 pubmed_types-0.1.1/src/pubmed_types/models/article_id_id_type.py
+-rw-r--r--   0        0        0      368 2023-06-03 02:44:02.580566 pubmed_types-0.1.1/src/pubmed_types/models/article_id_list.py
+-rw-r--r--   0        0        0     9515 2023-06-03 02:44:01.980574 pubmed_types-0.1.1/src/pubmed_types/models/article_meta.py
+-rw-r--r--   0        0        0      242 2023-06-03 02:44:02.828563 pubmed_types-0.1.1/src/pubmed_types/models/article_pub_model.py
+-rw-r--r--   0        0        0      353 2023-06-03 02:18:03.769929 pubmed_types-0.1.1/src/pubmed_types/models/article_set.py
+-rw-r--r--   0        0        0     1495 2023-06-03 02:44:02.880562 pubmed_types-0.1.1/src/pubmed_types/models/article_title_1.py
+-rw-r--r--   0        0        0     3823 2023-06-03 02:44:01.988574 pubmed_types-0.1.1/src/pubmed_types/models/article_version.py
+-rw-r--r--   0        0        0      827 2023-06-03 02:44:01.992574 pubmed_types-0.1.1/src/pubmed_types/models/article_version_alternatives.py
+-rw-r--r--   0        0        0     1938 2023-06-03 02:44:02.580566 pubmed_types-0.1.1/src/pubmed_types/models/author.py
+-rw-r--r--   0        0        0       80 2023-06-03 02:44:02.836563 pubmed_types-0.1.1/src/pubmed_types/models/author_equal_contrib.py
+-rw-r--r--   0        0        0      838 2023-06-03 02:44:02.584566 pubmed_types-0.1.1/src/pubmed_types/models/author_list.py
+-rw-r--r--   0        0        0       82 2023-06-03 02:44:02.832563 pubmed_types-0.1.1/src/pubmed_types/models/author_list_complete_yn.py
+-rw-r--r--   0        0        0      100 2023-06-03 02:44:02.832563 pubmed_types-0.1.1/src/pubmed_types/models/author_list_type.py
+-rw-r--r--   0        0        0     1720 2023-06-03 02:44:02.000574 pubmed_types-0.1.1/src/pubmed_types/models/author_notes.py
+-rw-r--r--   0        0        0       75 2023-06-03 02:44:02.836563 pubmed_types-0.1.1/src/pubmed_types/models/author_valid_yn.py
+-rw-r--r--   0        0        0     2449 2023-06-03 02:44:02.004574 pubmed_types-0.1.1/src/pubmed_types/models/award_desc.py
+-rw-r--r--   0        0        0     4315 2023-06-03 02:44:02.012574 pubmed_types-0.1.1/src/pubmed_types/models/award_group.py
+-rw-r--r--   0        0        0     2442 2023-06-03 02:44:02.016574 pubmed_types-0.1.1/src/pubmed_types/models/award_name.py
+-rw-r--r--   0        0        0     2079 2023-06-03 02:44:02.020574 pubmed_types-0.1.1/src/pubmed_types/models/back.py
+-rw-r--r--   0        0        0      765 2023-06-03 02:44:02.584566 pubmed_types-0.1.1/src/pubmed_types/models/beginning_date.py
+-rw-r--r--   0        0        0     7356 2023-06-03 02:44:02.032574 pubmed_types-0.1.1/src/pubmed_types/models/body.py
+-rw-r--r--   0        0        0       78 2023-06-03 02:44:02.768564 pubmed_types-0.1.1/src/pubmed_types/models/bold_toggle.py
+-rw-r--r--   0        0        0     3125 2023-06-03 02:44:02.588566 pubmed_types-0.1.1/src/pubmed_types/models/book.py
+-rw-r--r--   0        0        0     4185 2023-06-03 02:44:02.560566 pubmed_types-0.1.1/src/pubmed_types/models/book_document.py
+-rw-r--r--   0        0        0      587 2023-06-03 02:44:02.556566 pubmed_types-0.1.1/src/pubmed_types/models/book_document_set.py
+-rw-r--r--   0        0        0     1444 2023-06-03 02:44:02.592566 pubmed_types-0.1.1/src/pubmed_types/models/book_title.py
+-rw-r--r--   0        0        0      112 2023-06-03 02:44:02.784563 pubmed_types-0.1.1/src/pubmed_types/models/boxed_text_orientation.py
+-rw-r--r--   0        0        0      149 2023-06-03 02:44:02.788563 pubmed_types-0.1.1/src/pubmed_types/models/boxed_text_position.py
+-rw-r--r--   0        0        0      529 2023-06-03 02:44:02.032574 pubmed_types-0.1.1/src/pubmed_types/models/break_mod.py
+-rw-r--r--   0        0        0      117 2023-06-03 02:44:02.788563 pubmed_types-0.1.1/src/pubmed_types/models/chem_struct_wrap_orientation.py
+-rw-r--r--   0        0        0      154 2023-06-03 02:44:02.788563 pubmed_types-0.1.1/src/pubmed_types/models/chem_struct_wrap_position.py
+-rw-r--r--   0        0        0      592 2023-06-03 02:44:02.592566 pubmed_types-0.1.1/src/pubmed_types/models/chemical.py
+-rw-r--r--   0        0        0      356 2023-06-03 02:44:02.592566 pubmed_types-0.1.1/src/pubmed_types/models/chemical_list.py
+-rw-r--r--   0        0        0     1065 2023-06-03 02:44:02.592566 pubmed_types-0.1.1/src/pubmed_types/models/citation.py
+-rw-r--r--   0        0        0     1344 2023-06-03 02:44:02.036574 pubmed_types-0.1.1/src/pubmed_types/models/city.py
+-rw-r--r--   0        0        0       82 2023-06-03 02:44:02.788563 pubmed_types-0.1.1/src/pubmed_types/models/code_executable.py
+-rw-r--r--   0        0        0      107 2023-06-03 02:44:02.788563 pubmed_types-0.1.1/src/pubmed_types/models/code_orientation.py
+-rw-r--r--   0        0        0      144 2023-06-03 02:44:02.788563 pubmed_types-0.1.1/src/pubmed_types/models/code_position.py
+-rw-r--r--   0        0        0      963 2023-06-03 02:44:02.596566 pubmed_types-0.1.1/src/pubmed_types/models/coi_statement.py
+-rw-r--r--   0        0        0     1574 2023-06-03 02:44:02.036574 pubmed_types-0.1.1/src/pubmed_types/models/col.py
+-rw-r--r--   0        0        0      148 2023-06-03 02:44:02.804563 pubmed_types-0.1.1/src/pubmed_types/models/col_align.py
+-rw-r--r--   0        0        0      133 2023-06-03 02:44:02.804563 pubmed_types-0.1.1/src/pubmed_types/models/col_valign.py
+-rw-r--r--   0        0        0     1765 2023-06-03 02:44:02.040573 pubmed_types-0.1.1/src/pubmed_types/models/colgroup.py
+-rw-r--r--   0        0        0      153 2023-06-03 02:44:02.808563 pubmed_types-0.1.1/src/pubmed_types/models/colgroup_align.py
+-rw-r--r--   0        0        0      138 2023-06-03 02:44:02.808563 pubmed_types-0.1.1/src/pubmed_types/models/colgroup_valign.py
+-rw-r--r--   0        0        0     1450 2023-06-03 02:44:02.596566 pubmed_types-0.1.1/src/pubmed_types/models/collection_title.py
+-rw-r--r--   0        0        0      965 2023-06-03 02:44:02.600566 pubmed_types-0.1.1/src/pubmed_types/models/collective_name.py
+-rw-r--r--   0        0        0      934 2023-06-03 02:44:02.600566 pubmed_types-0.1.1/src/pubmed_types/models/comments_corrections.py
+-rw-r--r--   0        0        0      424 2023-06-03 02:44:02.600566 pubmed_types-0.1.1/src/pubmed_types/models/comments_corrections_list.py
+-rw-r--r--   0        0        0     1025 2023-06-03 02:44:02.840563 pubmed_types-0.1.1/src/pubmed_types/models/comments_corrections_ref_type.py
+-rw-r--r--   0        0        0     7391 2023-06-03 02:44:02.052573 pubmed_types-0.1.1/src/pubmed_types/models/conf_num.py
+-rw-r--r--   0        0        0     7394 2023-06-03 02:44:02.064573 pubmed_types-0.1.1/src/pubmed_types/models/conf_theme.py
+-rw-r--r--   0        0        0     4292 2023-06-03 02:44:02.068573 pubmed_types-0.1.1/src/pubmed_types/models/conference.py
+-rw-r--r--   0        0        0       82 2023-06-03 02:44:02.780563 pubmed_types-0.1.1/src/pubmed_types/models/contrib_corresp.py
+-rw-r--r--   0        0        0       83 2023-06-03 02:44:02.784563 pubmed_types-0.1.1/src/pubmed_types/models/contrib_deceased.py
+-rw-r--r--   0        0        0       87 2023-06-03 02:44:02.784563 pubmed_types-0.1.1/src/pubmed_types/models/contrib_equal_contrib.py
+-rw-r--r--   0        0        0     1940 2023-06-03 02:44:02.072573 pubmed_types-0.1.1/src/pubmed_types/models/contrib_id.py
+-rw-r--r--   0        0        0       98 2023-06-03 02:44:02.784563 pubmed_types-0.1.1/src/pubmed_types/models/contrib_id_authenticated.py
+-rw-r--r--   0        0        0     1889 2023-06-03 02:44:02.076573 pubmed_types-0.1.1/src/pubmed_types/models/contributed_resource_group.py
+-rw-r--r--   0        0        0      768 2023-06-03 02:44:02.600566 pubmed_types-0.1.1/src/pubmed_types/models/contribution_date.py
+-rw-r--r--   0        0        0     1083 2023-06-03 02:44:02.080573 pubmed_types-0.1.1/src/pubmed_types/models/copyright_year.py
+-rw-r--r--   0        0        0     8856 2023-06-03 02:44:02.092573 pubmed_types-0.1.1/src/pubmed_types/models/corresp.py
+-rw-r--r--   0        0        0      871 2023-06-03 02:44:02.096573 pubmed_types-0.1.1/src/pubmed_types/models/count.py
+-rw-r--r--   0        0        0     1907 2023-06-03 02:44:02.100573 pubmed_types-0.1.1/src/pubmed_types/models/counts.py
+-rw-r--r--   0        0        0     3702 2023-06-03 02:44:02.104573 pubmed_types-0.1.1/src/pubmed_types/models/custom_meta.py
+-rw-r--r--   0        0        0     1389 2023-06-03 02:44:02.108573 pubmed_types-0.1.1/src/pubmed_types/models/custom_meta_group.py
+-rw-r--r--   0        0        0      579 2023-06-03 02:44:02.604566 pubmed_types-0.1.1/src/pubmed_types/models/data_bank.py
+-rw-r--r--   0        0        0      644 2023-06-03 02:44:02.604566 pubmed_types-0.1.1/src/pubmed_types/models/data_bank_list.py
+-rw-r--r--   0        0        0       84 2023-06-03 02:44:02.836563 pubmed_types-0.1.1/src/pubmed_types/models/data_bank_list_complete_yn.py
+-rw-r--r--   0        0        0      672 2023-06-03 02:44:02.604566 pubmed_types-0.1.1/src/pubmed_types/models/date_completed.py
+-rw-r--r--   0        0        0      670 2023-06-03 02:44:02.604566 pubmed_types-0.1.1/src/pubmed_types/models/date_revised.py
+-rw-r--r--   0        0        0     1328 2023-06-03 02:44:02.108573 pubmed_types-0.1.1/src/pubmed_types/models/day.py
+-rw-r--r--   0        0        0      338 2023-06-03 02:44:02.564566 pubmed_types-0.1.1/src/pubmed_types/models/delete_citation.py
+-rw-r--r--   0        0        0      309 2023-06-03 02:44:02.564566 pubmed_types-0.1.1/src/pubmed_types/models/delete_document.py
+-rw-r--r--   0        0        0      948 2023-06-03 02:44:02.608566 pubmed_types-0.1.1/src/pubmed_types/models/descriptor_name.py
+-rw-r--r--   0        0        0       88 2023-06-03 02:44:02.840563 pubmed_types-0.1.1/src/pubmed_types/models/descriptor_name_major_topic_yn.py
+-rw-r--r--   0        0        0       86 2023-06-03 02:44:02.840563 pubmed_types-0.1.1/src/pubmed_types/models/descriptor_name_type.py
+-rw-r--r--   0        0        0      331 2023-06-03 02:44:02.884562 pubmed_types-0.1.1/src/pubmed_types/models/disp_formula_1.py
+-rw-r--r--   0        0        0     1217 2023-06-03 02:44:02.112573 pubmed_types-0.1.1/src/pubmed_types/models/elocation_id.py
+-rw-r--r--   0        0        0      809 2023-06-03 02:44:02.884562 pubmed_types-0.1.1/src/pubmed_types/models/elocation_id_1.py
+-rw-r--r--   0        0        0       88 2023-06-03 02:44:02.832563 pubmed_types-0.1.1/src/pubmed_types/models/elocation_id_eid_type.py
+-rw-r--r--   0        0        0       80 2023-06-03 02:44:02.832563 pubmed_types-0.1.1/src/pubmed_types/models/elocation_id_valid_yn.py
+-rw-r--r--   0        0        0      762 2023-06-03 02:44:02.608566 pubmed_types-0.1.1/src/pubmed_types/models/ending_date.py
+-rw-r--r--   0        0        0      704 2023-06-03 02:44:02.116572 pubmed_types-0.1.1/src/pubmed_types/models/equation_count.py
+-rw-r--r--   0        0        0     1328 2023-06-03 02:44:02.116572 pubmed_types-0.1.1/src/pubmed_types/models/era.py
+-rw-r--r--   0        0        0     3816 2023-06-03 02:44:02.124572 pubmed_types-0.1.1/src/pubmed_types/models/event.py
+-rw-r--r--   0        0        0     3116 2023-06-03 02:44:02.132572 pubmed_types-0.1.1/src/pubmed_types/models/event_desc.py
+-rw-r--r--   0        0        0     3131 2023-06-03 02:44:02.136572 pubmed_types-0.1.1/src/pubmed_types/models/extended_by.py
+-rw-r--r--   0        0        0      692 2023-06-03 02:44:02.140572 pubmed_types-0.1.1/src/pubmed_types/models/fig_count.py
+-rw-r--r--   0        0        0      111 2023-06-03 02:44:02.796563 pubmed_types-0.1.1/src/pubmed_types/models/fig_group_orientation.py
+-rw-r--r--   0        0        0      148 2023-06-03 02:44:02.796563 pubmed_types-0.1.1/src/pubmed_types/models/fig_group_position.py
+-rw-r--r--   0        0        0      106 2023-06-03 02:44:02.792563 pubmed_types-0.1.1/src/pubmed_types/models/fig_orientation.py
+-rw-r--r--   0        0        0      143 2023-06-03 02:44:02.792563 pubmed_types-0.1.1/src/pubmed_types/models/fig_position.py
+-rw-r--r--   0        0        0      467 2023-06-03 02:18:03.781929 pubmed_types-0.1.1/src/pubmed_types/models/first_name.py
+-rw-r--r--   0        0        0       78 2023-06-03 02:18:04.049925 pubmed_types-0.1.1/src/pubmed_types/models/first_name_empty_yn.py
+-rw-r--r--   0        0        0      458 2023-06-03 02:18:03.777929 pubmed_types-0.1.1/src/pubmed_types/models/first_page.py
+-rw-r--r--   0        0        0      112 2023-06-03 02:18:04.045925 pubmed_types-0.1.1/src/pubmed_types/models/first_page_lzero.py
+-rw-r--r--   0        0        0     2865 2023-06-03 02:44:02.144572 pubmed_types-0.1.1/src/pubmed_types/models/floats_group.py
+-rw-r--r--   0        0        0     1461 2023-06-03 02:44:02.148572 pubmed_types-0.1.1/src/pubmed_types/models/fpage.py
+-rw-r--r--   0        0        0     2105 2023-06-03 02:44:02.156572 pubmed_types-0.1.1/src/pubmed_types/models/front.py
+-rw-r--r--   0        0        0     9514 2023-06-03 02:44:02.168572 pubmed_types-0.1.1/src/pubmed_types/models/front_stub.py
+-rw-r--r--   0        0        0     1657 2023-06-03 02:44:02.168572 pubmed_types-0.1.1/src/pubmed_types/models/funding_group.py
+-rw-r--r--   0        0        0     9232 2023-06-03 02:44:02.184572 pubmed_types-0.1.1/src/pubmed_types/models/funding_statement.py
+-rw-r--r--   0        0        0      327 2023-06-03 02:44:02.608566 pubmed_types-0.1.1/src/pubmed_types/models/gene_symbol_list.py
+-rw-r--r--   0        0        0      465 2023-06-03 02:44:02.612566 pubmed_types-0.1.1/src/pubmed_types/models/general_note.py
+-rw-r--r--   0        0        0      152 2023-06-03 02:44:02.844563 pubmed_types-0.1.1/src/pubmed_types/models/general_note_owner.py
+-rw-r--r--   0        0        0     1866 2023-06-03 02:44:02.184572 pubmed_types-0.1.1/src/pubmed_types/models/glyph_data.py
+-rw-r--r--   0        0        0      728 2023-06-03 02:44:02.188572 pubmed_types-0.1.1/src/pubmed_types/models/glyph_ref.py
+-rw-r--r--   0        0        0      806 2023-06-03 02:44:02.612566 pubmed_types-0.1.1/src/pubmed_types/models/grant.py
+-rw-r--r--   0        0        0      611 2023-06-03 02:44:02.612566 pubmed_types-0.1.1/src/pubmed_types/models/grant_list.py
+-rw-r--r--   0        0        0       81 2023-06-03 02:44:02.836563 pubmed_types-0.1.1/src/pubmed_types/models/grant_list_complete_yn.py
+-rw-r--r--   0        0        0      110 2023-06-03 02:44:02.792563 pubmed_types-0.1.1/src/pubmed_types/models/graphic_orientation.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.792563 pubmed_types-0.1.1/src/pubmed_types/models/graphic_position.py
+-rw-r--r--   0        0        0      551 2023-06-03 02:18:03.805928 pubmed_types-0.1.1/src/pubmed_types/models/group.py
+-rw-r--r--   0        0        0      338 2023-06-03 02:18:03.805928 pubmed_types-0.1.1/src/pubmed_types/models/group_list.py
+-rw-r--r--   0        0        0      425 2023-06-03 02:44:02.888562 pubmed_types-0.1.1/src/pubmed_types/models/history_1.py
+-rw-r--r--   0        0        0     7177 2023-06-03 02:44:02.908562 pubmed_types-0.1.1/src/pubmed_types/models/history_2.py
+-rw-r--r--   0        0        0      528 2023-06-03 02:44:02.192571 pubmed_types-0.1.1/src/pubmed_types/models/hr.py
+-rw-r--r--   0        0        0     3870 2023-06-03 02:18:03.805928 pubmed_types-0.1.1/src/pubmed_types/models/i.py
+-rw-r--r--   0        0        0      426 2023-06-03 02:44:02.616566 pubmed_types-0.1.1/src/pubmed_types/models/identifier.py
+-rw-r--r--   0        0        0      718 2023-06-03 02:44:02.192571 pubmed_types-0.1.1/src/pubmed_types/models/index_term_range_end.py
+-rw-r--r--   0        0        0     1475 2023-06-03 02:18:03.809928 pubmed_types-0.1.1/src/pubmed_types/models/individual_name.py
+-rw-r--r--   0        0        0     2029 2023-06-03 02:44:02.200571 pubmed_types-0.1.1/src/pubmed_types/models/institution_id.py
+-rw-r--r--   0        0        0     1537 2023-06-03 02:44:02.616566 pubmed_types-0.1.1/src/pubmed_types/models/investigator.py
+-rw-r--r--   0        0        0      380 2023-06-03 02:44:02.616566 pubmed_types-0.1.1/src/pubmed_types/models/investigator_list.py
+-rw-r--r--   0        0        0       81 2023-06-03 02:44:02.844563 pubmed_types-0.1.1/src/pubmed_types/models/investigator_valid_yn.py
+-rw-r--r--   0        0        0      515 2023-06-03 02:44:02.908562 pubmed_types-0.1.1/src/pubmed_types/models/issn_1.py
+-rw-r--r--   0        0        0      100 2023-06-03 02:44:02.828563 pubmed_types-0.1.1/src/pubmed_types/models/issn_issn_type.py
+-rw-r--r--   0        0        0     3124 2023-06-03 02:44:02.204571 pubmed_types-0.1.1/src/pubmed_types/models/issue_id.py
+-rw-r--r--   0        0        0     7395 2023-06-03 02:44:02.216571 pubmed_types-0.1.1/src/pubmed_types/models/issue_sponsor.py
+-rw-r--r--   0        0        0     7400 2023-06-03 02:44:02.228571 pubmed_types-0.1.1/src/pubmed_types/models/issue_subtitle.py
+-rw-r--r--   0        0        0     1874 2023-06-03 02:44:02.228571 pubmed_types-0.1.1/src/pubmed_types/models/issue_title_group.py
+-rw-r--r--   0        0        0       80 2023-06-03 02:44:02.768564 pubmed_types-0.1.1/src/pubmed_types/models/italic_toggle.py
+-rw-r--r--   0        0        0      508 2023-06-03 02:44:02.620566 pubmed_types-0.1.1/src/pubmed_types/models/item_list.py
+-rw-r--r--   0        0        0      873 2023-06-03 02:44:02.620566 pubmed_types-0.1.1/src/pubmed_types/models/journal.py
+-rw-r--r--   0        0        0     1543 2023-06-03 02:44:02.232571 pubmed_types-0.1.1/src/pubmed_types/models/journal_id.py
+-rw-r--r--   0        0        0      942 2023-06-03 02:44:02.620566 pubmed_types-0.1.1/src/pubmed_types/models/journal_issue.py
+-rw-r--r--   0        0        0      107 2023-06-03 02:44:02.832563 pubmed_types-0.1.1/src/pubmed_types/models/journal_issue_cited_medium.py
+-rw-r--r--   0        0        0     2752 2023-06-03 02:44:02.236571 pubmed_types-0.1.1/src/pubmed_types/models/journal_meta.py
+-rw-r--r--   0        0        0     7406 2023-06-03 02:44:02.252570 pubmed_types-0.1.1/src/pubmed_types/models/journal_subtitle.py
+-rw-r--r--   0        0        0     7404 2023-06-03 02:44:02.264570 pubmed_types-0.1.1/src/pubmed_types/models/journal_title.py
+-rw-r--r--   0        0        0     1683 2023-06-03 02:44:02.268570 pubmed_types-0.1.1/src/pubmed_types/models/journal_title_group.py
+-rw-r--r--   0        0        0     1342 2023-06-03 02:44:02.624565 pubmed_types-0.1.1/src/pubmed_types/models/keyword.py
+-rw-r--r--   0        0        0      601 2023-06-03 02:44:02.624565 pubmed_types-0.1.1/src/pubmed_types/models/keyword_list.py
+-rw-r--r--   0        0        0      184 2023-06-03 02:44:02.844563 pubmed_types-0.1.1/src/pubmed_types/models/keyword_list_owner.py
+-rw-r--r--   0        0        0       81 2023-06-03 02:44:02.844563 pubmed_types-0.1.1/src/pubmed_types/models/keyword_major_topic_yn.py
+-rw-r--r--   0        0        0      460 2023-06-03 02:44:02.624565 pubmed_types-0.1.1/src/pubmed_types/models/location_label.py
+-rw-r--r--   0        0        0      205 2023-06-03 02:44:02.852563 pubmed_types-0.1.1/src/pubmed_types/models/location_label_type.py
+-rw-r--r--   0        0        0     1338 2023-06-03 02:44:02.272570 pubmed_types-0.1.1/src/pubmed_types/models/lpage.py
+-rw-r--r--   0        0        0      108 2023-06-03 02:44:02.792563 pubmed_types-0.1.1/src/pubmed_types/models/media_orientation.py
+-rw-r--r--   0        0        0      145 2023-06-03 02:44:02.796563 pubmed_types-0.1.1/src/pubmed_types/models/media_position.py
+-rw-r--r--   0        0        0     5578 2023-06-03 02:44:02.568566 pubmed_types-0.1.1/src/pubmed_types/models/medline_citation.py
+-rw-r--r--   0        0        0      178 2023-06-03 02:44:02.828563 pubmed_types-0.1.1/src/pubmed_types/models/medline_citation_owner.py
+-rw-r--r--   0        0        0      284 2023-06-03 02:44:02.828563 pubmed_types-0.1.1/src/pubmed_types/models/medline_citation_status.py
+-rw-r--r--   0        0        0      813 2023-06-03 02:44:02.624565 pubmed_types-0.1.1/src/pubmed_types/models/medline_journal_info.py
+-rw-r--r--   0        0        0      618 2023-06-03 02:44:02.628565 pubmed_types-0.1.1/src/pubmed_types/models/mesh_heading.py
+-rw-r--r--   0        0        0      376 2023-06-03 02:44:02.628565 pubmed_types-0.1.1/src/pubmed_types/models/mesh_heading_list.py
+-rw-r--r--   0        0        0     6803 2023-06-03 02:44:02.284570 pubmed_types-0.1.1/src/pubmed_types/models/meta_name.py
+-rw-r--r--   0        0        0     6806 2023-06-03 02:44:02.296570 pubmed_types-0.1.1/src/pubmed_types/models/meta_value.py
+-rw-r--r--   0        0        0     1408 2023-06-03 02:44:02.300570 pubmed_types-0.1.1/src/pubmed_types/models/milestone_end.py
+-rw-r--r--   0        0        0     1414 2023-06-03 02:44:02.304570 pubmed_types-0.1.1/src/pubmed_types/models/milestone_start.py
+-rw-r--r--   0        0        0       83 2023-06-03 02:44:02.772564 pubmed_types-0.1.1/src/pubmed_types/models/monospace_toggle.py
+-rw-r--r--   0        0        0     1334 2023-06-03 02:44:02.304570 pubmed_types-0.1.1/src/pubmed_types/models/month.py
+-rw-r--r--   0        0        0      153 2023-06-03 02:44:02.784563 pubmed_types-0.1.1/src/pubmed_types/models/name_name_style.py
+-rw-r--r--   0        0        0      423 2023-06-03 02:44:02.628565 pubmed_types-0.1.1/src/pubmed_types/models/name_of_substance.py
+-rw-r--r--   0        0        0     1422 2023-06-03 02:44:02.308570 pubmed_types-0.1.1/src/pubmed_types/models/object_id.py
+-rw-r--r--   0        0        0      354 2023-06-03 02:44:02.632565 pubmed_types-0.1.1/src/pubmed_types/models/object_list.py
+-rw-r--r--   0        0        0      497 2023-06-03 02:44:02.632565 pubmed_types-0.1.1/src/pubmed_types/models/object_mod.py
+-rw-r--r--   0        0        0       81 2023-06-03 02:44:02.820563 pubmed_types-0.1.1/src/pubmed_types/models/option_correct.py
+-rw-r--r--   0        0        0       15 2023-06-03 02:17:59.961981 pubmed_types-0.1.1/src/pubmed_types/models/org/__init__.py
+-rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.1/src/pubmed_types/models/org/niso/__init__.py
+-rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.1/src/pubmed_types/models/org/niso/schemas/__init__.py
+-rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.1/src/pubmed_types/models/org/niso/schemas/ali/__init__.py
+-rw-r--r--   0        0        0      124 2023-06-03 02:43:58.380623 pubmed_types-0.1.1/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/__init__.py
+-rw-r--r--   0        0        0      631 2023-06-03 02:44:02.552566 pubmed_types-0.1.1/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/free_to_read.py
+-rw-r--r--   0        0        0      578 2023-06-03 02:44:02.552566 pubmed_types-0.1.1/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/license_ref.py
+-rw-r--r--   0        0        0       15 2023-06-03 02:17:59.961981 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/__init__.py
+-rw-r--r--   0        0        0       15 2023-06-03 02:17:59.989981 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/__init__.py
+-rw-r--r--   0        0        0       15 2023-06-03 02:17:59.989981 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/__init__.py
+-rw-r--r--   0        0        0    18558 2023-06-03 02:43:58.344624 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/__init__.py
+-rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.116600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/abs.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.132599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/and_mod.py
+-rw-r--r--   0        0        0     2149 2023-06-03 02:44:00.364596 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/annotation.py
+-rw-r--r--   0        0        0     1582 2023-06-03 02:44:00.148599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/approx.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.184599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccos.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.184599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccosh.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.184599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccot.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.188599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccoth.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.188599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccsc.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.188599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccsch.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.188599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arcsec.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.188599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arcsech.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.180599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arcsin.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.192599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arcsinh.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.184599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arctan.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.192599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arctanh.py
+-rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.120600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arg.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.164599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/card.py
+-rw-r--r--   0        0        0      466 2023-06-03 02:44:00.160599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cartesianproduct.py
+-rw-r--r--   0        0        0     1737 2023-06-03 02:44:00.092600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cbytes.py
+-rw-r--r--   0        0        0     1584 2023-06-03 02:44:00.128600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ceiling.py
+-rw-r--r--   0        0        0      450 2023-06-03 02:44:00.096600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/codomain.py
+-rw-r--r--   0        0        0      168 2023-06-03 02:44:00.224598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/columnalignstyle.py
+-rw-r--r--   0        0        0      452 2023-06-03 02:44:00.208598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/complexes.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.104600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/compose.py
+-rw-r--r--   0        0        0  1555308 2023-06-03 02:44:00.088600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/condition.py
+-rw-r--r--   0        0        0     1588 2023-06-03 02:44:00.120600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/conjugate.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cos.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.176599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cosh.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.176599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cot.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.180599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/coth.py
+-rw-r--r--   0        0        0     1767 2023-06-03 02:44:00.092600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cs.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/csc.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.180599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/csch.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.156599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/curl.py
+-rw-r--r--   0        0        0      189 2023-06-03 02:44:02.664565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/declare_occurrence.py
+-rw-r--r--   0        0        0      456 2023-06-03 02:44:00.196599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/determinant.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.152599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/diff.py
+-rw-r--r--   0        0        0      454 2023-06-03 02:44:00.156599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/divergence.py
+-rw-r--r--   0        0        0     1582 2023-06-03 02:44:00.108600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/divide.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.096600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/domain.py
+-rw-r--r--   0        0        0      450 2023-06-03 02:44:00.208598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/emptyset.py
+-rw-r--r--   0        0        0      438 2023-06-03 02:44:00.140599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/eq.py
+-rw-r--r--   0        0        0      454 2023-06-03 02:44:00.140599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/equivalent.py
+-rw-r--r--   0        0        0      454 2023-06-03 02:44:00.216598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/eulergamma.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.140599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/exists.py
+-rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.128600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/exp.py
+-rw-r--r--   0        0        0      458 2023-06-03 02:44:00.208598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/exponentiale.py
+-rw-r--r--   0        0        0     1588 2023-06-03 02:44:00.116600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/factorial.py
+-rw-r--r--   0        0        0     1586 2023-06-03 02:44:00.148599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/factorof.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.212598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/false.py
+-rw-r--r--   0        0        0     1580 2023-06-03 02:44:00.124600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/floor.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.140599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/forall.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.132599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/gcd.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.144599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/geq.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.156599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/grad.py
+-rw-r--r--   0        0        0      438 2023-06-03 02:44:00.140599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/gt.py
+-rw-r--r--   0        0        0      444 2023-06-03 02:44:00.096600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ident.py
+-rw-r--r--   0        0        0      444 2023-06-03 02:44:00.100600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/image.py
+-rw-r--r--   0        0        0     1588 2023-06-03 02:44:00.124600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/imaginary.py
+-rw-r--r--   0        0        0      454 2023-06-03 02:44:00.212598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/imaginaryi.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.136599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/implies.py
+-rw-r--r--   0        0        0      438 2023-06-03 02:44:00.160599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/in_mod.py
+-rw-r--r--   0        0        0      450 2023-06-03 02:44:00.216598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/infinity.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.152599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/int_mod.py
+-rw-r--r--   0        0        0      450 2023-06-03 02:44:00.204599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/integers.py
+-rw-r--r--   0        0        0      452 2023-06-03 02:44:00.160599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/intersect.py
+-rw-r--r--   0        0        0      450 2023-06-03 02:44:00.096600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/interval.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.096600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/inverse.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.100600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/lambda_mod.py
+-rw-r--r--   0        0        0      452 2023-06-03 02:44:00.156599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/laplacian.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.132599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/lcm.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.144599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/leq.py
+-rw-r--r--   0        0        0      444 2023-06-03 02:44:00.168599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/limit.py
+-rw-r--r--   0        0        0      161 2023-06-03 02:44:00.224598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/linestyle.py
+-rw-r--r--   0        0        0      161 2023-06-03 02:44:02.664565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/list_order.py
+-rw-r--r--   0        0        0      438 2023-06-03 02:44:00.100600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ln.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.100600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/log.py
+-rw-r--r--   0        0        0      438 2023-06-03 02:44:00.140599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/lt.py
+-rw-r--r--   0        0        0      136 2023-06-03 02:44:02.664565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maction_value.py
+-rw-r--r--   0        0        0     2637 2023-06-03 02:44:00.268597 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maligngroup.py
+-rw-r--r--   0        0        0      207 2023-06-03 02:44:02.708564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maligngroup_groupalign.py
+-rw-r--r--   0        0        0      140 2023-06-03 02:44:02.708564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maligngroup_value.py
+-rw-r--r--   0        0        0     2605 2023-06-03 02:44:00.264598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/malignmark.py
+-rw-r--r--   0        0        0      144 2023-06-03 02:44:02.708564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/malignmark_edge.py
+-rw-r--r--   0        0        0      139 2023-06-03 02:44:02.708564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/malignmark_value.py
+-rw-r--r--   0        0        0    74524 2023-06-03 02:44:00.364596 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math.py
+-rw-r--r--   0        0        0      140 2023-06-03 02:44:02.744564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_accent.py
+-rw-r--r--   0        0        0      145 2023-06-03 02:44:02.744564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_accentunder.py
+-rw-r--r--   0        0        0      161 2023-06-03 02:44:02.744564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_align.py
+-rw-r--r--   0        0        0      142 2023-06-03 02:44:02.744564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_bevelled.py
+-rw-r--r--   0        0        0      165 2023-06-03 02:44:02.744564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_charalign.py
+-rw-r--r--   0        0        0      166 2023-06-03 02:44:02.744564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_denomalign.py
+-rw-r--r--   0        0        0      131 2023-06-03 02:44:02.748564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_dir.py
+-rw-r--r--   0        0        0      145 2023-06-03 02:44:02.768564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_display.py
+-rw-r--r--   0        0        0      146 2023-06-03 02:44:02.744564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_displaystyle.py
+-rw-r--r--   0        0        0      138 2023-06-03 02:44:02.748564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_edge.py
+-rw-r--r--   0        0        0      146 2023-06-03 02:44:02.748564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_equalcolumns.py
+-rw-r--r--   0        0        0      143 2023-06-03 02:44:02.748564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_equalrows.py
+-rw-r--r--   0        0        0      139 2023-06-03 02:44:02.748564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_fence.py
+-rw-r--r--   0        0        0      166 2023-06-03 02:44:02.748564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_form.py
+-rw-r--r--   0        0        0      199 2023-06-03 02:44:02.752564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_indentalign.py
+-rw-r--r--   0        0        0      236 2023-06-03 02:44:02.752564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_indentalignfirst.py
+-rw-r--r--   0        0        0      235 2023-06-03 02:44:02.752564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_indentalignlast.py
+-rw-r--r--   0        0        0      185 2023-06-03 02:44:02.744564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_infixlinebreakstyle.py
+-rw-r--r--   0        0        0      141 2023-06-03 02:44:02.752564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_largeop.py
+-rw-r--r--   0        0        0      225 2023-06-03 02:44:02.752564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_linebreak.py
+-rw-r--r--   0        0        0      228 2023-06-03 02:44:02.756564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_linebreakstyle.py
+-rw-r--r--   0        0        0      208 2023-06-03 02:44:02.756564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_location.py
+-rw-r--r--   0        0        0      495 2023-06-03 02:44:02.756564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_longdivstyle.py
+-rw-r--r--   0        0        0      641 2023-06-03 02:44:02.760564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_mathvariant.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.760564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_movablelimits.py
+-rw-r--r--   0        0        0      164 2023-06-03 02:44:02.760564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_numalign.py
+-rw-r--r--   0        0        0      220 2023-06-03 02:44:02.768564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_overflow.py
+-rw-r--r--   0        0        0      143 2023-06-03 02:44:02.760564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_separator.py
+-rw-r--r--   0        0        0      204 2023-06-03 02:44:02.760564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_side.py
+-rw-r--r--   0        0        0      200 2023-06-03 02:44:02.764564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_stackalign.py
+-rw-r--r--   0        0        0      142 2023-06-03 02:44:02.764564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_stretchy.py
+-rw-r--r--   0        0        0      143 2023-06-03 02:44:02.764564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_symmetric.py
+-rw-r--r--   0        0        0      117 2023-06-03 02:44:02.740564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_value.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.196599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/matrix.py
+-rw-r--r--   0        0        0      452 2023-06-03 02:44:00.196599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/matrixrow.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.128600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/max.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.192599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mean.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.192599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/median.py
+-rw-r--r--   0        0        0      137 2023-06-03 02:44:02.680565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/menclose_value.py
+-rw-r--r--   0        0        0      135 2023-06-03 02:44:02.680565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/merror_value.py
+-rw-r--r--   0        0        0      136 2023-06-03 02:44:02.680565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfenced_value.py
+-rw-r--r--   0        0        0      143 2023-06-03 02:44:02.704564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfrac_bevelled.py
+-rw-r--r--   0        0        0      167 2023-06-03 02:44:02.704564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfrac_denomalign.py
+-rw-r--r--   0        0        0      165 2023-06-03 02:44:02.704564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfrac_numalign.py
+-rw-r--r--   0        0        0      120 2023-06-03 02:44:02.704564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfrac_value.py
+-rw-r--r--   0        0        0     5862 2023-06-03 02:44:00.256598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph.py
+-rw-r--r--   0        0        0      151 2023-06-03 02:44:02.660565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_fontstyle.py
+-rw-r--r--   0        0        0      148 2023-06-03 02:44:02.660565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_fontweight.py
+-rw-r--r--   0        0        0      643 2023-06-03 02:44:02.660565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_mathvariant.py
+-rw-r--r--   0        0        0      135 2023-06-03 02:44:02.660565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_value.py
+-rw-r--r--   0        0        0     5329 2023-06-03 02:44:00.228598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi.py
+-rw-r--r--   0        0        0      129 2023-06-03 02:44:02.732564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_dir.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.736564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_fontstyle.py
+-rw-r--r--   0        0        0      144 2023-06-03 02:44:02.732564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_fontweight.py
+-rw-r--r--   0        0        0      639 2023-06-03 02:44:02.732564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_mathvariant.py
+-rw-r--r--   0        0        0      131 2023-06-03 02:44:02.732564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_value.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.132599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/min.py
+-rw-r--r--   0        0        0     1580 2023-06-03 02:44:00.108600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/minus.py
+-rw-r--r--   0        0        0     3231 2023-06-03 02:44:00.276597 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlabeledtr.py
+-rw-r--r--   0        0        0      214 2023-06-03 02:44:02.736564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlabeledtr_rowalign.py
+-rw-r--r--   0        0        0      139 2023-06-03 02:44:02.736564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlabeledtr_value.py
+-rw-r--r--   0        0        0      499 2023-06-03 02:44:02.664565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlongdiv_longdivstyle.py
+-rw-r--r--   0        0        0      137 2023-06-03 02:44:02.664565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlongdiv_value.py
+-rw-r--r--   0        0        0      142 2023-06-03 02:44:02.672565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mmultiscripts_value.py
+-rw-r--r--   0        0        0     5329 2023-06-03 02:44:00.232598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn.py
+-rw-r--r--   0        0        0      129 2023-06-03 02:44:02.732564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_dir.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.732564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_fontstyle.py
+-rw-r--r--   0        0        0      144 2023-06-03 02:44:02.732564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_fontweight.py
+-rw-r--r--   0        0        0      639 2023-06-03 02:44:02.732564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_mathvariant.py
+-rw-r--r--   0        0        0      131 2023-06-03 02:44:02.728564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_value.py
+-rw-r--r--   0        0        0    10043 2023-06-03 02:44:00.240598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo.py
+-rw-r--r--   0        0        0      138 2023-06-03 02:44:02.724564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_accent.py
+-rw-r--r--   0        0        0      129 2023-06-03 02:44:02.720564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_dir.py
+-rw-r--r--   0        0        0      137 2023-06-03 02:44:02.724564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_fence.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.720564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_fontstyle.py
+-rw-r--r--   0        0        0      144 2023-06-03 02:44:02.720564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_fontweight.py
+-rw-r--r--   0        0        0      164 2023-06-03 02:44:02.724564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_form.py
+-rw-r--r--   0        0        0      197 2023-06-03 02:44:02.728564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_indentalign.py
+-rw-r--r--   0        0        0      234 2023-06-03 02:44:02.728564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_indentalignfirst.py
+-rw-r--r--   0        0        0      233 2023-06-03 02:44:02.728564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_indentalignlast.py
+-rw-r--r--   0        0        0      139 2023-06-03 02:44:02.724564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_largeop.py
+-rw-r--r--   0        0        0      223 2023-06-03 02:44:02.728564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_linebreak.py
+-rw-r--r--   0        0        0      226 2023-06-03 02:44:02.728564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_linebreakstyle.py
+-rw-r--r--   0        0        0      639 2023-06-03 02:44:02.720564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_mathvariant.py
+-rw-r--r--   0        0        0      145 2023-06-03 02:44:02.724564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_movablelimits.py
+-rw-r--r--   0        0        0      141 2023-06-03 02:44:02.724564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_separator.py
+-rw-r--r--   0        0        0      140 2023-06-03 02:44:02.724564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_stretchy.py
+-rw-r--r--   0        0        0      141 2023-06-03 02:44:02.724564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_symmetric.py
+-rw-r--r--   0        0        0      125 2023-06-03 02:44:02.720564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_value.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.196599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mode.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.100600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/moment.py
+-rw-r--r--   0        0        0      141 2023-06-03 02:44:02.676565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mover_accent.py
+-rw-r--r--   0        0        0      162 2023-06-03 02:44:02.676565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mover_align.py
+-rw-r--r--   0        0        0      134 2023-06-03 02:44:02.676565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mover_value.py
+-rw-r--r--   0        0        0      136 2023-06-03 02:44:02.680565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mpadded_value.py
+-rw-r--r--   0        0        0      137 2023-06-03 02:44:02.680565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mphantom_value.py
+-rw-r--r--   0        0        0     2432 2023-06-03 02:44:00.264598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mprescripts.py
+-rw-r--r--   0        0        0      140 2023-06-03 02:44:02.736564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mprescripts_value.py
+-rw-r--r--   0        0        0      134 2023-06-03 02:44:02.700564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mroot_value.py
+-rw-r--r--   0        0        0      131 2023-06-03 02:44:02.708564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mrow_dir.py
+-rw-r--r--   0        0        0      133 2023-06-03 02:44:02.704564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mrow_value.py
+-rw-r--r--   0        0        0     5585 2023-06-03 02:44:00.252598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms.py
+-rw-r--r--   0        0        0      129 2023-06-03 02:44:02.712564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_dir.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.712564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_fontstyle.py
+-rw-r--r--   0        0        0      144 2023-06-03 02:44:02.712564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_fontweight.py
+-rw-r--r--   0        0        0      639 2023-06-03 02:44:02.708564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_mathvariant.py
+-rw-r--r--   0        0        0      131 2023-06-03 02:44:02.708564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_value.py
+-rw-r--r--   0        0        0      213 2023-06-03 02:44:02.740564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mscarries_location.py
+-rw-r--r--   0        0        0      292 2023-06-03 02:44:02.740564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mscarries_value.py
+-rw-r--r--   0        0        0      211 2023-06-03 02:44:02.740564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mscarry_location.py
+-rw-r--r--   0        0        0      290 2023-06-03 02:44:02.740564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mscarry_value.py
+-rw-r--r--   0        0        0      136 2023-06-03 02:44:02.740564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msgroup_value.py
+-rw-r--r--   0        0        0     3475 2023-06-03 02:44:00.260598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msline.py
+-rw-r--r--   0        0        0      121 2023-06-03 02:44:02.740564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msline_value.py
+-rw-r--r--   0        0        0     5838 2023-06-03 02:44:00.248598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace.py
+-rw-r--r--   0        0        0      133 2023-06-03 02:44:02.712564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_dir.py
+-rw-r--r--   0        0        0      151 2023-06-03 02:44:02.716564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_fontstyle.py
+-rw-r--r--   0        0        0      148 2023-06-03 02:44:02.716564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_fontweight.py
+-rw-r--r--   0        0        0      269 2023-06-03 02:44:02.716564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_linebreak.py
+-rw-r--r--   0        0        0      643 2023-06-03 02:44:02.712564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_mathvariant.py
+-rw-r--r--   0        0        0      135 2023-06-03 02:44:02.712564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_value.py
+-rw-r--r--   0        0        0      134 2023-06-03 02:44:02.700564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msqrt_value.py
+-rw-r--r--   0        0        0      134 2023-06-03 02:44:02.740564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msrow_value.py
+-rw-r--r--   0        0        0      167 2023-06-03 02:44:02.664565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstack_charalign.py
+-rw-r--r--   0        0        0      202 2023-06-03 02:44:02.664565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstack_stackalign.py
+-rw-r--r--   0        0        0      123 2023-06-03 02:44:02.664565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstack_value.py
+-rw-r--r--   0        0        0      142 2023-06-03 02:44:02.684565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_accent.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.684565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_accentunder.py
+-rw-r--r--   0        0        0      163 2023-06-03 02:44:02.684565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_align.py
+-rw-r--r--   0        0        0      144 2023-06-03 02:44:02.684565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_bevelled.py
+-rw-r--r--   0        0        0      167 2023-06-03 02:44:02.684565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_charalign.py
+-rw-r--r--   0        0        0      168 2023-06-03 02:44:02.684565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_denomalign.py
+-rw-r--r--   0        0        0      133 2023-06-03 02:44:02.688565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_dir.py
+-rw-r--r--   0        0        0      148 2023-06-03 02:44:02.680565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_displaystyle.py
+-rw-r--r--   0        0        0      140 2023-06-03 02:44:02.688565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_edge.py
+-rw-r--r--   0        0        0      148 2023-06-03 02:44:02.688565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_equalcolumns.py
+-rw-r--r--   0        0        0      145 2023-06-03 02:44:02.688565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_equalrows.py
+-rw-r--r--   0        0        0      141 2023-06-03 02:44:02.688565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_fence.py
+-rw-r--r--   0        0        0      151 2023-06-03 02:44:02.700564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_fontstyle.py
+-rw-r--r--   0        0        0      148 2023-06-03 02:44:02.700564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_fontweight.py
+-rw-r--r--   0        0        0      168 2023-06-03 02:44:02.688565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_form.py
+-rw-r--r--   0        0        0      201 2023-06-03 02:44:02.692565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_indentalign.py
+-rw-r--r--   0        0        0      238 2023-06-03 02:44:02.692565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_indentalignfirst.py
+-rw-r--r--   0        0        0      237 2023-06-03 02:44:02.692565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_indentalignlast.py
+-rw-r--r--   0        0        0      187 2023-06-03 02:44:02.684565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_infixlinebreakstyle.py
+-rw-r--r--   0        0        0      143 2023-06-03 02:44:02.692565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_largeop.py
+-rw-r--r--   0        0        0      227 2023-06-03 02:44:02.692565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_linebreak.py
+-rw-r--r--   0        0        0      230 2023-06-03 02:44:02.692565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_linebreakstyle.py
+-rw-r--r--   0        0        0      210 2023-06-03 02:44:02.692565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_location.py
+-rw-r--r--   0        0        0      497 2023-06-03 02:44:02.696565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_longdivstyle.py
+-rw-r--r--   0        0        0      643 2023-06-03 02:44:02.696565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_mathvariant.py
+-rw-r--r--   0        0        0      149 2023-06-03 02:44:02.696565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_movablelimits.py
+-rw-r--r--   0        0        0      166 2023-06-03 02:44:02.696565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_numalign.py
+-rw-r--r--   0        0        0      145 2023-06-03 02:44:02.696565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_separator.py
+-rw-r--r--   0        0        0      206 2023-06-03 02:44:02.700564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_side.py
+-rw-r--r--   0        0        0      202 2023-06-03 02:44:02.700564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_stackalign.py
+-rw-r--r--   0        0        0      144 2023-06-03 02:44:02.700564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_stretchy.py
+-rw-r--r--   0        0        0      145 2023-06-03 02:44:02.700564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_symmetric.py
+-rw-r--r--   0        0        0      135 2023-06-03 02:44:02.680565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_value.py
+-rw-r--r--   0        0        0      133 2023-06-03 02:44:02.680565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msub_value.py
+-rw-r--r--   0        0        0      136 2023-06-03 02:44:02.676565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msubsup_value.py
+-rw-r--r--   0        0        0      133 2023-06-03 02:44:02.676565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msup_value.py
+-rw-r--r--   0        0        0     6510 2023-06-03 02:44:00.272597 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable.py
+-rw-r--r--   0        0        0      148 2023-06-03 02:44:02.668565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_displaystyle.py
+-rw-r--r--   0        0        0      148 2023-06-03 02:44:02.668565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_equalcolumns.py
+-rw-r--r--   0        0        0      145 2023-06-03 02:44:02.668565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_equalrows.py
+-rw-r--r--   0        0        0      206 2023-06-03 02:44:02.668565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_side.py
+-rw-r--r--   0        0        0      141 2023-06-03 02:44:02.668565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_value.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.280597 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtd.py
+-rw-r--r--   0        0        0     5386 2023-06-03 02:44:00.244598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext.py
+-rw-r--r--   0        0        0      132 2023-06-03 02:44:02.716564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_dir.py
+-rw-r--r--   0        0        0      150 2023-06-03 02:44:02.716564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_fontstyle.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.716564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_fontweight.py
+-rw-r--r--   0        0        0      642 2023-06-03 02:44:02.716564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_mathvariant.py
+-rw-r--r--   0        0        0      134 2023-06-03 02:44:02.716564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_value.py
+-rw-r--r--   0        0        0     3175 2023-06-03 02:44:00.280597 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtr.py
+-rw-r--r--   0        0        0      207 2023-06-03 02:44:02.672565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtr_rowalign.py
+-rw-r--r--   0        0        0      132 2023-06-03 02:44:02.668565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtr_value.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.676565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munder_accentunder.py
+-rw-r--r--   0        0        0      163 2023-06-03 02:44:02.676565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munder_align.py
+-rw-r--r--   0        0        0      135 2023-06-03 02:44:02.676565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munder_value.py
+-rw-r--r--   0        0        0      146 2023-06-03 02:44:02.672565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munderover_accent.py
+-rw-r--r--   0        0        0      151 2023-06-03 02:44:02.672565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munderover_accentunder.py
+-rw-r--r--   0        0        0      167 2023-06-03 02:44:02.672565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munderover_align.py
+-rw-r--r--   0        0        0      139 2023-06-03 02:44:02.672565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munderover_value.py
+-rw-r--r--   0        0        0      462 2023-06-03 02:44:00.204599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/naturalnumbers.py
+-rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.144599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/neq.py
+-rw-r--r--   0        0        0     2401 2023-06-03 02:44:00.260598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/none.py
+-rw-r--r--   0        0        0      133 2023-06-03 02:44:02.736564 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/none_value.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.136599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/not_mod.py
+-rw-r--r--   0        0        0      454 2023-06-03 02:44:00.212598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/notanumber.py
+-rw-r--r--   0        0        0      444 2023-06-03 02:44:00.160599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/notin.py
+-rw-r--r--   0        0        0      456 2023-06-03 02:44:00.164599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/notprsubset.py
+-rw-r--r--   0        0        0      452 2023-06-03 02:44:00.164599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/notsubset.py
+-rw-r--r--   0        0        0      438 2023-06-03 02:44:00.136599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/or_mod.py
+-rw-r--r--   0        0        0      458 2023-06-03 02:44:00.204599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/outerproduct.py
+-rw-r--r--   0        0        0      456 2023-06-03 02:44:00.156599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/partialdiff.py
+-rw-r--r--   0        0        0      438 2023-06-03 02:44:00.216598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/pi.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.132599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/plus.py
+-rw-r--r--   0        0        0     1580 2023-06-03 02:44:00.108600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/power.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.208598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/primes.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.168599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/product.py
+-rw-r--r--   0        0        0      450 2023-06-03 02:44:00.164599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/prsubset.py
+-rw-r--r--   0        0        0     1586 2023-06-03 02:44:00.104600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/quotient.py
+-rw-r--r--   0        0        0      452 2023-06-03 02:44:00.204599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/rationals.py
+-rw-r--r--   0        0        0     1578 2023-06-03 02:44:00.124600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/real.py
+-rw-r--r--   0        0        0      444 2023-06-03 02:44:00.204599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/reals.py
+-rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.112600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/rem.py
+-rw-r--r--   0        0        0     1578 2023-06-03 02:44:00.112600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/root.py
+-rw-r--r--   0        0        0      460 2023-06-03 02:44:00.200599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/scalarproduct.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.192599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sdev.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sec.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.180599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sech.py
+-rw-r--r--   0        0        0      450 2023-06-03 02:44:00.200599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/selector.py
+-rw-r--r--   0        0        0      215 2023-06-03 02:44:00.092600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sep.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.164599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/setdiff.py
+-rw-r--r--   0        0        0     1405 2023-06-03 02:44:00.088600 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/share.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sin.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.176599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sinh.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.164599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/subset.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.168599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sum.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/tan.py
+-rw-r--r--   0        0        0      442 2023-06-03 02:44:00.176599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/tanh.py
+-rw-r--r--   0        0        0     1710 2023-06-03 02:44:00.152599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/tendsto.py
+-rw-r--r--   0        0        0      444 2023-06-03 02:44:00.132599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/times.py
+-rw-r--r--   0        0        0      452 2023-06-03 02:44:00.200599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/transpose.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.212598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/true.py
+-rw-r--r--   0        0        0      448 2023-06-03 02:44:00.160599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/union.py
+-rw-r--r--   0        0        0      450 2023-06-03 02:44:00.192599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/variance.py
+-rw-r--r--   0        0        0      446 2023-06-03 02:44:00.196599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/vector.py
+-rw-r--r--   0        0        0      460 2023-06-03 02:44:00.200599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/vectorproduct.py
+-rw-r--r--   0        0        0      209 2023-06-03 02:44:00.224598 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/verticalalign.py
+-rw-r--r--   0        0        0      440 2023-06-03 02:44:00.136599 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/xor.py
+-rw-r--r--   0        0        0       15 2023-06-03 02:17:59.961981 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/__init__.py
+-rw-r--r--   0        0        0      488 2023-06-03 02:43:58.316624 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/__init__.py
+-rw-r--r--   0        0        0      188 2023-06-03 02:44:02.660565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/actuate_value.py
+-rw-r--r--   0        0        0     1893 2023-06-03 02:43:58.428623 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/arc_type.py
+-rw-r--r--   0        0        0     1169 2023-06-03 02:43:58.420623 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/extended.py
+-rw-r--r--   0        0        0     1453 2023-06-03 02:43:58.428623 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/locator_type.py
+-rw-r--r--   0        0        0     1244 2023-06-03 02:43:58.424623 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/resource_type.py
+-rw-r--r--   0        0        0      193 2023-06-03 02:44:02.660565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/show_value.py
+-rw-r--r--   0        0        0     1940 2023-06-03 02:43:58.416623 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/simple.py
+-rw-r--r--   0        0        0     1203 2023-06-03 02:43:58.424623 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/title_elt_type.py
+-rw-r--r--   0        0        0      247 2023-06-03 02:44:02.660565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/type_value.py
+-rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/xml/__init__.py
+-rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/xml/pkg_1998/__init__.py
+-rw-r--r--   0        0        0      120 2023-06-03 02:43:58.380623 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/xml/pkg_1998/namespace/__init__.py
+-rw-r--r--   0        0        0      118 2023-06-03 02:44:02.656565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/xml/pkg_1998/namespace/lang_value.py
+-rw-r--r--   0        0        0      154 2023-06-03 02:44:02.656565 pubmed_types-0.1.1/src/pubmed_types/models/org/w3/xml/pkg_1998/namespace/space_value.py
+-rw-r--r--   0        0        0      997 2023-06-03 02:44:02.632565 pubmed_types-0.1.1/src/pubmed_types/models/other_abstract.py
+-rw-r--r--   0        0        0      223 2023-06-03 02:44:02.844563 pubmed_types-0.1.1/src/pubmed_types/models/other_abstract_type.py
+-rw-r--r--   0        0        0      518 2023-06-03 02:44:02.632565 pubmed_types-0.1.1/src/pubmed_types/models/other_id.py
+-rw-r--r--   0        0        0      257 2023-06-03 02:44:02.840563 pubmed_types-0.1.1/src/pubmed_types/models/other_id_source.py
+-rw-r--r--   0        0        0      863 2023-06-03 02:44:02.312570 pubmed_types-0.1.1/src/pubmed_types/models/overline_end.py
+-rw-r--r--   0        0        0      747 2023-06-03 02:44:02.312570 pubmed_types-0.1.1/src/pubmed_types/models/overline_start.py
+-rw-r--r--   0        0        0       82 2023-06-03 02:44:02.772564 pubmed_types-0.1.1/src/pubmed_types/models/overline_toggle.py
+-rw-r--r--   0        0        0      692 2023-06-03 02:44:02.316570 pubmed_types-0.1.1/src/pubmed_types/models/page_count.py
+-rw-r--r--   0        0        0     1349 2023-06-03 02:44:02.320570 pubmed_types-0.1.1/src/pubmed_types/models/page_range.py
+-rw-r--r--   0        0        0      649 2023-06-03 02:44:02.636565 pubmed_types-0.1.1/src/pubmed_types/models/pagination.py
+-rw-r--r--   0        0        0     1147 2023-06-03 02:44:02.636565 pubmed_types-0.1.1/src/pubmed_types/models/param.py
+-rw-r--r--   0        0        0      831 2023-06-03 02:44:02.640565 pubmed_types-0.1.1/src/pubmed_types/models/personal_name_subject.py
+-rw-r--r--   0        0        0      426 2023-06-03 02:44:02.640565 pubmed_types-0.1.1/src/pubmed_types/models/personal_name_subject_list.py
+-rw-r--r--   0        0        0      461 2023-06-03 02:44:02.632565 pubmed_types-0.1.1/src/pubmed_types/models/pmid.py
+-rw-r--r--   0        0        0     1366 2023-06-03 02:44:02.320570 pubmed_types-0.1.1/src/pubmed_types/models/postal_code.py
+-rw-r--r--   0        0        0      112 2023-06-03 02:44:02.796563 pubmed_types-0.1.1/src/pubmed_types/models/preformat_orientation.py
+-rw-r--r--   0        0        0      149 2023-06-03 02:44:02.796563 pubmed_types-0.1.1/src/pubmed_types/models/preformat_position.py
+-rw-r--r--   0        0        0     2142 2023-06-03 02:44:02.324570 pubmed_types-0.1.1/src/pubmed_types/models/principal_award_recipient.py
+-rw-r--r--   0        0        0     1855 2023-06-03 02:44:02.328570 pubmed_types-0.1.1/src/pubmed_types/models/principal_investigator.py
+-rw-r--r--   0        0        0     2483 2023-06-03 02:44:02.332569 pubmed_types-0.1.1/src/pubmed_types/models/processing_meta.py
+-rw-r--r--   0        0        0      148 2023-06-03 02:44:02.824563 pubmed_types-0.1.1/src/pubmed_types/models/processing_meta_base_tagset.py
+-rw-r--r--   0        0        0      109 2023-06-03 02:44:02.824563 pubmed_types-0.1.1/src/pubmed_types/models/processing_meta_mathml_version.py
+-rw-r--r--   0        0        0      138 2023-06-03 02:44:02.824563 pubmed_types-0.1.1/src/pubmed_types/models/processing_meta_table_model.py
+-rw-r--r--   0        0        0      116 2023-06-03 02:44:02.828563 pubmed_types-0.1.1/src/pubmed_types/models/processing_meta_tagset_family.py
+-rw-r--r--   0        0        0      936 2023-06-03 02:44:02.912562 pubmed_types-0.1.1/src/pubmed_types/models/pub_date_1.py
+-rw-r--r--   0        0        0     2895 2023-06-03 02:44:02.916561 pubmed_types-0.1.1/src/pubmed_types/models/pub_date_2.py
+-rw-r--r--   0        0        0      740 2023-06-03 02:44:02.332569 pubmed_types-0.1.1/src/pubmed_types/models/pub_date_not_available.py
+-rw-r--r--   0        0        0      408 2023-06-03 02:18:04.041925 pubmed_types-0.1.1/src/pubmed_types/models/pub_date_pub_status.py
+-rw-r--r--   0        0        0      708 2023-06-03 02:44:02.336569 pubmed_types-0.1.1/src/pubmed_types/models/pub_history.py
+-rw-r--r--   0        0        0     2871 2023-06-03 02:44:02.340569 pubmed_types-0.1.1/src/pubmed_types/models/pub_id.py
+-rw-r--r--   0        0        0     1462 2023-06-03 02:44:02.644565 pubmed_types-0.1.1/src/pubmed_types/models/pub_med_pub_date.py
+-rw-r--r--   0        0        0      496 2023-06-03 02:44:02.848563 pubmed_types-0.1.1/src/pubmed_types/models/pub_med_pub_date_pub_status.py
+-rw-r--r--   0        0        0      423 2023-06-03 02:44:02.640565 pubmed_types-0.1.1/src/pubmed_types/models/publication_type.py
+-rw-r--r--   0        0        0      400 2023-06-03 02:44:02.640565 pubmed_types-0.1.1/src/pubmed_types/models/publication_type_list.py
+-rw-r--r--   0        0        0     1192 2023-06-03 02:18:03.561932 pubmed_types-0.1.1/src/pubmed_types/models/publisher.py
+-rw-r--r--   0        0        0      606 2023-06-03 02:44:02.920561 pubmed_types-0.1.1/src/pubmed_types/models/publisher_1.py
+-rw-r--r--   0        0        0     1193 2023-06-03 02:44:02.920561 pubmed_types-0.1.1/src/pubmed_types/models/publisher_2.py
+-rw-r--r--   0        0        0     1013 2023-06-03 02:44:02.924561 pubmed_types-0.1.1/src/pubmed_types/models/publisher_name_1.py
+-rw-r--r--   0        0        0      600 2023-06-03 02:44:02.556566 pubmed_types-0.1.1/src/pubmed_types/models/pubmed_article.py
+-rw-r--r--   0        0        0      839 2023-06-03 02:44:02.552566 pubmed_types-0.1.1/src/pubmed_types/models/pubmed_article_set.py
+-rw-r--r--   0        0        0      611 2023-06-03 02:44:02.556566 pubmed_types-0.1.1/src/pubmed_types/models/pubmed_book_article.py
+-rw-r--r--   0        0        0      384 2023-06-03 02:44:02.556566 pubmed_types-0.1.1/src/pubmed_types/models/pubmed_book_article_set.py
+-rw-r--r--   0        0        0      991 2023-06-03 02:44:02.572566 pubmed_types-0.1.1/src/pubmed_types/models/pubmed_book_data.py
+-rw-r--r--   0        0        0     1217 2023-06-03 02:44:02.572566 pubmed_types-0.1.1/src/pubmed_types/models/pubmed_data.py
+-rw-r--r--   0        0        0      724 2023-06-03 02:44:02.644565 pubmed_types-0.1.1/src/pubmed_types/models/qualifier_name.py
+-rw-r--r--   0        0        0       87 2023-06-03 02:44:02.840563 pubmed_types-0.1.1/src/pubmed_types/models/qualifier_name_major_topic_yn.py
+-rw-r--r--   0        0        0      268 2023-06-03 02:44:02.800563 pubmed_types-0.1.1/src/pubmed_types/models/question_question_response_type.py
+-rw-r--r--   0        0        0      695 2023-06-03 02:44:02.344569 pubmed_types-0.1.1/src/pubmed_types/models/ref_count.py
+-rw-r--r--   0        0        0      576 2023-06-03 02:44:02.644565 pubmed_types-0.1.1/src/pubmed_types/models/reference.py
+-rw-r--r--   0        0        0      678 2023-06-03 02:44:02.644565 pubmed_types-0.1.1/src/pubmed_types/models/reference_list.py
+-rw-r--r--   0        0        0      460 2023-06-03 02:18:03.773929 pubmed_types-0.1.1/src/pubmed_types/models/replaces.py
+-rw-r--r--   0        0        0      192 2023-06-03 02:18:04.045925 pubmed_types-0.1.1/src/pubmed_types/models/replaces_id_type.py
+-rw-r--r--   0        0        0     1440 2023-06-03 02:44:02.348569 pubmed_types-0.1.1/src/pubmed_types/models/resource_group.py
+-rw-r--r--   0        0        0     2014 2023-06-03 02:44:02.348569 pubmed_types-0.1.1/src/pubmed_types/models/resource_id.py
+-rw-r--r--   0        0        0     4999 2023-06-03 02:44:02.356569 pubmed_types-0.1.1/src/pubmed_types/models/resource_name.py
+-rw-r--r--   0        0        0     1009 2023-06-03 02:44:02.360569 pubmed_types-0.1.1/src/pubmed_types/models/resource_wrap.py
+-rw-r--r--   0        0        0     2223 2023-06-03 02:44:02.364569 pubmed_types-0.1.1/src/pubmed_types/models/response.py
+-rw-r--r--   0        0        0     3137 2023-06-03 02:44:02.368569 pubmed_types-0.1.1/src/pubmed_types/models/restricted_by.py
+-rw-r--r--   0        0        0       79 2023-06-03 02:44:02.772564 pubmed_types-0.1.1/src/pubmed_types/models/roman_toggle.py
+-rw-r--r--   0        0        0      728 2023-06-03 02:44:02.368569 pubmed_types-0.1.1/src/pubmed_types/models/rp.py
+-rw-r--r--   0        0        0     1346 2023-06-03 02:44:02.372569 pubmed_types-0.1.1/src/pubmed_types/models/rt.py
+-rw-r--r--   0        0        0       83 2023-06-03 02:44:02.772564 pubmed_types-0.1.1/src/pubmed_types/models/sans_serif_toggle.py
+-rw-r--r--   0        0        0       76 2023-06-03 02:44:02.776564 pubmed_types-0.1.1/src/pubmed_types/models/sc_toggle.py
+-rw-r--r--   0        0        0     1337 2023-06-03 02:44:02.376569 pubmed_types-0.1.1/src/pubmed_types/models/season.py
+-rw-r--r--   0        0        0      765 2023-06-03 02:44:02.648565 pubmed_types-0.1.1/src/pubmed_types/models/section.py
+-rw-r--r--   0        0        0     1341 2023-06-03 02:44:02.648565 pubmed_types-0.1.1/src/pubmed_types/models/section_title.py
+-rw-r--r--   0        0        0      347 2023-06-03 02:44:02.648565 pubmed_types-0.1.1/src/pubmed_types/models/sections.py
+-rw-r--r--   0        0        0     9015 2023-06-03 02:44:02.388569 pubmed_types-0.1.1/src/pubmed_types/models/self_uri.py
+-rw-r--r--   0        0        0     7416 2023-06-03 02:44:02.400569 pubmed_types-0.1.1/src/pubmed_types/models/series_text.py
+-rw-r--r--   0        0        0     7394 2023-06-03 02:44:02.412568 pubmed_types-0.1.1/src/pubmed_types/models/series_title.py
+-rw-r--r--   0        0        0     7912 2023-06-03 02:44:02.424568 pubmed_types-0.1.1/src/pubmed_types/models/sig.py
+-rw-r--r--   0        0        0     8403 2023-06-03 02:44:02.440568 pubmed_types-0.1.1/src/pubmed_types/models/sig_block.py
+-rw-r--r--   0        0        0     1361 2023-06-03 02:44:02.444568 pubmed_types-0.1.1/src/pubmed_types/models/state.py
+-rw-r--r--   0        0        0       80 2023-06-03 02:44:02.776564 pubmed_types-0.1.1/src/pubmed_types/models/strike_toggle.py
+-rw-r--r--   0        0        0     8497 2023-06-03 02:44:02.460568 pubmed_types-0.1.1/src/pubmed_types/models/string_conf.py
+-rw-r--r--   0        0        0      159 2023-06-03 02:44:02.784563 pubmed_types-0.1.1/src/pubmed_types/models/string_name_name_style.py
+-rw-r--r--   0        0        0       87 2023-06-03 02:44:02.780563 pubmed_types-0.1.1/src/pubmed_types/models/styled_content_toggle.py
+-rw-r--r--   0        0        0      993 2023-06-03 02:44:02.924561 pubmed_types-0.1.1/src/pubmed_types/models/sub_1.py
+-rw-r--r--   0        0        0       92 2023-06-03 02:44:02.780563 pubmed_types-0.1.1/src/pubmed_types/models/sub_arrange.py
+-rw-r--r--   0        0        0     2576 2023-06-03 02:44:02.468568 pubmed_types-0.1.1/src/pubmed_types/models/sub_article.py
+-rw-r--r--   0        0        0      999 2023-06-03 02:44:02.924561 pubmed_types-0.1.1/src/pubmed_types/models/suffix_1.py
+-rw-r--r--   0        0        0      993 2023-06-03 02:44:02.928561 pubmed_types-0.1.1/src/pubmed_types/models/sup_1.py
+-rw-r--r--   0        0        0       92 2023-06-03 02:44:02.780563 pubmed_types-0.1.1/src/pubmed_types/models/sup_arrange.py
+-rw-r--r--   0        0        0      386 2023-06-03 02:44:02.648565 pubmed_types-0.1.1/src/pubmed_types/models/suppl_mesh_list.py
+-rw-r--r--   0        0        0      668 2023-06-03 02:44:02.652565 pubmed_types-0.1.1/src/pubmed_types/models/suppl_mesh_name.py
+-rw-r--r--   0        0        0      185 2023-06-03 02:44:02.836563 pubmed_types-0.1.1/src/pubmed_types/models/suppl_mesh_name_type.py
+-rw-r--r--   0        0        0      124 2023-06-03 02:44:02.800563 pubmed_types-0.1.1/src/pubmed_types/models/supplementary_material_orientation.py
+-rw-r--r--   0        0        0      161 2023-06-03 02:44:02.800563 pubmed_types-0.1.1/src/pubmed_types/models/supplementary_material_position.py
+-rw-r--r--   0        0        0     1316 2023-06-03 02:44:02.472568 pubmed_types-0.1.1/src/pubmed_types/models/support_description.py
+-rw-r--r--   0        0        0     1500 2023-06-03 02:44:02.476568 pubmed_types-0.1.1/src/pubmed_types/models/support_group.py
+-rw-r--r--   0        0        0     9397 2023-06-03 02:44:02.500567 pubmed_types-0.1.1/src/pubmed_types/models/support_source.py
+-rw-r--r--   0        0        0      695 2023-06-03 02:44:02.500567 pubmed_types-0.1.1/src/pubmed_types/models/table_count.py
+-rw-r--r--   0        0        0      220 2023-06-03 02:44:02.804563 pubmed_types-0.1.1/src/pubmed_types/models/table_frame.py
+-rw-r--r--   0        0        0      140 2023-06-03 02:44:02.804563 pubmed_types-0.1.1/src/pubmed_types/models/table_rules.py
+-rw-r--r--   0        0        0      117 2023-06-03 02:44:02.820563 pubmed_types-0.1.1/src/pubmed_types/models/table_wrap_group_orientation.py
+-rw-r--r--   0        0        0      154 2023-06-03 02:44:02.820563 pubmed_types-0.1.1/src/pubmed_types/models/table_wrap_group_position.py
+-rw-r--r--   0        0        0      112 2023-06-03 02:44:02.800563 pubmed_types-0.1.1/src/pubmed_types/models/table_wrap_orientation.py
+-rw-r--r--   0        0        0      149 2023-06-03 02:44:02.800563 pubmed_types-0.1.1/src/pubmed_types/models/table_wrap_position.py
+-rw-r--r--   0        0        0      150 2023-06-03 02:44:02.816563 pubmed_types-0.1.1/src/pubmed_types/models/tbody_align.py
+-rw-r--r--   0        0        0      135 2023-06-03 02:44:02.820563 pubmed_types-0.1.1/src/pubmed_types/models/tbody_valign.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.812563 pubmed_types-0.1.1/src/pubmed_types/models/td_align.py
+-rw-r--r--   0        0        0      129 2023-06-03 02:44:02.812563 pubmed_types-0.1.1/src/pubmed_types/models/td_scope.py
+-rw-r--r--   0        0        0      132 2023-06-03 02:44:02.816563 pubmed_types-0.1.1/src/pubmed_types/models/td_valign.py
+-rw-r--r--   0        0        0     1386 2023-06-03 02:44:02.504567 pubmed_types-0.1.1/src/pubmed_types/models/tex_math.py
+-rw-r--r--   0        0        0      128 2023-06-03 02:44:02.780563 pubmed_types-0.1.1/src/pubmed_types/models/tex_math_notation.py
+-rw-r--r--   0        0        0      150 2023-06-03 02:44:02.816563 pubmed_types-0.1.1/src/pubmed_types/models/tfoot_align.py
+-rw-r--r--   0        0        0      135 2023-06-03 02:44:02.816563 pubmed_types-0.1.1/src/pubmed_types/models/tfoot_valign.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.812563 pubmed_types-0.1.1/src/pubmed_types/models/th_align.py
+-rw-r--r--   0        0        0      129 2023-06-03 02:44:02.812563 pubmed_types-0.1.1/src/pubmed_types/models/th_scope.py
+-rw-r--r--   0        0        0      132 2023-06-03 02:44:02.812563 pubmed_types-0.1.1/src/pubmed_types/models/th_valign.py
+-rw-r--r--   0        0        0      150 2023-06-03 02:44:02.808563 pubmed_types-0.1.1/src/pubmed_types/models/thead_align.py
+-rw-r--r--   0        0        0      135 2023-06-03 02:44:02.808563 pubmed_types-0.1.1/src/pubmed_types/models/thead_valign.py
+-rw-r--r--   0        0        0     1542 2023-06-03 02:44:02.508567 pubmed_types-0.1.1/src/pubmed_types/models/title_group.py
+-rw-r--r--   0        0        0      147 2023-06-03 02:44:02.808563 pubmed_types-0.1.1/src/pubmed_types/models/tr_align.py
+-rw-r--r--   0        0        0      132 2023-06-03 02:44:02.808563 pubmed_types-0.1.1/src/pubmed_types/models/tr_valign.py
+-rw-r--r--   0        0        0     8912 2023-06-03 02:44:02.520567 pubmed_types-0.1.1/src/pubmed_types/models/trans_abstract.py
+-rw-r--r--   0        0        0     7376 2023-06-03 02:44:02.532567 pubmed_types-0.1.1/src/pubmed_types/models/trans_subtitle.py
+-rw-r--r--   0        0        0     1641 2023-06-03 02:44:02.536567 pubmed_types-0.1.1/src/pubmed_types/models/trans_title_group.py
+-rw-r--r--   0        0        0     2610 2023-06-03 02:44:02.584566 pubmed_types-0.1.1/src/pubmed_types/models/u.py
+-rw-r--r--   0        0        0      866 2023-06-03 02:44:02.536567 pubmed_types-0.1.1/src/pubmed_types/models/underline_end.py
+-rw-r--r--   0        0        0      750 2023-06-03 02:44:02.540567 pubmed_types-0.1.1/src/pubmed_types/models/underline_start.py
+-rw-r--r--   0        0        0       83 2023-06-03 02:44:02.776564 pubmed_types-0.1.1/src/pubmed_types/models/underline_toggle.py
+-rw-r--r--   0        0        0      614 2023-06-03 02:44:02.652565 pubmed_types-0.1.1/src/pubmed_types/models/url.py
+-rw-r--r--   0        0        0      661 2023-06-03 02:44:02.856562 pubmed_types-0.1.1/src/pubmed_types/models/url_lang.py
+-rw-r--r--   0        0        0      150 2023-06-03 02:44:02.856562 pubmed_types-0.1.1/src/pubmed_types/models/url_type.py
+-rw-r--r--   0        0        0     1072 2023-06-03 02:44:02.656565 pubmed_types-0.1.1/src/pubmed_types/models/vernacular_title.py
+-rw-r--r--   0        0        0     2893 2023-06-03 02:44:02.544567 pubmed_types-0.1.1/src/pubmed_types/models/volume_issue_group.py
+-rw-r--r--   0        0        0      962 2023-06-03 02:44:02.656565 pubmed_types-0.1.1/src/pubmed_types/models/volume_title.py
+-rw-r--r--   0        0        0      692 2023-06-03 02:44:02.548566 pubmed_types-0.1.1/src/pubmed_types/models/word_count.py
+-rw-r--r--   0        0        0      330 2023-06-03 02:44:02.656565 pubmed_types-0.1.1/src/pubmed_types/models/xs_pattern.py
+-rw-r--r--   0        0        0     1627 2023-06-03 02:44:02.552566 pubmed_types-0.1.1/src/pubmed_types/models/year.py
+-rw-r--r--   0        0        0     5086 1970-01-01 00:00:00.000000 pubmed_types-0.1.1/PKG-INFO
```

### Comparing `pubmed_types-0.1.0/LICENSE` & `pubmed_types-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/__init__.py` & `pubmed_types-0.1.1/src/pubmed_types/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/abbrev_journal_title.py` & `pubmed_types-0.1.1/src/pubmed_types/models/abbrev_journal_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/abstract_1.py` & `pubmed_types-0.1.1/src/pubmed_types/models/abstract_1.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/abstract_text.py` & `pubmed_types-0.1.1/src/pubmed_types/models/abstract_text.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/access_date.py` & `pubmed_types-0.1.1/src/pubmed_types/models/access_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/affiliation.py` & `pubmed_types-0.1.1/src/pubmed_types/models/affiliation.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/affiliation_info.py` & `pubmed_types-0.1.1/src/pubmed_types/models/affiliation_info.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/alt_text.py` & `pubmed_types-0.1.1/src/pubmed_types/models/alt_text.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/app.py` & `pubmed_types-0.1.1/src/pubmed_types/models/app.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/app_group.py` & `pubmed_types-0.1.1/src/pubmed_types/models/app_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/article_1.py` & `pubmed_types-0.1.1/src/pubmed_types/models/article_1.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/article_2.py` & `pubmed_types-0.1.1/src/pubmed_types/models/article_2.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/article_categories.py` & `pubmed_types-0.1.1/src/pubmed_types/models/article_categories.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/article_date.py` & `pubmed_types-0.1.1/src/pubmed_types/models/article_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/article_id.py` & `pubmed_types-0.1.1/src/pubmed_types/models/article_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/article_meta.py` & `pubmed_types-0.1.1/src/pubmed_types/models/article_meta.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/article_title_1.py` & `pubmed_types-0.1.1/src/pubmed_types/models/article_title_1.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/article_version.py` & `pubmed_types-0.1.1/src/pubmed_types/models/article_version.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/article_version_alternatives.py` & `pubmed_types-0.1.1/src/pubmed_types/models/article_version_alternatives.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/author.py` & `pubmed_types-0.1.1/src/pubmed_types/models/author.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/author_list.py` & `pubmed_types-0.1.1/src/pubmed_types/models/author_list.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/author_notes.py` & `pubmed_types-0.1.1/src/pubmed_types/models/author_notes.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/award_desc.py` & `pubmed_types-0.1.1/src/pubmed_types/models/award_desc.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/award_group.py` & `pubmed_types-0.1.1/src/pubmed_types/models/award_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/award_name.py` & `pubmed_types-0.1.1/src/pubmed_types/models/award_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/back.py` & `pubmed_types-0.1.1/src/pubmed_types/models/back.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/beginning_date.py` & `pubmed_types-0.1.1/src/pubmed_types/models/beginning_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/body.py` & `pubmed_types-0.1.1/src/pubmed_types/models/body.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/book.py` & `pubmed_types-0.1.1/src/pubmed_types/models/book.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/book_document.py` & `pubmed_types-0.1.1/src/pubmed_types/models/book_document.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/book_document_set.py` & `pubmed_types-0.1.1/src/pubmed_types/models/book_document_set.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/book_title.py` & `pubmed_types-0.1.1/src/pubmed_types/models/book_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/break_mod.py` & `pubmed_types-0.1.1/src/pubmed_types/models/break_mod.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/chemical.py` & `pubmed_types-0.1.1/src/pubmed_types/models/chemical.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/citation.py` & `pubmed_types-0.1.1/src/pubmed_types/models/citation.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/city.py` & `pubmed_types-0.1.1/src/pubmed_types/models/city.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/coi_statement.py` & `pubmed_types-0.1.1/src/pubmed_types/models/coi_statement.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/col.py` & `pubmed_types-0.1.1/src/pubmed_types/models/col.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/colgroup.py` & `pubmed_types-0.1.1/src/pubmed_types/models/colgroup.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/collection_title.py` & `pubmed_types-0.1.1/src/pubmed_types/models/collection_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/collective_name.py` & `pubmed_types-0.1.1/src/pubmed_types/models/collective_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/comments_corrections.py` & `pubmed_types-0.1.1/src/pubmed_types/models/comments_corrections.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/comments_corrections_ref_type.py` & `pubmed_types-0.1.1/src/pubmed_types/models/comments_corrections_ref_type.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/conf_num.py` & `pubmed_types-0.1.1/src/pubmed_types/models/conf_num.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/conf_theme.py` & `pubmed_types-0.1.1/src/pubmed_types/models/conf_theme.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/conference.py` & `pubmed_types-0.1.1/src/pubmed_types/models/conference.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/contrib_id.py` & `pubmed_types-0.1.1/src/pubmed_types/models/contrib_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/contributed_resource_group.py` & `pubmed_types-0.1.1/src/pubmed_types/models/contributed_resource_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/contribution_date.py` & `pubmed_types-0.1.1/src/pubmed_types/models/contribution_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/copyright_year.py` & `pubmed_types-0.1.1/src/pubmed_types/models/copyright_year.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/corresp.py` & `pubmed_types-0.1.1/src/pubmed_types/models/corresp.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/count.py` & `pubmed_types-0.1.1/src/pubmed_types/models/count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/counts.py` & `pubmed_types-0.1.1/src/pubmed_types/models/counts.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/custom_meta.py` & `pubmed_types-0.1.1/src/pubmed_types/models/custom_meta.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/custom_meta_group.py` & `pubmed_types-0.1.1/src/pubmed_types/models/custom_meta_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/data_bank.py` & `pubmed_types-0.1.1/src/pubmed_types/models/data_bank.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/data_bank_list.py` & `pubmed_types-0.1.1/src/pubmed_types/models/data_bank_list.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/date_completed.py` & `pubmed_types-0.1.1/src/pubmed_types/models/date_completed.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/date_revised.py` & `pubmed_types-0.1.1/src/pubmed_types/models/date_revised.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/day.py` & `pubmed_types-0.1.1/src/pubmed_types/models/day.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/descriptor_name.py` & `pubmed_types-0.1.1/src/pubmed_types/models/descriptor_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/elocation_id.py` & `pubmed_types-0.1.1/src/pubmed_types/models/elocation_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/elocation_id_1.py` & `pubmed_types-0.1.1/src/pubmed_types/models/elocation_id_1.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/ending_date.py` & `pubmed_types-0.1.1/src/pubmed_types/models/ending_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/equation_count.py` & `pubmed_types-0.1.1/src/pubmed_types/models/equation_count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/era.py` & `pubmed_types-0.1.1/src/pubmed_types/models/era.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/event.py` & `pubmed_types-0.1.1/src/pubmed_types/models/event.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/event_desc.py` & `pubmed_types-0.1.1/src/pubmed_types/models/event_desc.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/extended_by.py` & `pubmed_types-0.1.1/src/pubmed_types/models/extended_by.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/fig_count.py` & `pubmed_types-0.1.1/src/pubmed_types/models/fig_count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/floats_group.py` & `pubmed_types-0.1.1/src/pubmed_types/models/floats_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/fpage.py` & `pubmed_types-0.1.1/src/pubmed_types/models/fpage.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/front.py` & `pubmed_types-0.1.1/src/pubmed_types/models/front.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/front_stub.py` & `pubmed_types-0.1.1/src/pubmed_types/models/front_stub.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/funding_group.py` & `pubmed_types-0.1.1/src/pubmed_types/models/funding_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/funding_statement.py` & `pubmed_types-0.1.1/src/pubmed_types/models/funding_statement.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/glyph_data.py` & `pubmed_types-0.1.1/src/pubmed_types/models/glyph_data.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/glyph_ref.py` & `pubmed_types-0.1.1/src/pubmed_types/models/glyph_ref.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/grant.py` & `pubmed_types-0.1.1/src/pubmed_types/models/grant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/grant_list.py` & `pubmed_types-0.1.1/src/pubmed_types/models/grant_list.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/group.py` & `pubmed_types-0.1.1/src/pubmed_types/models/group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/history_2.py` & `pubmed_types-0.1.1/src/pubmed_types/models/history_2.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/hr.py` & `pubmed_types-0.1.1/src/pubmed_types/models/hr.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/i.py` & `pubmed_types-0.1.1/src/pubmed_types/models/i.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/index_term_range_end.py` & `pubmed_types-0.1.1/src/pubmed_types/models/index_term_range_end.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/individual_name.py` & `pubmed_types-0.1.1/src/pubmed_types/models/individual_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/institution_id.py` & `pubmed_types-0.1.1/src/pubmed_types/models/institution_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/investigator.py` & `pubmed_types-0.1.1/src/pubmed_types/models/investigator.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/issn_1.py` & `pubmed_types-0.1.1/src/pubmed_types/models/issn_1.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/issue_id.py` & `pubmed_types-0.1.1/src/pubmed_types/models/issue_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/issue_sponsor.py` & `pubmed_types-0.1.1/src/pubmed_types/models/issue_sponsor.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/issue_subtitle.py` & `pubmed_types-0.1.1/src/pubmed_types/models/issue_subtitle.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/issue_title_group.py` & `pubmed_types-0.1.1/src/pubmed_types/models/issue_title_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/journal.py` & `pubmed_types-0.1.1/src/pubmed_types/models/journal.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/journal_id.py` & `pubmed_types-0.1.1/src/pubmed_types/models/journal_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/journal_issue.py` & `pubmed_types-0.1.1/src/pubmed_types/models/journal_issue.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/journal_meta.py` & `pubmed_types-0.1.1/src/pubmed_types/models/journal_meta.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/journal_subtitle.py` & `pubmed_types-0.1.1/src/pubmed_types/models/journal_subtitle.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/journal_title.py` & `pubmed_types-0.1.1/src/pubmed_types/models/journal_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/journal_title_group.py` & `pubmed_types-0.1.1/src/pubmed_types/models/journal_title_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/keyword.py` & `pubmed_types-0.1.1/src/pubmed_types/models/keyword.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/keyword_list.py` & `pubmed_types-0.1.1/src/pubmed_types/models/keyword_list.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/lpage.py` & `pubmed_types-0.1.1/src/pubmed_types/models/lpage.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/medline_citation.py` & `pubmed_types-0.1.1/src/pubmed_types/models/medline_citation.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/medline_journal_info.py` & `pubmed_types-0.1.1/src/pubmed_types/models/medline_journal_info.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/mesh_heading.py` & `pubmed_types-0.1.1/src/pubmed_types/models/mesh_heading.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/meta_name.py` & `pubmed_types-0.1.1/src/pubmed_types/models/meta_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/meta_value.py` & `pubmed_types-0.1.1/src/pubmed_types/models/meta_value.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/milestone_end.py` & `pubmed_types-0.1.1/src/pubmed_types/models/milestone_end.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/milestone_start.py` & `pubmed_types-0.1.1/src/pubmed_types/models/milestone_start.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/month.py` & `pubmed_types-0.1.1/src/pubmed_types/models/month.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/object_id.py` & `pubmed_types-0.1.1/src/pubmed_types/models/object_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/free_to_read.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/free_to_read.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/license_ref.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/license_ref.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/__init__.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/__init__.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/abs.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/abs.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/annotation.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/annotation.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/approx.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/approx.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arg.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arg.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cbytes.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cbytes.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ceiling.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ceiling.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/condition.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/condition.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/conjugate.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/conjugate.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cs.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cs.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/divide.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/divide.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/exp.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/exp.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/factorial.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/factorial.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/factorof.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/factorof.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/floor.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/floor.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/imaginary.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/imaginary.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maligngroup.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maligngroup.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/malignmark.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/malignmark.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_mathvariant.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_mathvariant.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_mathvariant.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/minus.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/minus.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlabeledtr.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlabeledtr.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_mathvariant.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_mathvariant.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mprescripts.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mprescripts.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_mathvariant.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msline.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msline.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_mathvariant.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_mathvariant.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_mathvariant.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtr.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtr.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/neq.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/neq.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/none.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/none.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/power.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/power.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/quotient.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/quotient.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/real.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/real.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/rem.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/rem.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/root.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/root.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/share.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/share.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/tendsto.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/tendsto.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1999/xlink/arc_type.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/arc_type.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1999/xlink/extended.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/extended.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1999/xlink/locator_type.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/locator_type.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1999/xlink/resource_type.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/resource_type.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1999/xlink/simple.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/simple.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/org/w3/pkg_1999/xlink/title_elt_type.py` & `pubmed_types-0.1.1/src/pubmed_types/models/org/w3/pkg_1999/xlink/title_elt_type.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/other_abstract.py` & `pubmed_types-0.1.1/src/pubmed_types/models/other_abstract.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/other_id.py` & `pubmed_types-0.1.1/src/pubmed_types/models/other_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/overline_end.py` & `pubmed_types-0.1.1/src/pubmed_types/models/overline_end.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/overline_start.py` & `pubmed_types-0.1.1/src/pubmed_types/models/overline_start.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/page_count.py` & `pubmed_types-0.1.1/src/pubmed_types/models/page_count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/page_range.py` & `pubmed_types-0.1.1/src/pubmed_types/models/page_range.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/pagination.py` & `pubmed_types-0.1.1/src/pubmed_types/models/pagination.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/param.py` & `pubmed_types-0.1.1/src/pubmed_types/models/param.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/personal_name_subject.py` & `pubmed_types-0.1.1/src/pubmed_types/models/personal_name_subject.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/postal_code.py` & `pubmed_types-0.1.1/src/pubmed_types/models/postal_code.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/principal_award_recipient.py` & `pubmed_types-0.1.1/src/pubmed_types/models/principal_award_recipient.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/principal_investigator.py` & `pubmed_types-0.1.1/src/pubmed_types/models/principal_investigator.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/processing_meta.py` & `pubmed_types-0.1.1/src/pubmed_types/models/processing_meta.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/pub_date_1.py` & `pubmed_types-0.1.1/src/pubmed_types/models/pub_date_1.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/pub_date_2.py` & `pubmed_types-0.1.1/src/pubmed_types/models/pub_date_2.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/pub_date_not_available.py` & `pubmed_types-0.1.1/src/pubmed_types/models/pub_date_not_available.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/pub_history.py` & `pubmed_types-0.1.1/src/pubmed_types/models/pub_history.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/pub_id.py` & `pubmed_types-0.1.1/src/pubmed_types/models/pub_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/pub_med_pub_date.py` & `pubmed_types-0.1.1/src/pubmed_types/models/pub_med_pub_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/publisher.py` & `pubmed_types-0.1.1/src/pubmed_types/models/publisher.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/publisher_1.py` & `pubmed_types-0.1.1/src/pubmed_types/models/publisher_1.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/publisher_2.py` & `pubmed_types-0.1.1/src/pubmed_types/models/publisher_2.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/publisher_name_1.py` & `pubmed_types-0.1.1/src/pubmed_types/models/publisher_name_1.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/pubmed_article.py` & `pubmed_types-0.1.1/src/pubmed_types/models/pubmed_article.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/pubmed_article_set.py` & `pubmed_types-0.1.1/src/pubmed_types/models/pubmed_article_set.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/pubmed_book_article.py` & `pubmed_types-0.1.1/src/pubmed_types/models/pubmed_book_article.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/pubmed_book_data.py` & `pubmed_types-0.1.1/src/pubmed_types/models/pubmed_book_data.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/pubmed_data.py` & `pubmed_types-0.1.1/src/pubmed_types/models/pubmed_data.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/qualifier_name.py` & `pubmed_types-0.1.1/src/pubmed_types/models/qualifier_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/ref_count.py` & `pubmed_types-0.1.1/src/pubmed_types/models/ref_count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/reference.py` & `pubmed_types-0.1.1/src/pubmed_types/models/reference.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/reference_list.py` & `pubmed_types-0.1.1/src/pubmed_types/models/reference_list.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/resource_group.py` & `pubmed_types-0.1.1/src/pubmed_types/models/resource_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/resource_id.py` & `pubmed_types-0.1.1/src/pubmed_types/models/resource_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/resource_name.py` & `pubmed_types-0.1.1/src/pubmed_types/models/resource_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/resource_wrap.py` & `pubmed_types-0.1.1/src/pubmed_types/models/resource_wrap.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/response.py` & `pubmed_types-0.1.1/src/pubmed_types/models/response.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/restricted_by.py` & `pubmed_types-0.1.1/src/pubmed_types/models/restricted_by.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/rp.py` & `pubmed_types-0.1.1/src/pubmed_types/models/rp.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/rt.py` & `pubmed_types-0.1.1/src/pubmed_types/models/rt.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/season.py` & `pubmed_types-0.1.1/src/pubmed_types/models/season.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/section.py` & `pubmed_types-0.1.1/src/pubmed_types/models/section.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/section_title.py` & `pubmed_types-0.1.1/src/pubmed_types/models/section_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/self_uri.py` & `pubmed_types-0.1.1/src/pubmed_types/models/self_uri.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/series_text.py` & `pubmed_types-0.1.1/src/pubmed_types/models/series_text.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/series_title.py` & `pubmed_types-0.1.1/src/pubmed_types/models/series_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/sig.py` & `pubmed_types-0.1.1/src/pubmed_types/models/sig.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/sig_block.py` & `pubmed_types-0.1.1/src/pubmed_types/models/sig_block.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/state.py` & `pubmed_types-0.1.1/src/pubmed_types/models/state.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/string_conf.py` & `pubmed_types-0.1.1/src/pubmed_types/models/string_conf.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/sub_1.py` & `pubmed_types-0.1.1/src/pubmed_types/models/sub_1.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/sub_article.py` & `pubmed_types-0.1.1/src/pubmed_types/models/sub_article.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/suffix_1.py` & `pubmed_types-0.1.1/src/pubmed_types/models/suffix_1.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/sup_1.py` & `pubmed_types-0.1.1/src/pubmed_types/models/sup_1.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/suppl_mesh_name.py` & `pubmed_types-0.1.1/src/pubmed_types/models/suppl_mesh_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/support_description.py` & `pubmed_types-0.1.1/src/pubmed_types/models/support_description.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/support_group.py` & `pubmed_types-0.1.1/src/pubmed_types/models/support_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/support_source.py` & `pubmed_types-0.1.1/src/pubmed_types/models/support_source.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/table_count.py` & `pubmed_types-0.1.1/src/pubmed_types/models/table_count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/tex_math.py` & `pubmed_types-0.1.1/src/pubmed_types/models/tex_math.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/title_group.py` & `pubmed_types-0.1.1/src/pubmed_types/models/title_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/trans_abstract.py` & `pubmed_types-0.1.1/src/pubmed_types/models/trans_abstract.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/trans_subtitle.py` & `pubmed_types-0.1.1/src/pubmed_types/models/trans_subtitle.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/trans_title_group.py` & `pubmed_types-0.1.1/src/pubmed_types/models/trans_title_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/u.py` & `pubmed_types-0.1.1/src/pubmed_types/models/u.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/underline_end.py` & `pubmed_types-0.1.1/src/pubmed_types/models/underline_end.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/underline_start.py` & `pubmed_types-0.1.1/src/pubmed_types/models/underline_start.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/url.py` & `pubmed_types-0.1.1/src/pubmed_types/models/url.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/url_lang.py` & `pubmed_types-0.1.1/src/pubmed_types/models/url_lang.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/vernacular_title.py` & `pubmed_types-0.1.1/src/pubmed_types/models/vernacular_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/volume_issue_group.py` & `pubmed_types-0.1.1/src/pubmed_types/models/volume_issue_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/volume_title.py` & `pubmed_types-0.1.1/src/pubmed_types/models/volume_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/word_count.py` & `pubmed_types-0.1.1/src/pubmed_types/models/word_count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.0/src/pubmed_types/models/year.py` & `pubmed_types-0.1.1/src/pubmed_types/models/year.py`

 * *Files identical despite different names*

