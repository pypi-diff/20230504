# Comparing `tmp/feffery_antd_components-0.2.5.tar.gz` & `tmp/feffery_antd_components-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feffery_antd_components-0.2.5.tar", last modified: Tue Apr 25 08:45:38 2023, max compression
+gzip compressed data, was "feffery_antd_components-0.2.6.tar", last modified: Thu May  4 07:04:52 2023, max compression
```

## Comparing `feffery_antd_components-0.2.5.tar` & `feffery_antd_components-0.2.6.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 08:45:38.104397 feffery_antd_components-0.2.5/
--rw-rw-rw-   0        0        0     1087 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.5/LICENSE
--rw-rw-rw-   0        0        0      288 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0      346 2023-04-25 08:45:38.104397 feffery_antd_components-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     2301 2023-04-25 07:15:50.000000 feffery_antd_components-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 08:45:38.097055 feffery_antd_components-0.2.5/feffery_antd_components/
--rw-rw-rw-   0        0        0     3328 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdAccordion.py
--rw-rw-rw-   0        0        0     2539 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdAccordionItem.py
--rw-rw-rw-   0        0        0     2006 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdAffix.py
--rw-rw-rw-   0        0        0     2627 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdAlert.py
--rw-rw-rw-   0        0        0     2314 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdAnchor.py
--rw-rw-rw-   0        0        0     2586 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdAvatar.py
--rw-rw-rw-   0        0        0     2611 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdAvatarGroup.py
--rw-rw-rw-   0        0        0     1892 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdBackTop.py
--rw-rw-rw-   0        0        0     2730 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdBadge.py
--rw-rw-rw-   0        0        0     2313 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdBreadcrumb.py
--rw-rw-rw-   0        0        0     3218 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdButton.py
--rw-rw-rw-   0        0        0     3356 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCalendar.py
--rw-rw-rw-   0        0        0     2991 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCard.py
--rw-rw-rw-   0        0        0     1924 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCardGrid.py
--rw-rw-rw-   0        0        0     2490 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCarousel.py
--rw-rw-rw-   0        0        0     5312 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCascader.py
--rw-rw-rw-   0        0        0     3615 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCheckCard.py
--rw-rw-rw-   0        0        0     3694 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCheckCardGroup.py
--rw-rw-rw-   0        0        0     3303 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCheckbox.py
--rw-rw-rw-   0        0        0     3388 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCheckboxGroup.py
--rw-rw-rw-   0        0        0     3890 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCol.py
--rw-rw-rw-   0        0        0     3763 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCollapse.py
--rw-rw-rw-   0        0        0     3987 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdComment.py
--rw-rw-rw-   0        0        0     2076 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdConfigProvider.py
--rw-rw-rw-   0        0        0     1824 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdContent.py
--rw-rw-rw-   0        0        0     2109 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCopyText.py
--rw-rw-rw-   0        0        0     2497 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCountdown.py
--rw-rw-rw-   0        0        0     2530 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdCustomSkeleton.py
--rw-rw-rw-   0        0        0     5353 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdDatePicker.py
--rw-rw-rw-   0        0        0     5418 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdDateRangePicker.py
--rw-rw-rw-   0        0        0     2263 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdDescriptionItem.py
--rw-rw-rw-   0        0        0     2745 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdDescriptions.py
--rw-rw-rw-   0        0        0     2676 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdDivider.py
--rw-rw-rw-   0        0        0     6274 2023-04-25 08:45:37.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdDraggerUpload.py
--rw-rw-rw-   0        0        0     3109 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdDrawer.py
--rw-rw-rw-   0        0        0     3744 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdDropdown.py
--rw-rw-rw-   0        0        0     2250 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdEmpty.py
--rw-rw-rw-   0        0        0     1820 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdFooter.py
--rw-rw-rw-   0        0        0     2552 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdForm.py
--rw-rw-rw-   0        0        0     3351 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdFormItem.py
--rw-rw-rw-   0        0        0     1820 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdHeader.py
--rw-rw-rw-   0        0        0     1829 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdIcon.py
--rw-rw-rw-   0        0        0     5562 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdImage.py
--rw-rw-rw-   0        0        0     5674 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdInput.py
--rw-rw-rw-   0        0        0     5082 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdInputNumber.py
--rw-rw-rw-   0        0        0     1820 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdLayout.py
--rw-rw-rw-   0        0        0     3094 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdMentions.py
--rw-rw-rw-   0        0        0     4059 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdMenu.py
--rw-rw-rw-   0        0        0     2110 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdMessage.py
--rw-rw-rw-   0        0        0     5365 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdModal.py
--rw-rw-rw-   0        0        0     2417 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdNotification.py
--rw-rw-rw-   0        0        0     2555 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdPageHeader.py
--rw-rw-rw-   0        0        0     4592 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdPagination.py
--rw-rw-rw-   0        0        0     2752 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdParagraph.py
--rw-rw-rw-   0        0        0     2002 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdPasteImage.py
--rw-rw-rw-   0        0        0     6381 2023-04-25 08:45:37.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdPictureUpload.py
--rw-rw-rw-   0        0        0     4807 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdPopconfirm.py
--rw-rw-rw-   0        0        0     3562 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdPopover.py
--rw-rw-rw-   0        0        0     2869 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdPopupCard.py
--rw-rw-rw-   0        0        0     3352 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdProgress.py
--rw-rw-rw-   0        0        0     4008 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdRadioGroup.py
--rw-rw-rw-   0        0        0     3488 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdRate.py
--rw-rw-rw-   0        0        0     2181 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdResult.py
--rw-rw-rw-   0        0        0     2068 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdRibbon.py
--rw-rw-rw-   0        0        0     2489 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdRow.py
--rw-rw-rw-   0        0        0     3715 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSegmented.py
--rw-rw-rw-   0        0        0     3598 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSegmentedColoring.py
--rw-rw-rw-   0        0        0     7197 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSelect.py
--rw-rw-rw-   0        0        0     2846 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSider.py
--rw-rw-rw-   0        0        0     3193 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSkeleton.py
--rw-rw-rw-   0        0        0     1934 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSkeletonAvatar.py
--rw-rw-rw-   0        0        0     2017 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSkeletonButton.py
--rw-rw-rw-   0        0        0     1604 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSkeletonImage.py
--rw-rw-rw-   0        0        0     1808 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSkeletonInput.py
--rw-rw-rw-   0        0        0     4230 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSlider.py
--rw-rw-rw-   0        0        0     2389 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSpace.py
--rw-rw-rw-   0        0        0     2931 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSpin.py
--rw-rw-rw-   0        0        0     2853 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSpoiler.py
--rw-rw-rw-   0        0        0     2607 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdStatistic.py
--rw-rw-rw-   0        0        0     3223 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSteps.py
--rw-rw-rw-   0        0        0     3651 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdSwitch.py
--rw-rw-rw-   0        0        0     2314 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTabPane.py
--rw-rw-rw-   0        0        0    19271 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTable.py
--rw-rw-rw-   0        0        0     5266 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTabs.py
--rw-rw-rw-   0        0        0     1950 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTag.py
--rw-rw-rw-   0        0        0     2820 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdText.py
--rw-rw-rw-   0        0        0     4722 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTimePicker.py
--rw-rw-rw-   0        0        0     4787 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTimeRangePicker.py
--rw-rw-rw-   0        0        0     2750 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTimeline.py
--rw-rw-rw-   0        0        0     2900 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTitle.py
--rw-rw-rw-   0        0        0     3445 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTooltip.py
--rw-rw-rw-   0        0        0     4586 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTransfer.py
--rw-rw-rw-   0        0        0     5301 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTree.py
--rw-rw-rw-   0        0        0     6685 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdTreeSelect.py
--rw-rw-rw-   0        0        0     5669 2023-04-25 08:45:37.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdUpload.py
--rw-rw-rw-   0        0        0     2397 2023-04-25 08:45:36.000000 feffery_antd_components-0.2.5/feffery_antd_components/AntdWatermark.py
--rw-rw-rw-   0        0        0     1571 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.5/feffery_antd_components/__init__.py
--rw-rw-rw-   0        0        0     5752 2023-04-25 08:45:37.000000 feffery_antd_components-0.2.5/feffery_antd_components/_imports_.py
--rw-rw-rw-   0        0        0  3771264 2023-04-25 08:45:31.000000 feffery_antd_components-0.2.5/feffery_antd_components/feffery_antd_components.min.js
--rw-rw-rw-   0        0        0   624550 2023-04-25 08:45:37.000000 feffery_antd_components-0.2.5/feffery_antd_components/metadata.json
--rw-rw-rw-   0        0        0     3031 2023-04-25 08:45:32.000000 feffery_antd_components-0.2.5/feffery_antd_components/package-info.json
-drwxrwxrwx   0        0        0        0 2023-04-25 08:45:38.102376 feffery_antd_components-0.2.5/feffery_antd_components.egg-info/
--rw-rw-rw-   0        0        0      346 2023-04-25 08:45:37.000000 feffery_antd_components-0.2.5/feffery_antd_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4341 2023-04-25 08:45:37.000000 feffery_antd_components-0.2.5/feffery_antd_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 08:45:37.000000 feffery_antd_components-0.2.5/feffery_antd_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-25 08:45:37.000000 feffery_antd_components-0.2.5/feffery_antd_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-25 08:45:37.000000 feffery_antd_components-0.2.5/feffery_antd_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3031 2023-04-25 08:45:01.000000 feffery_antd_components-0.2.5/package.json
--rw-rw-rw-   0        0        0       42 2023-04-25 08:45:38.105395 feffery_antd_components-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      715 2023-04-25 07:15:34.000000 feffery_antd_components-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:04:52.906213 feffery_antd_components-0.2.6/
+-rw-rw-rw-   0        0        0     1087 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0      288 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      346 2023-05-04 07:04:52.905214 feffery_antd_components-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2301 2023-05-04 07:03:17.000000 feffery_antd_components-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 07:04:52.898222 feffery_antd_components-0.2.6/feffery_antd_components/
+-rw-rw-rw-   0        0        0     3328 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdAccordion.py
+-rw-rw-rw-   0        0        0     2539 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdAccordionItem.py
+-rw-rw-rw-   0        0        0     2006 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdAffix.py
+-rw-rw-rw-   0        0        0     2627 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdAlert.py
+-rw-rw-rw-   0        0        0     2314 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdAnchor.py
+-rw-rw-rw-   0        0        0     2586 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdAvatar.py
+-rw-rw-rw-   0        0        0     2611 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdAvatarGroup.py
+-rw-rw-rw-   0        0        0     1892 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdBackTop.py
+-rw-rw-rw-   0        0        0     2730 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdBadge.py
+-rw-rw-rw-   0        0        0     2313 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdBreadcrumb.py
+-rw-rw-rw-   0        0        0     3218 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdButton.py
+-rw-rw-rw-   0        0        0     3356 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdCalendar.py
+-rw-rw-rw-   0        0        0     2991 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdCard.py
+-rw-rw-rw-   0        0        0     1924 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdCardGrid.py
+-rw-rw-rw-   0        0        0     2490 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdCarousel.py
+-rw-rw-rw-   0        0        0     5312 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdCascader.py
+-rw-rw-rw-   0        0        0     3615 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdCheckCard.py
+-rw-rw-rw-   0        0        0     3694 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdCheckCardGroup.py
+-rw-rw-rw-   0        0        0     3303 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdCheckbox.py
+-rw-rw-rw-   0        0        0     3388 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdCheckboxGroup.py
+-rw-rw-rw-   0        0        0     3890 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdCol.py
+-rw-rw-rw-   0        0        0     3763 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdCollapse.py
+-rw-rw-rw-   0        0        0     3987 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdComment.py
+-rw-rw-rw-   0        0        0     2076 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdConfigProvider.py
+-rw-rw-rw-   0        0        0     1824 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdContent.py
+-rw-rw-rw-   0        0        0     2109 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdCopyText.py
+-rw-rw-rw-   0        0        0     2497 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdCountdown.py
+-rw-rw-rw-   0        0        0     2530 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdCustomSkeleton.py
+-rw-rw-rw-   0        0        0     5353 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdDatePicker.py
+-rw-rw-rw-   0        0        0     5418 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdDateRangePicker.py
+-rw-rw-rw-   0        0        0     2263 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdDescriptionItem.py
+-rw-rw-rw-   0        0        0     2745 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdDescriptions.py
+-rw-rw-rw-   0        0        0     2676 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdDivider.py
+-rw-rw-rw-   0        0        0     6311 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdDraggerUpload.py
+-rw-rw-rw-   0        0        0     3109 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdDrawer.py
+-rw-rw-rw-   0        0        0     4113 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdDropdown.py
+-rw-rw-rw-   0        0        0     2250 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdEmpty.py
+-rw-rw-rw-   0        0        0     1820 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdFooter.py
+-rw-rw-rw-   0        0        0     2552 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdForm.py
+-rw-rw-rw-   0        0        0     3351 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdFormItem.py
+-rw-rw-rw-   0        0        0     1820 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdHeader.py
+-rw-rw-rw-   0        0        0     1829 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdIcon.py
+-rw-rw-rw-   0        0        0     5562 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdImage.py
+-rw-rw-rw-   0        0        0     5674 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdInput.py
+-rw-rw-rw-   0        0        0     5082 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdInputNumber.py
+-rw-rw-rw-   0        0        0     1820 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdLayout.py
+-rw-rw-rw-   0        0        0     3094 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdMentions.py
+-rw-rw-rw-   0        0        0     4059 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdMenu.py
+-rw-rw-rw-   0        0        0     2110 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdMessage.py
+-rw-rw-rw-   0        0        0     5365 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdModal.py
+-rw-rw-rw-   0        0        0     2417 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdNotification.py
+-rw-rw-rw-   0        0        0     2555 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdPageHeader.py
+-rw-rw-rw-   0        0        0     4592 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdPagination.py
+-rw-rw-rw-   0        0        0     2752 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdParagraph.py
+-rw-rw-rw-   0        0        0     2002 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdPasteImage.py
+-rw-rw-rw-   0        0        0     6418 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdPictureUpload.py
+-rw-rw-rw-   0        0        0     4807 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdPopconfirm.py
+-rw-rw-rw-   0        0        0     3562 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdPopover.py
+-rw-rw-rw-   0        0        0     2869 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdPopupCard.py
+-rw-rw-rw-   0        0        0     3352 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdProgress.py
+-rw-rw-rw-   0        0        0     4008 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdRadioGroup.py
+-rw-rw-rw-   0        0        0     3488 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdRate.py
+-rw-rw-rw-   0        0        0     2181 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdResult.py
+-rw-rw-rw-   0        0        0     2068 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdRibbon.py
+-rw-rw-rw-   0        0        0     2489 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdRow.py
+-rw-rw-rw-   0        0        0     3715 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdSegmented.py
+-rw-rw-rw-   0        0        0     3598 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdSegmentedColoring.py
+-rw-rw-rw-   0        0        0     7197 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdSelect.py
+-rw-rw-rw-   0        0        0     2846 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdSider.py
+-rw-rw-rw-   0        0        0     3193 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdSkeleton.py
+-rw-rw-rw-   0        0        0     1934 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdSkeletonAvatar.py
+-rw-rw-rw-   0        0        0     2017 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdSkeletonButton.py
+-rw-rw-rw-   0        0        0     1604 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdSkeletonImage.py
+-rw-rw-rw-   0        0        0     1808 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdSkeletonInput.py
+-rw-rw-rw-   0        0        0     4230 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdSlider.py
+-rw-rw-rw-   0        0        0     2389 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdSpace.py
+-rw-rw-rw-   0        0        0     2931 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdSpin.py
+-rw-rw-rw-   0        0        0     2853 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdSpoiler.py
+-rw-rw-rw-   0        0        0     2607 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdStatistic.py
+-rw-rw-rw-   0        0        0     3223 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdSteps.py
+-rw-rw-rw-   0        0        0     3651 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdSwitch.py
+-rw-rw-rw-   0        0        0     2314 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdTabPane.py
+-rw-rw-rw-   0        0        0    19336 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdTable.py
+-rw-rw-rw-   0        0        0     5266 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdTabs.py
+-rw-rw-rw-   0        0        0     1950 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdTag.py
+-rw-rw-rw-   0        0        0     2820 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdText.py
+-rw-rw-rw-   0        0        0     4722 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdTimePicker.py
+-rw-rw-rw-   0        0        0     4787 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdTimeRangePicker.py
+-rw-rw-rw-   0        0        0     2750 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdTimeline.py
+-rw-rw-rw-   0        0        0     2900 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdTitle.py
+-rw-rw-rw-   0        0        0     3445 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdTooltip.py
+-rw-rw-rw-   0        0        0     4586 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdTransfer.py
+-rw-rw-rw-   0        0        0     5547 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdTree.py
+-rw-rw-rw-   0        0        0     6685 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdTreeSelect.py
+-rw-rw-rw-   0        0        0     5706 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdUpload.py
+-rw-rw-rw-   0        0        0     2397 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/AntdWatermark.py
+-rw-rw-rw-   0        0        0     1571 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.6/feffery_antd_components/__init__.py
+-rw-rw-rw-   0        0        0     5752 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/_imports_.py
+-rw-rw-rw-   0        0        0  3775075 2023-05-04 07:04:45.000000 feffery_antd_components-0.2.6/feffery_antd_components/feffery_antd_components.min.js
+-rw-rw-rw-   0        0        0   626329 2023-05-04 07:04:51.000000 feffery_antd_components-0.2.6/feffery_antd_components/metadata.json
+-rw-rw-rw-   0        0        0     3031 2023-05-04 07:04:47.000000 feffery_antd_components-0.2.6/feffery_antd_components/package-info.json
+drwxrwxrwx   0        0        0        0 2023-05-04 07:04:52.904217 feffery_antd_components-0.2.6/feffery_antd_components.egg-info/
+-rw-rw-rw-   0        0        0      346 2023-05-04 07:04:52.000000 feffery_antd_components-0.2.6/feffery_antd_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4341 2023-05-04 07:04:52.000000 feffery_antd_components-0.2.6/feffery_antd_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 07:04:52.000000 feffery_antd_components-0.2.6/feffery_antd_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-04 07:04:52.000000 feffery_antd_components-0.2.6/feffery_antd_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-05-04 07:04:52.000000 feffery_antd_components-0.2.6/feffery_antd_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3031 2023-05-04 03:11:34.000000 feffery_antd_components-0.2.6/package.json
+-rw-rw-rw-   0        0        0       42 2023-05-04 07:04:52.906213 feffery_antd_components-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      715 2023-04-25 07:15:34.000000 feffery_antd_components-0.2.6/setup.py
```

### Comparing `feffery_antd_components-0.2.5/LICENSE` & `feffery_antd_components-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/README.md` & `feffery_antd_components-0.2.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/CNFeffery/feffery-antd-components.svg)](http://isitmaintained.com/project/CNFeffery/feffery-antd-components "Average time to resolve an issue")
 [![Percentage of issues still open](http://isitmaintained.com/badge/open/CNFeffery/feffery-antd-components.svg)](http://isitmaintained.com/project/CNFeffery/feffery-antd-components "Percentage of issues still open")
 
 </div>
 
 简体中文 | [English](./README-en_US.md)
 
-`feffery-components`计划子项目，`Plotly Dash`第三方组件库，基于`Antd`，将超多具有丰富功能的通用网页常用交互组件引入`Dash`的生态中 🥳，最新稳定版本：`0.2.3`
+`feffery-components`计划子项目，`Plotly Dash`第三方组件库，基于`Antd`，将超多具有丰富功能的通用网页常用交互组件引入`Dash`的生态中 🥳，最新稳定版本：`0.2.6`
 
 ## 1 最新版本安装方式
 
 ```bash
 pip install feffery-antd-components -U
 ```
```

#### html2text {}

```diff
@@ -12,15 +12,15 @@
  components "Average time to resolve an issue") [![Percentage of issues still
       open](http://isitmaintained.com/badge/open/CNFeffery/feffery-antd-
   components.svg)](http://isitmaintained.com/project/CNFeffery/feffery-antd-
                  components "Percentage of issues still open")
 ç®ä½ä¸­æ | [English](./README-en_US.md) `feffery-
 components`è®¡åå­é¡¹ç®ï¼`Plotly
 Dash`ç¬¬ä¸æ¹ç»ä»¶åºï¼åºäº`Antd`ï¼å°è¶å¤å·æä¸°å¯åè½çéç¨ç½é¡µå¸¸ç¨äº¤äºç»ä»¶å¼å¥`Dash`ççæä¸­
-ð¥³ï¼ææ°ç¨³å®çæ¬ï¼`0.2.3` ## 1 ææ°çæ¬å®è£æ¹å¼ ```bash pip
+ð¥³ï¼ææ°ç¨³å®çæ¬ï¼`0.2.6` ## 1 ææ°çæ¬å®è£æ¹å¼ ```bash pip
 install feffery-antd-components -U ``` ## 2 ææ°é¢åå¸çæ¬å®è£æ¹å¼
 ```bash pip install feffery-antd-components --pre -U ``` ## 3 éæèµæº CDN
 å éæ¹æ³ ```Python # édebugæ¨¡å¼ä¸å¯¹Dash
 ()ä¼ å¥åæ°serve_locally=Falseä¼å¼ºå¶æµè§å¨ç«¯ä»unpkg
 cdnå è½½åä¸ªä¾èµç #
 xxx.min.jsç­éæèµæºï¼ä»èé¿åå ç¨æå¡å¨å¸¦å®½ï¼éåä¸­å°åç«ç¹å éè®¿é®
 app = dash.Dash(serve_locally=False) ``` ## 4 å¨çº¿ææ¡£ ææ¡£å°å ## 5
```

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdAccordion.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdAccordion.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdAccordionItem.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdAccordionItem.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdAffix.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdAffix.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdAlert.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdAlert.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdAnchor.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdAnchor.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdAvatar.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdAvatar.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdAvatarGroup.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdAvatarGroup.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdBackTop.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdBackTop.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdBadge.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdBadge.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdBreadcrumb.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdBreadcrumb.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdButton.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdButton.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdCalendar.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdCalendar.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdCard.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdCard.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdCardGrid.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdCardGrid.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdCarousel.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdCarousel.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdCascader.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdCascader.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdCheckCard.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdCheckCard.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdCheckCardGroup.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdCheckCardGroup.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdCheckbox.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdCheckbox.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdCheckboxGroup.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdCheckboxGroup.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdCol.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdCol.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdCollapse.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdCollapse.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdComment.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdComment.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdConfigProvider.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdConfigProvider.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdContent.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdContent.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdCopyText.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdCopyText.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdCountdown.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdCountdown.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdCustomSkeleton.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdCustomSkeleton.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdDatePicker.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdDatePicker.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdDateRangePicker.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdDateRangePicker.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdDescriptionItem.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdDescriptionItem.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdDescriptions.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdDescriptions.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdDivider.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdDivider.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdDraggerUpload.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdDraggerUpload.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 - confirmBeforeDelete (boolean; default False)
 
 - defaultFileList (list of dicts; optional)
 
     `defaultFileList` is a list of dicts with keys:
 
+    - fileSize (number; optional)
+
     - name (string; optional)
 
     - status (a value equal to: 'done', 'error', 'removed'; optional)
 
     - taskId (string; optional)
 
     - uid (boolean | number | string | dict | list; optional)
```

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdDrawer.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdDrawer.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdDropdown.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdDropdown.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,14 +29,20 @@
 
 - className (string | dict; optional)
 
 - clickedKey (string; optional)
 
 - disabled (boolean; default False)
 
+- freePosition (boolean; default False)
+
+- freePositionClassName (string; optional)
+
+- freePositionStyle (dict; optional)
+
 - key (string; optional)
 
 - loading_state (dict; optional)
 
     `loading_state` is a dict with keys:
 
     - component_name (string; optional):
@@ -84,18 +90,18 @@
 
 - visible (boolean; default False)"""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'feffery_antd_components'
     _type = 'AntdDropdown'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, className=Component.UNDEFINED, style=Component.UNDEFINED, key=Component.UNDEFINED, title=Component.UNDEFINED, buttonMode=Component.UNDEFINED, buttonProps=Component.UNDEFINED, clickedKey=Component.UNDEFINED, nClicks=Component.UNDEFINED, menuItems=Component.UNDEFINED, arrow=Component.UNDEFINED, disabled=Component.UNDEFINED, overlayClassName=Component.UNDEFINED, overlayStyle=Component.UNDEFINED, placement=Component.UNDEFINED, trigger=Component.UNDEFINED, autoAdjustOverflow=Component.UNDEFINED, visible=Component.UNDEFINED, popupContainer=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'arrow', 'autoAdjustOverflow', 'buttonMode', 'buttonProps', 'className', 'clickedKey', 'disabled', 'key', 'loading_state', 'menuItems', 'nClicks', 'overlayClassName', 'overlayStyle', 'placement', 'popupContainer', 'style', 'title', 'trigger', 'visible']
+    def __init__(self, id=Component.UNDEFINED, className=Component.UNDEFINED, style=Component.UNDEFINED, key=Component.UNDEFINED, title=Component.UNDEFINED, buttonMode=Component.UNDEFINED, buttonProps=Component.UNDEFINED, freePosition=Component.UNDEFINED, freePositionStyle=Component.UNDEFINED, freePositionClassName=Component.UNDEFINED, clickedKey=Component.UNDEFINED, nClicks=Component.UNDEFINED, menuItems=Component.UNDEFINED, arrow=Component.UNDEFINED, disabled=Component.UNDEFINED, overlayClassName=Component.UNDEFINED, overlayStyle=Component.UNDEFINED, placement=Component.UNDEFINED, trigger=Component.UNDEFINED, autoAdjustOverflow=Component.UNDEFINED, visible=Component.UNDEFINED, popupContainer=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'arrow', 'autoAdjustOverflow', 'buttonMode', 'buttonProps', 'className', 'clickedKey', 'disabled', 'freePosition', 'freePositionClassName', 'freePositionStyle', 'key', 'loading_state', 'menuItems', 'nClicks', 'overlayClassName', 'overlayStyle', 'placement', 'popupContainer', 'style', 'title', 'trigger', 'visible']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'arrow', 'autoAdjustOverflow', 'buttonMode', 'buttonProps', 'className', 'clickedKey', 'disabled', 'key', 'loading_state', 'menuItems', 'nClicks', 'overlayClassName', 'overlayStyle', 'placement', 'popupContainer', 'style', 'title', 'trigger', 'visible']
+        self.available_properties = ['id', 'arrow', 'autoAdjustOverflow', 'buttonMode', 'buttonProps', 'className', 'clickedKey', 'disabled', 'freePosition', 'freePositionClassName', 'freePositionStyle', 'key', 'loading_state', 'menuItems', 'nClicks', 'overlayClassName', 'overlayStyle', 'placement', 'popupContainer', 'style', 'title', 'trigger', 'visible']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
         super(AntdDropdown, self).__init__(**args)
```

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdEmpty.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdEmpty.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdFooter.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdFooter.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdForm.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdForm.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdFormItem.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdFormItem.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdHeader.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdHeader.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdIcon.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdIcon.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdImage.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdImage.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdInput.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdInput.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdInputNumber.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdInputNumber.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdLayout.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdLayout.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdMentions.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdMentions.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdMenu.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdMenu.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdMessage.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdMessage.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdModal.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdModal.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdNotification.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdNotification.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdPageHeader.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdPageHeader.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdPagination.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdPagination.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdParagraph.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdParagraph.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdPasteImage.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdPasteImage.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdPictureUpload.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdPictureUpload.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 - confirmBeforeDelete (boolean; default False)
 
 - defaultFileList (list of dicts; optional)
 
     `defaultFileList` is a list of dicts with keys:
 
+    - fileSize (number; optional)
+
     - name (string; optional)
 
     - status (a value equal to: 'done', 'error', 'removed'; optional)
 
     - taskId (string; optional)
 
     - uid (boolean | number | string | dict | list; optional)
```

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdPopconfirm.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdPopconfirm.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdPopover.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdPopover.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdPopupCard.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdPopupCard.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdProgress.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdProgress.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdRadioGroup.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdRadioGroup.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdRate.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdRate.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdResult.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdResult.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdRibbon.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdRibbon.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdRow.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdRow.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdSegmented.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdSegmented.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdSegmentedColoring.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdSegmentedColoring.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdSelect.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdSelect.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdSider.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdSider.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdSkeleton.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdSkeleton.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdSkeletonAvatar.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdSkeletonAvatar.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdSkeletonButton.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdSkeletonButton.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdSkeletonImage.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdSkeletonImage.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdSkeletonInput.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdSkeletonInput.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdSlider.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdSlider.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdSpace.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdSpace.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdSpin.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdSpin.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdSpoiler.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdSpoiler.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdStatistic.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdStatistic.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdSteps.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdSteps.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdSwitch.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdSwitch.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdTabPane.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdTabPane.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdTable.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdTable.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,16 @@
 - currentData (list; optional)
 
 - customFormatFuncs (dict with strings as keys and values of type string; optional)
 
 - data (list of dicts; optional)
 
     `data` is a list of dicts with strings as keys and values of type
-    string | number | dict with keys:
+    list of boolean | number | string | dict | lists | string | number
+    | dict with keys:
 
     - content (string; optional)
 
     - disabled (boolean; optional)
 
     - href (string; optional)
 
@@ -268,15 +269,15 @@
 
     - options (list of dicts; optional)
 
         `options` is a list of dicts with keys:
 
         - label (string; optional)
 
-        - value (string; optional)
+        - value (string | number; optional)
 
     - placeholder (string; optional)
 
     - placement (a value equal to: 'bottomLeft', 'bottomRight', 'topLeft', 'topRight'; optional)
 
     - size (a value equal to: 'small', 'middle', 'large'; optional)
```

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdTabs.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdTabs.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdTag.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdTag.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdText.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdText.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdTimePicker.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdTimePicker.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdTimeRangePicker.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdTimeRangePicker.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdTimeline.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdTimeline.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdTitle.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdTitle.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdTooltip.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdTooltip.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdTransfer.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdTransfer.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdTree.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdTree.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,22 @@
 
 - checkable (boolean; default False)
 
 - checkedKeys (list of strings; optional)
 
 - className (string | number; optional)
 
+- clickedContextMenu (dict; optional)
+
+    `clickedContextMenu` is a dict with keys:
+
+    - menuKey (string; optional)
+
+    - nodeKey (string; optional)
+
 - defaultCheckedKeys (list of strings; optional)
 
 - defaultExpandAll (boolean; default False)
 
 - defaultExpandParent (boolean; default False)
 
 - defaultExpandedKeys (list of strings; optional)
@@ -93,18 +101,18 @@
 
 - treeDataMode (a value equal to: 'tree', 'flat'; default 'tree')"""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'feffery_antd_components'
     _type = 'AntdTree'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, className=Component.UNDEFINED, style=Component.UNDEFINED, key=Component.UNDEFINED, treeDataMode=Component.UNDEFINED, treeData=Component.UNDEFINED, showIcon=Component.UNDEFINED, selectable=Component.UNDEFINED, multiple=Component.UNDEFINED, checkable=Component.UNDEFINED, defaultExpandAll=Component.UNDEFINED, expandedKeys=Component.UNDEFINED, defaultExpandedKeys=Component.UNDEFINED, defaultExpandParent=Component.UNDEFINED, selectedKeys=Component.UNDEFINED, defaultSelectedKeys=Component.UNDEFINED, checkedKeys=Component.UNDEFINED, defaultCheckedKeys=Component.UNDEFINED, halfCheckedKeys=Component.UNDEFINED, checkStrictly=Component.UNDEFINED, showLine=Component.UNDEFINED, height=Component.UNDEFINED, draggable=Component.UNDEFINED, draggedNodeKey=Component.UNDEFINED, loading_state=Component.UNDEFINED, persistence=Component.UNDEFINED, persisted_props=Component.UNDEFINED, persistence_type=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'checkStrictly', 'checkable', 'checkedKeys', 'className', 'defaultCheckedKeys', 'defaultExpandAll', 'defaultExpandParent', 'defaultExpandedKeys', 'defaultSelectedKeys', 'draggable', 'draggedNodeKey', 'expandedKeys', 'halfCheckedKeys', 'height', 'key', 'loading_state', 'multiple', 'persisted_props', 'persistence', 'persistence_type', 'selectable', 'selectedKeys', 'showIcon', 'showLine', 'style', 'treeData', 'treeDataMode']
+    def __init__(self, id=Component.UNDEFINED, className=Component.UNDEFINED, style=Component.UNDEFINED, key=Component.UNDEFINED, treeDataMode=Component.UNDEFINED, treeData=Component.UNDEFINED, showIcon=Component.UNDEFINED, selectable=Component.UNDEFINED, multiple=Component.UNDEFINED, checkable=Component.UNDEFINED, defaultExpandAll=Component.UNDEFINED, expandedKeys=Component.UNDEFINED, defaultExpandedKeys=Component.UNDEFINED, defaultExpandParent=Component.UNDEFINED, selectedKeys=Component.UNDEFINED, defaultSelectedKeys=Component.UNDEFINED, checkedKeys=Component.UNDEFINED, defaultCheckedKeys=Component.UNDEFINED, halfCheckedKeys=Component.UNDEFINED, checkStrictly=Component.UNDEFINED, showLine=Component.UNDEFINED, height=Component.UNDEFINED, draggable=Component.UNDEFINED, draggedNodeKey=Component.UNDEFINED, clickedContextMenu=Component.UNDEFINED, loading_state=Component.UNDEFINED, persistence=Component.UNDEFINED, persisted_props=Component.UNDEFINED, persistence_type=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'checkStrictly', 'checkable', 'checkedKeys', 'className', 'clickedContextMenu', 'defaultCheckedKeys', 'defaultExpandAll', 'defaultExpandParent', 'defaultExpandedKeys', 'defaultSelectedKeys', 'draggable', 'draggedNodeKey', 'expandedKeys', 'halfCheckedKeys', 'height', 'key', 'loading_state', 'multiple', 'persisted_props', 'persistence', 'persistence_type', 'selectable', 'selectedKeys', 'showIcon', 'showLine', 'style', 'treeData', 'treeDataMode']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'checkStrictly', 'checkable', 'checkedKeys', 'className', 'defaultCheckedKeys', 'defaultExpandAll', 'defaultExpandParent', 'defaultExpandedKeys', 'defaultSelectedKeys', 'draggable', 'draggedNodeKey', 'expandedKeys', 'halfCheckedKeys', 'height', 'key', 'loading_state', 'multiple', 'persisted_props', 'persistence', 'persistence_type', 'selectable', 'selectedKeys', 'showIcon', 'showLine', 'style', 'treeData', 'treeDataMode']
+        self.available_properties = ['id', 'checkStrictly', 'checkable', 'checkedKeys', 'className', 'clickedContextMenu', 'defaultCheckedKeys', 'defaultExpandAll', 'defaultExpandParent', 'defaultExpandedKeys', 'defaultSelectedKeys', 'draggable', 'draggedNodeKey', 'expandedKeys', 'halfCheckedKeys', 'height', 'key', 'loading_state', 'multiple', 'persisted_props', 'persistence', 'persistence_type', 'selectable', 'selectedKeys', 'showIcon', 'showLine', 'style', 'treeData', 'treeDataMode']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
         super(AntdTree, self).__init__(**args)
```

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdTreeSelect.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdTreeSelect.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdUpload.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdUpload.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 - confirmBeforeDelete (boolean; default False)
 
 - defaultFileList (list of dicts; optional)
 
     `defaultFileList` is a list of dicts with keys:
 
+    - fileSize (number; optional)
+
     - name (string; optional)
 
     - status (a value equal to: 'done', 'error', 'removed'; optional)
 
     - taskId (string; optional)
 
     - uid (boolean | number | string | dict | list; optional)
```

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/AntdWatermark.py` & `feffery_antd_components-0.2.6/feffery_antd_components/AntdWatermark.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/__init__.py` & `feffery_antd_components-0.2.6/feffery_antd_components/__init__.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/_imports_.py` & `feffery_antd_components-0.2.6/feffery_antd_components/_imports_.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/feffery_antd_components.min.js` & `feffery_antd_components-0.2.6/feffery_antd_components/feffery_antd_components.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -57,15 +57,15 @@
     return Object.defineProperty(r, "p", {
         get: (t = o().src.split("/").slice(0, -1).join("/") + "/", function() {
             return t
         })
     }), "undefined" != typeof jsonpScriptSrc && (i = jsonpScriptSrc, jsonpScriptSrc = function(t) {
         var e, n = /\/_dash-component-suites\//.test(o().src),
             t = i(t);
-        return n ? ((e = (n = t.split("/")).slice(-1)[0].split(".")).splice(1, 0, "v0_2_5m1682412291"), n.splice(-1, 1, e.join(".")), n.join("/")) : t
+        return n ? ((e = (n = t.split("/")).slice(-1)[0].split(".")).splice(1, 0, "v0_2_6m1683183844"), n.splice(-1, 1, e.join(".")), n.join("/")) : t
     }), r(r.s = 688)
 }([function(t, e) {
     t.exports = window.React
 }, function(t, e) {
     t.exports = window.PropTypes
 }, function(R, t, e) {
     "use strict";
@@ -7085,15 +7085,15 @@
             return D
         }), e.d(n, "equals", function() {
             return T
         }), e.d(n, "mul", function() {
             return z
         }), e.d(n, "sub", function() {
             return A
-        }), e(56));
+        }), e(57));
 
     function a() {
         var t = new v.a(9);
         return v.a != Float32Array && (t[1] = 0, t[2] = 0, t[3] = 0, t[5] = 0, t[6] = 0, t[7] = 0), t[0] = 1, t[4] = 1, t[8] = 1, t
     }
 
     function r(t, e) {
@@ -8678,15 +8678,15 @@
             opacity: 1
         }
     }
 
     function o(t, e) {
         return !0 === (null == e ? void 0 : e.deadline) || "height" === e.propertyName
     }
-    var n = n(57),
+    var n = n(58),
         i = {
             motionName: "ant-motion-collapse",
             onAppearStart: a,
             onEnterStart: a,
             onAppearActive: r,
             onEnterActive: r,
             onLeaveStart: function(t) {
@@ -8807,15 +8807,15 @@
         return a
     }), n.d(e, "a", function() {
         return i
     });
     var r = n(5),
         e = n(7),
         o = n.n(e),
-        e = n(57);
+        e = n(58);
 
     function a(t, e, n) {
         var a;
         return o()((a = {}, Object(r.a)(a, "".concat(t, "-status-success"), "success" === e), Object(r.a)(a, "".concat(t, "-status-warning"), "warning" === e), Object(r.a)(a, "".concat(t, "-status-error"), "error" === e), Object(r.a)(a, "".concat(t, "-status-validating"), "validating" === e), Object(r.a)(a, "".concat(t, "-has-feedback"), n), a))
     }
     Object(e.a)("warning", "error", "");
     var i = function(t, e) {
@@ -9769,45 +9769,14 @@
     }), n.d(e, "c", function() {
         return p
     }), n.d(e, "d", function() {
         return P
     }), n.d(e, "f", function() {
         return a
     })
-}, function(t, e, n) {
-    "use strict";
-    n.d(e, "b", function() {
-        return a
-    }), n.d(e, "a", function() {
-        return r
-    }), n.d(e, "c", function() {
-        return o
-    });
-    var a = 1e-6,
-        r = "undefined" != typeof Float32Array ? Float32Array : Array,
-        o = Math.random;
-    Math.PI, Math.hypot || (Math.hypot = function() {
-        for (var t = 0, e = arguments.length; e--;) t += arguments[e] * arguments[e];
-        return Math.sqrt(t)
-    })
-}, function(t, e, n) {
-    "use strict";
-    n.d(e, "a", function() {
-        return a
-    }), n.d(e, "b", function() {
-        return r
-    });
-    var a = function() {
-            for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
-            return e
-        },
-        r = function() {
-            for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
-            return e
-        }
 }, function(R, I, t) {
     "use strict";
 
     function e(t, e) {
         return E.createElement(S.a, Object(M.a)(Object(M.a)({}, t), {}, {
             ref: e,
             icon: Rn
@@ -22837,14 +22806,45 @@
         setProps: L.a.func
     }, A.defaultProps = {
         nClicks: 0,
         debounceWait: 200
     }, I.a = A
 }, function(t, e, n) {
     "use strict";
+    n.d(e, "b", function() {
+        return a
+    }), n.d(e, "a", function() {
+        return r
+    }), n.d(e, "c", function() {
+        return o
+    });
+    var a = 1e-6,
+        r = "undefined" != typeof Float32Array ? Float32Array : Array,
+        o = Math.random;
+    Math.PI, Math.hypot || (Math.hypot = function() {
+        for (var t = 0, e = arguments.length; e--;) t += arguments[e] * arguments[e];
+        return Math.sqrt(t)
+    })
+}, function(t, e, n) {
+    "use strict";
+    n.d(e, "a", function() {
+        return a
+    }), n.d(e, "b", function() {
+        return r
+    });
+    var a = function() {
+            for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
+            return e
+        },
+        r = function() {
+            for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
+            return e
+        }
+}, function(t, e, n) {
+    "use strict";
     n.d(e, "c", function() {
         return r
     }), n.d(e, "a", function() {
         return o
     });
 
     function p(t, e) {
@@ -30500,15 +30500,15 @@
         V = n(37),
         K = n(69),
         U = n(60),
         G = n(49),
         q = n(32),
         X = n(59),
         $ = n(48),
-        Z = n(254);
+        Z = n(255);
     n.d(e, "b", function() {
         return r
     }), n.d(e, "c", function() {
         return o
     }), n.d(e, "d", function() {
         return i
     });
@@ -30806,15 +30806,15 @@
                     }, t), n)) : null
                 }).filter(function(t) {
                     return t
                 })
             }(t)
         }, [t])
     }
-    var y, T = n(157),
+    var y, T = n(156),
         x = Object(E.forwardRef)(function(t, e) {
             var n = E.useContext(T.b) || {},
                 a = E.useContext(C.b),
                 r = a.getPrefixCls,
                 o = a.getPopupContainer,
                 i = a.direction,
                 a = r(),
@@ -61033,15 +61033,15 @@
         A = n(0),
         r = n.n(A),
         R = n(69),
         I = n(60),
         N = n(49),
         Y = n(59),
         l = n(29),
-        a = n(57),
+        a = n(58),
         B = n(192),
         F = A.createContext(void 0),
         o = n(77),
         c = n(44),
         s = function() {
             return {
                 width: 0,
@@ -61857,19 +61857,45 @@
 }, function(t, e, n) {
     "use strict";
     n.d(e, "b", function() {
         return a
     }), n.d(e, "a", function() {
         return r
     });
-    var e = n(57),
+    var e = n(58),
         a = Object(e.a)("success", "processing", "error", "default", "warning"),
         r = Object(e.a)("pink", "red", "yellow", "orange", "cyan", "green", "blue", "purple", "geekblue", "magenta", "volcano", "gold", "lime")
 }, function(t, e, n) {
     "use strict";
+    n.d(e, "a", function() {
+        return a
+    });
+    var r = n(6),
+        o = n(0),
+        i = o.createContext(null),
+        a = function(t) {
+            var e = t.children,
+                n = function(t, e) {
+                    var n = {};
+                    for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
+                    if (null != t && "function" == typeof Object.getOwnPropertySymbols)
+                        for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
+                    return n
+                }(t, ["children"]),
+                a = o.useContext(i),
+                t = o.useMemo(function() {
+                    return Object(r.a)(Object(r.a)({}, a), n)
+                }, [a, n.prefixCls, n.mode, n.selectable]);
+            return o.createElement(i.Provider, {
+                value: t
+            }, e)
+        };
+    e.b = i
+}, function(t, e, n) {
+    "use strict";
     var l = n(6),
         c = n(15),
         s = n(0),
         u = {
             border: 0,
             background: "transparent",
             padding: 0,
@@ -61903,40 +61929,14 @@
                 },
                 style: i
             }))
         });
     e.a = n
 }, function(t, e, n) {
     "use strict";
-    n.d(e, "a", function() {
-        return a
-    });
-    var r = n(6),
-        o = n(0),
-        i = o.createContext(null),
-        a = function(t) {
-            var e = t.children,
-                n = function(t, e) {
-                    var n = {};
-                    for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
-                    if (null != t && "function" == typeof Object.getOwnPropertySymbols)
-                        for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
-                    return n
-                }(t, ["children"]),
-                a = o.useContext(i),
-                t = o.useMemo(function() {
-                    return Object(r.a)(Object(r.a)({}, a), n)
-                }, [a, n.prefixCls, n.mode, n.selectable]);
-            return o.createElement(i.Provider, {
-                value: t
-            }, e)
-        };
-    e.b = i
-}, function(t, e, n) {
-    "use strict";
     n.d(e, "getAdjust", function() {
         return r
     }), n.d(e, "registerAdjust", function() {
         return o
     }), n(98), n(227);
     var a = {},
         r = function(t) {
@@ -62234,15 +62234,15 @@
         x = n(5),
         _ = n(8),
         a = n(7),
         O = n.n(a),
         w = n(43),
         k = n(0),
         j = n(69),
-        M = n(255);
+        M = n(254);
 
     function E(t) {
         var e = t.className,
             n = t.direction,
             a = t.index,
             r = t.marginDirection,
             o = t.children,
@@ -63995,15 +63995,15 @@
         n = t(305),
         q = t.n(n),
         X = t(62),
         de = t(112),
         mn = t(147),
         $ = t(134),
         Z = t(105),
-        J = t(157),
+        J = t(156),
         gn = t(209),
         Q = t(523),
         tt = t(143),
         T = t(127),
         z = t(198),
         bn = t(15);
 
@@ -66261,15 +66261,15 @@
     }), e.d(t, "sqrDist", function() {
         return G
     }), e.d(t, "sqrLen", function() {
         return q
     }), e.d(t, "forEach", function() {
         return X
     });
-    var r = e(56);
+    var r = e(57);
 
     function n() {
         var t = new r.a(2);
         return r.a != Float32Array && (t[0] = 0, t[1] = 0), t
     }
 
     function a(t) {
@@ -70934,15 +70934,15 @@
         S = n(104),
         r = n(8),
         o = n(13),
         m = n(531),
         g = n(194),
         b = n(35),
         L = n(37),
-        l = n(254),
+        l = n(255),
         v = {
             click: "onClick",
             hover: "onMouseOver"
         },
         a = E.forwardRef(function(s, u) {
             function d() {
                 s.disabled || (f && a(), n(function(t) {
@@ -71512,15 +71512,15 @@
         b = n.n(o),
         o = n(152),
         v = n.n(o),
         y = n(35),
         x = n(0),
         _ = n(69),
         O = n(29),
-        o = n(57),
+        o = n(58),
         w = function(t, e) {
             var n = {};
             for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
             if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                 for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
             return n
         },
@@ -72256,15 +72256,15 @@
     }), e.d(t, "len", function() {
         return $
     }), e.d(t, "sqrLen", function() {
         return Z
     }), e.d(t, "forEach", function() {
         return J
     });
-    var i = e(56);
+    var i = e(57);
 
     function n() {
         var t = new i.a(3);
         return i.a != Float32Array && (t[0] = 0, t[1] = 0, t[2] = 0), t
     }
 
     function a(t) {
@@ -73219,14 +73219,28 @@
             }) : Object(l.a)(Object(l.a)({}, c.a[t]), {
                 overflow: u(r)
             }), i[t].ignoreShake = !0
         }), i
     }
 }, function(t, e, n) {
     "use strict";
+    var a = n(8),
+        r = n(0),
+        o = n(207);
+    e.a = function() {
+        var t = r.useState(!1),
+            t = Object(a.a)(t, 2),
+            e = t[0],
+            n = t[1];
+        return r.useEffect(function() {
+            n(Object(o.b)())
+        }, []), e
+    }
+}, function(t, e, n) {
+    "use strict";
     n.d(e, "a", function() {
         return a
     });
     var r = n(0);
 
     function a(e, t) {
         function n() {
@@ -73243,28 +73257,14 @@
                         t && clearTimeout(t)
                     })
                 }
         }, []), n
     }
 }, function(t, e, n) {
     "use strict";
-    var a = n(8),
-        r = n(0),
-        o = n(207);
-    e.a = function() {
-        var t = r.useState(!1),
-            t = Object(a.a)(t, 2),
-            e = t[0],
-            n = t[1];
-        return r.useEffect(function() {
-            n(Object(o.b)())
-        }, []), e
-    }
-}, function(t, e, n) {
-    "use strict";
     n = n(0), n = Object(n.createContext)({});
     e.a = n
 }, function(t, e, n) {
     "use strict";
     var x = n(5),
         _ = n(6),
         O = n(13),
@@ -75939,18 +75939,18 @@
                 className: j
             }) : O))
         }),
         E = e(95),
         C = e(30),
         S = e(105),
         U = e(69),
-        L = e(157),
+        L = e(156),
         P = e(253),
         G = e(29),
-        a = e(57),
+        a = e(58),
         q = e(193),
         X = e(62),
         $ = e(59),
         Z = e(166),
         n = (r.__ANT_BUTTON = !0, r),
         J = (Object(a.a)("topLeft", "topCenter", "topRight", "bottomLeft", "bottomCenter", "bottomRight", "top", "bottom"), o.Button = n, t.a = o)
 }, function(t, e, n) {
@@ -76564,15 +76564,15 @@
         $ = n(48),
         o = n(22),
         r = n(23),
         i = n(26),
         l = n(27),
         c = n(75),
         f = n(29),
-        s = n(57),
+        s = n(58),
         u = Object(s.a)("text", "input"),
         Z = (s = K.Component, Object(i.a)(d, s), a = Object(l.a)(d), Object(r.a)(d, [{
             key: "renderClearIcon",
             value: function(t) {
                 var e = this.props,
                     n = e.value,
                     a = e.disabled,
@@ -77539,15 +77539,15 @@
         return T.createElement(s.a, Object(l.a)(Object(l.a)({}, t), {}, {
             ref: e,
             icon: c
         }))
     }
     var a = e(250),
         D = e(6),
-        r = e(57),
+        r = e(58),
         T = e(0),
         o = e(62),
         i = e(309),
         z = e(5),
         A = e(282),
         R = e(281),
         I = e(75),
@@ -78500,15 +78500,15 @@
                 form: k,
                 className: o
             })))))
         }),
         tt = e(82),
         Z = e(37),
         J = e(29),
-        d = e(57),
+        d = e(58),
         Q = e(33),
         p = e(121),
         f = e(75),
         h = e(122),
         _ = e(77),
         P = e(41),
         D = e(35),
@@ -88573,15 +88573,15 @@
         _ant_design_charts__WEBPACK_IMPORTED_MODULE_21__ = __webpack_require__(689),
         _ant_design_charts__WEBPACK_IMPORTED_MODULE_22__ = __webpack_require__(690),
         _ant_design_charts__WEBPACK_IMPORTED_MODULE_23__ = __webpack_require__(691),
         _ant_design_charts__WEBPACK_IMPORTED_MODULE_24__ = __webpack_require__(692),
         _ant_design_charts__WEBPACK_IMPORTED_MODULE_25__ = __webpack_require__(693),
         react_highlight_words__WEBPACK_IMPORTED_MODULE_26__ = __webpack_require__(507),
         react_highlight_words__WEBPACK_IMPORTED_MODULE_26___default = __webpack_require__.n(react_highlight_words__WEBPACK_IMPORTED_MODULE_26__),
-        _AntdIcon_react__WEBPACK_IMPORTED_MODULE_27__ = __webpack_require__(58),
+        _AntdIcon_react__WEBPACK_IMPORTED_MODULE_27__ = __webpack_require__(56),
         _ant_design_icons__WEBPACK_IMPORTED_MODULE_28__ = __webpack_require__(127),
         _ant_design_icons__WEBPACK_IMPORTED_MODULE_29__ = __webpack_require__(101),
         _ant_design_icons__WEBPACK_IMPORTED_MODULE_30__ = __webpack_require__(310),
         lodash__WEBPACK_IMPORTED_MODULE_31__ = __webpack_require__(10),
         lodash__WEBPACK_IMPORTED_MODULE_31___default = __webpack_require__.n(lodash__WEBPACK_IMPORTED_MODULE_31__),
         _locales_react__WEBPACK_IMPORTED_MODULE_32__ = __webpack_require__(25),
         _contexts_PropsContext__WEBPACK_IMPORTED_MODULE_33__ = __webpack_require__(28),
@@ -89656,79 +89656,81 @@
                                     disabled: t.disabled
                                 }, t.content || "链接🔗")
                             } : "copyable" === columns[_i6].renderOptions.renderType ? columns[_i6].render = function(t) {
                                 return react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(Text, {
                                     copyable: !0
                                 }, t)
                             } : "dropdown" === columns[_i6].renderOptions.renderType ? columns[_i6].render = function(t, r) {
+                                var e;
                                 return react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(antd__WEBPACK_IMPORTED_MODULE_8__.a, {
                                     overlay: react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(antd__WEBPACK_IMPORTED_MODULE_9__.a, {
                                         onClick: function(t, e, n, a) {
                                             setTimeout(function() {
                                                 setProps({
                                                     nClicksDropdownItem: nClicksDropdownItem + 1,
                                                     recentlyClickedDropdownItemTitle: t.key,
                                                     recentlyDropdownItemClickedDataIndex: columns[_i6].dataIndex,
                                                     recentlyDropdownItemClickedRow: r
                                                 })
                                             }, 200)
                                         }
-                                    }, t.map(function(t) {
+                                    }, (t = t || []).map(function(t) {
                                         return t ? t.isDivider ? react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(antd__WEBPACK_IMPORTED_MODULE_9__.a.Divider, null) : react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(antd__WEBPACK_IMPORTED_MODULE_9__.a.Item, {
                                             icon: react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(_AntdIcon_react__WEBPACK_IMPORTED_MODULE_27__.a, {
                                                 icon: t.icon
                                             }),
                                             disabled: t.disabled,
                                             key: t.title
                                         }, react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement("a", null, t.title)) : null
                                     })),
-                                    arrow: null == (t = columns[_i6].renderOptions) || null == (t = t.dropdownProps) ? void 0 : t.arrow,
-                                    disabled: null == (t = columns[_i6].renderOptions) || null == (t = t.dropdownProps) ? void 0 : t.disabled,
-                                    overlayClassName: null == (t = columns[_i6].renderOptions) || null == (t = t.dropdownProps) ? void 0 : t.overlayClassName,
-                                    overlayStyle: null == (t = columns[_i6].renderOptions) || null == (t = t.dropdownProps) ? void 0 : t.overlayStyle,
-                                    placement: null == (t = columns[_i6].renderOptions) || null == (t = t.dropdownProps) ? void 0 : t.placement,
-                                    trigger: null != (t = columns[_i6].renderOptions) && null != (t = t.dropdownProps) && t.trigger ? [columns[_i6].renderOptions.dropdownProps.trigger] : ["hover"],
+                                    arrow: null == (e = columns[_i6].renderOptions) || null == (e = e.dropdownProps) ? void 0 : e.arrow,
+                                    disabled: (null == (e = columns[_i6].renderOptions) || null == (e = e.dropdownProps) ? void 0 : e.disabled) || 0 === t.length,
+                                    overlayClassName: null == (e = columns[_i6].renderOptions) || null == (t = e.dropdownProps) ? void 0 : t.overlayClassName,
+                                    overlayStyle: null == (e = columns[_i6].renderOptions) || null == (t = e.dropdownProps) ? void 0 : t.overlayStyle,
+                                    placement: null == (e = columns[_i6].renderOptions) || null == (t = e.dropdownProps) ? void 0 : t.placement,
+                                    trigger: null != (e = columns[_i6].renderOptions) && null != (t = e.dropdownProps) && t.trigger ? [columns[_i6].renderOptions.dropdownProps.trigger] : ["hover"],
                                     getPopupContainer: containerId ? function() {
                                         return document.getElementById(containerId) ? document.getElementById(containerId) : document.body
                                     } : void 0
                                 }, react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement("a", {
                                     className: "ant-dropdown-link",
                                     onClick: function(t) {
                                         return t.preventDefault()
                                     }
-                                }, null == (t = columns[_i6].renderOptions) || null == (t = t.dropdownProps) ? void 0 : t.title, " ", react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(_ant_design_icons__WEBPACK_IMPORTED_MODULE_29__.a, null)))
+                                }, null == (e = columns[_i6].renderOptions) || null == (t = e.dropdownProps) ? void 0 : t.title, " ", react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(_ant_design_icons__WEBPACK_IMPORTED_MODULE_29__.a, null)))
                             } : "dropdown-links" === columns[_i6].renderOptions.renderType ? columns[_i6].render = function(t) {
+                                var e;
                                 return react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(antd__WEBPACK_IMPORTED_MODULE_8__.a, {
-                                    overlay: react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(antd__WEBPACK_IMPORTED_MODULE_9__.a, null, t.map(function(t) {
+                                    overlay: react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(antd__WEBPACK_IMPORTED_MODULE_9__.a, null, (t = t || []).map(function(t) {
                                         return t ? t.isDivider ? react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(antd__WEBPACK_IMPORTED_MODULE_9__.a.Divider, null) : react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(antd__WEBPACK_IMPORTED_MODULE_9__.a.Item, {
                                             icon: react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(_AntdIcon_react__WEBPACK_IMPORTED_MODULE_27__.a, {
                                                 icon: t.icon
                                             }),
                                             disabled: t.disabled,
                                             key: t.title
                                         }, react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement("a", {
                                             href: t.href,
                                             target: "_blank"
                                         }, t.title)) : null
                                     })),
-                                    arrow: null == (t = columns[_i6].renderOptions) || null == (t = t.dropdownProps) ? void 0 : t.arrow,
-                                    disabled: null == (t = columns[_i6].renderOptions) || null == (t = t.dropdownProps) ? void 0 : t.disabled,
-                                    overlayClassName: null == (t = columns[_i6].renderOptions) || null == (t = t.dropdownProps) ? void 0 : t.overlayClassName,
-                                    overlayStyle: null == (t = columns[_i6].renderOptions) || null == (t = t.dropdownProps) ? void 0 : t.overlayStyle,
-                                    placement: null == (t = columns[_i6].renderOptions) || null == (t = t.dropdownProps) ? void 0 : t.placement,
-                                    trigger: null != (t = columns[_i6].renderOptions) && null != (t = t.dropdownProps) && t.trigger ? [columns[_i6].renderOptions.dropdownProps.trigger] : ["hover"],
+                                    arrow: null == (e = columns[_i6].renderOptions) || null == (e = e.dropdownProps) ? void 0 : e.arrow,
+                                    disabled: (null == (e = columns[_i6].renderOptions) || null == (e = e.dropdownProps) ? void 0 : e.disabled) || 0 === t.length,
+                                    overlayClassName: null == (e = columns[_i6].renderOptions) || null == (t = e.dropdownProps) ? void 0 : t.overlayClassName,
+                                    overlayStyle: null == (e = columns[_i6].renderOptions) || null == (t = e.dropdownProps) ? void 0 : t.overlayStyle,
+                                    placement: null == (e = columns[_i6].renderOptions) || null == (t = e.dropdownProps) ? void 0 : t.placement,
+                                    trigger: null != (e = columns[_i6].renderOptions) && null != (t = e.dropdownProps) && t.trigger ? [columns[_i6].renderOptions.dropdownProps.trigger] : ["hover"],
                                     getPopupContainer: containerId ? function() {
                                         return document.getElementById(containerId) ? document.getElementById(containerId) : document.body
                                     } : void 0
                                 }, react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement("a", {
                                     className: "ant-dropdown-link",
                                     onClick: function(t) {
                                         return t.preventDefault()
                                     }
-                                }, null == (t = columns[_i6].renderOptions) || null == (t = t.dropdownProps) ? void 0 : t.title, " ", react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(_ant_design_icons__WEBPACK_IMPORTED_MODULE_29__.a, null)))
+                                }, null == (e = columns[_i6].renderOptions) || null == (t = e.dropdownProps) ? void 0 : t.title, " ", react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(_ant_design_icons__WEBPACK_IMPORTED_MODULE_29__.a, null)))
                             } : "ellipsis-copyable" === columns[_i6].renderOptions.renderType ? (columns[_i6].ellipsis = {
                                 showTitle: !1
                             }, columns[_i6].render = function(t) {
                                 return react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(Text, {
                                     copyable: !0,
                                     ellipsis: {
                                         tooltip: t
@@ -90259,15 +90261,15 @@
             hidden: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.bool,
             ellipsis: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.any,
             sorter: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.any,
             render: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.any,
             onCell: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.any,
             title_: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.any
         })),
-        data: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.arrayOf(prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.objectOf(prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.oneOfType([prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string, prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.number, prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.exact({
+        data: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.arrayOf(prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.objectOf(prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.oneOfType([prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.arrayOf(prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.any), prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string, prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.number, prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.exact({
             content: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string,
             href: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string,
             target: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string,
             disabled: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.bool
         }), prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.arrayOf(prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.number), prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.oneOfType([prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.exact({
             color: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string,
             tag: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.oneOfType([prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string, prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.number])
@@ -90346,15 +90348,15 @@
             })]),
             shape: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.oneOf(["circle", "square"])
         }), prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.exact({
             className: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string,
             style: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.object,
             options: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.arrayOf(prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.exact({
                 label: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string,
-                value: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string
+                value: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.oneOfType([prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string, prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.number])
             })),
             listHeight: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.number,
             mode: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.oneOf(["multiple", "tags"]),
             disabled: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.bool,
             size: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.oneOf(["small", "middle", "large"]),
             bordered: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.bool,
             placeholder: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string,
@@ -104305,23 +104307,24 @@
                     display: "flex",
                     justifyContent: "center"
                 }
             }, React.createElement(E.a, null))
         }, x),
         D = e(78),
         T = e(523),
-        I = e(58);
+        R = e(147),
+        I = e(56);
 
-    function R(t) {
+    function N(t) {
         return null != t && "object" == typeof t && !0 === t["@@functional/placeholder"]
     }
 
-    function N(n) {
+    function Y(n) {
         return function t(e) {
-            return 0 === arguments.length || R(e) ? t : n.apply(this, arguments)
+            return 0 === arguments.length || N(e) ? t : n.apply(this, arguments)
         }
     }
 
     function B(t) {
         var n;
         return t && (t = (n = Object(V.cloneDeep)(t)).filter(function(t) {
             return Object(V.isUndefined)(t.parent)
@@ -104335,32 +104338,75 @@
         }), t)
     }
 
     function j(t) {
         return t && !Array.isArray(t) ? [t] : t
     }
 
-    function Y(t) {
-        return (et(t.props.disabled) && t.props._dashprivate_layout && t.props._dashprivate_layout.props ? t.props._dashprivate_layout : t).props
+    function et(t) {
+        return (nt(t.props.disabled) && t.props._dashprivate_layout && t.props._dashprivate_layout.props ? t.props._dashprivate_layout : t).props
     }
-    var et = N(function(t) {
+    var nt = Y(function(t) {
         return null == t
     });
 
-    function nt() {
-        return (nt = Object.assign ? Object.assign.bind() : function(t) {
+    function at(t) {
+        return (at = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
+            return typeof t
+        } : function(t) {
+            return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
+        })(t)
+    }
+
+    function rt() {
+        return (rt = Object.assign ? Object.assign.bind() : function(t) {
             for (var e = 1; e < arguments.length; e++) {
                 var n, a = arguments[e];
                 for (n in a) Object.prototype.hasOwnProperty.call(a, n) && (t[n] = a[n])
             }
             return t
         }).apply(this, arguments)
     }
 
-    function at(t) {
+    function ot(e, t) {
+        var n, a = Object.keys(e);
+        return Object.getOwnPropertySymbols && (n = Object.getOwnPropertySymbols(e), t && (n = n.filter(function(t) {
+            return Object.getOwnPropertyDescriptor(e, t).enumerable
+        })), a.push.apply(a, n)), a
+    }
+
+    function it(a) {
+        for (var t = 1; t < arguments.length; t++) {
+            var r = null != arguments[t] ? arguments[t] : {};
+            t % 2 ? ot(Object(r), !0).forEach(function(t) {
+                var e, n;
+                e = a, t = r[n = t], (n = function() {
+                    var t = function(t) {
+                        if ("object" !== at(t) || null === t) return t;
+                        var e = t[Symbol.toPrimitive];
+                        if (void 0 === e) return String(t);
+                        e = e.call(t, "string");
+                        if ("object" !== at(e)) return e;
+                        throw new TypeError("@@toPrimitive must return a primitive value.")
+                    }(n);
+                    return "symbol" === at(t) ? t : String(t)
+                }()) in e ? Object.defineProperty(e, n, {
+                    value: t,
+                    enumerable: !0,
+                    configurable: !0,
+                    writable: !0
+                }) : e[n] = t
+            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(r)) : ot(Object(r)).forEach(function(t) {
+                Object.defineProperty(a, t, Object.getOwnPropertyDescriptor(r, t))
+            })
+        }
+        return a
+    }
+
+    function lt(t) {
         var e = t.id,
             n = t.className,
             s = t.setProps,
             a = t.style,
             r = t.key,
             u = t.treeData,
             o = t.treeDataMode,
@@ -104396,22 +104442,22 @@
             }, []), Object(Wt.useMemo)(function() {
                 return B(u)
             }, [u])),
             E = ("flat" === o && (u = E), {
                 expandedKeys: d
             }),
             E = Object(V.omitBy)(E, V.isUndefined);
-        return React.createElement(T.a, nt({
+        return React.createElement(T.a, rt({
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             treeData: function t(e) {
                 if (Object(V.isObject)(e))
-                    if (e.tooltipProps && (e.title = React.createElement(D.a, e.tooltipProps, e.title)), e.children) {
+                    if (e.tooltipProps && Object(V.isString)(e.title) && (e.title = React.createElement(D.a, e.tooltipProps, e.title)), e.children) {
                         Object(V.isString)(e.icon) && (e.icon = React.createElement(I.a, {
                             icon: e.icon
                         }));
                         for (var n = 0; n < e.children.length; n++) e.children[n] = t(e.children[n])
                     } else Object(V.isString)(e.icon) && (e.icon = React.createElement(I.a, {
                         icon: e.icon
                     }));
@@ -104428,15 +104474,15 @@
             defaultExpandParent: m,
             defaultCheckedKeys: b,
             defaultSelectedKeys: v,
             checkStrictly: g,
             multiple: y,
             showLine: x,
             onSelect: function(t) {
-                s({
+                console.log("节点选择发生", t), s({
                     selectedKeys: t
                 })
             },
             onCheck: function(t, e) {
                 s(g ? {
                     checkedKeys: t.checked,
                     halfCheckedKeys: t.halfChecked
@@ -104453,19 +104499,41 @@
             onDragEnter: function(t) {
                 s({
                     expandedKeys: t.expandedKeys
                 })
             },
             showIcon: _,
             height: O,
-            titleRender: function(t) {
-                return React.createElement("span", {
-                    className: t.className ? "ant-tree-title ".concat(t.className) : "ant-tree-title",
-                    style: t.style
-                }, t.title)
+            titleRender: function(e) {
+                return e.contextMenu ? React.createElement(R.a, {
+                    menu: {
+                        items: e.contextMenu.map(function(t) {
+                            return it(it({}, t), {}, {
+                                icon: React.createElement(I.a, {
+                                    icon: t.icon
+                                })
+                            })
+                        }),
+                        onClick: function(t) {
+                            t.domEvent.stopPropagation(), s({
+                                clickedContextMenu: {
+                                    nodeKey: e.key,
+                                    menuKey: t.key
+                                }
+                            })
+                        }
+                    },
+                    trigger: ["contextMenu"]
+                }, React.createElement("span", {
+                    className: e.className ? "ant-tree-title ".concat(e.className) : "ant-tree-title",
+                    style: e.style
+                }, e.title)) : React.createElement("span", {
+                    className: e.className ? "ant-tree-title ".concat(e.className) : "ant-tree-title",
+                    style: e.style
+                }, e.title)
             },
             showLeafIcon: !1,
             draggable: w && "flat" !== o,
             blockNode: w && "flat" !== o,
             onDrop: w && "flat" !== o ? function(t) {
                 function r(t, e, n) {
                     for (var a = 0; a < t.length; a++) {
@@ -104506,15 +104574,20 @@
             disableCheckbox: n.a.bool,
             selectable: n.a.bool,
             style: n.a.object,
             className: n.a.string,
             tooltipProps: n.a.exact({
                 title: n.a.string,
                 placement: n.a.oneOf(["top", "left", "right", "bottom", "topLeft", "topRight", "bottomLeft", "bottomRight"])
-            })
+            }),
+            contextMenu: n.a.arrayOf(n.a.exact({
+                key: n.a.string,
+                label: n.a.string,
+                icon: n.a.string
+            }))
         },
         r = n.a.shape(a),
         a = (a.children = n.a.arrayOf(r), n.a.arrayOf(r)),
         r = {
             title: n.a.string.isRequired,
             key: n.a.string.isRequired,
             disabled: n.a.bool,
@@ -104524,17 +104597,22 @@
             selectable: n.a.bool,
             parent: n.a.string,
             style: n.a.object,
             className: n.a.string,
             tooltipProps: n.a.exact({
                 title: n.a.string,
                 placement: n.a.oneOf(["top", "left", "right", "bottom", "topLeft", "topRight", "bottomLeft", "bottomRight"])
-            })
+            }),
+            contextMenu: n.a.arrayOf(n.a.exact({
+                key: n.a.string,
+                label: n.a.string,
+                icon: n.a.string
+            }))
         },
-        rt = (at.propTypes = {
+        ct = (lt.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.number]),
             style: n.a.object,
             key: n.a.string,
             treeDataMode: n.a.oneOf(["tree", "flat"]),
             treeData: n.a.oneOfType([a, n.a.arrayOf(r)]),
             showIcon: n.a.bool,
@@ -104553,180 +104631,184 @@
             checkStrictly: n.a.bool,
             showLine: n.a.oneOfType([n.a.bool, n.a.exact({
                 showLeafIcon: n.a.bool
             })]),
             height: n.a.number,
             draggable: n.a.bool,
             draggedNodeKey: n.a.string,
+            clickedContextMenu: n.a.exact({
+                nodeKey: n.a.string,
+                menuKey: n.a.string
+            }),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func,
             persistence: n.a.oneOfType([n.a.bool, n.a.string, n.a.number]),
             persisted_props: n.a.arrayOf(n.a.oneOf(["selectedKeys", "checkedKeys", "expandedKeys", "halfCheckedKeys"])),
             persistence_type: n.a.oneOf(["local", "session", "memory"])
-        }, at.defaultProps = {
+        }, lt.defaultProps = {
             showIcon: !1,
             treeDataMode: "tree",
             checkable: !1,
             defaultExpandAll: !1,
             defaultExpandParent: !1,
             checkStrictly: !1,
             multiple: !1,
             selectable: !0,
             showLine: {
                 showLeafIcon: !1
             },
             draggable: !1,
             persisted_props: ["selectedKeys", "checkedKeys", "expandedKeys", "halfCheckedKeys"],
             persistence_type: "local"
-        }, at),
-        ot = e(456),
+        }, lt),
+        st = e(456),
         Ut = e(11),
         Gt = e(8),
-        it = e(72),
+        ut = e(72),
         i = e(22),
         a = e(23),
         r = e(26),
         o = e(27),
         qt = e(13),
-        lt = e(66),
-        ct = e(35),
-        st = e(33);
+        dt = e(66),
+        pt = e(35),
+        ft = e(33);
 
-    function ut(r) {
+    function ht(r) {
         function t() {
             if (null == o) {
                 for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
-                o = Object(st.a)((a = e, function() {
+                o = Object(ft.a)((a = e, function() {
                     o = null, r.apply(void 0, Object(Ut.a)(a))
                 }))
             }
             var a
         }
         var o;
         return t.cancel = function() {
-            st.a.cancel(o), o = null
+            ft.a.cancel(o), o = null
         }, t
     }
 
-    function dt() {
+    function mt() {
         return function(e, n, t) {
             var a = t.value,
                 r = !1;
             return {
                 configurable: !0,
                 get: function() {
                     var t;
-                    return r || this === e.prototype || this.hasOwnProperty(n) ? a : (t = ut(a.bind(this)), r = !0, Object.defineProperty(this, n, {
+                    return r || this === e.prototype || this.hasOwnProperty(n) ? a : (t = ht(a.bind(this)), r = !0, Object.defineProperty(this, n, {
                         value: t,
                         configurable: !0,
                         writable: !0
                     }), r = !1, t)
                 }
             }
         }
     }
 
-    function pt(t) {
+    function gt(t) {
         return t !== window ? t.getBoundingClientRect() : {
             top: 0,
             bottom: window.innerHeight
         }
     }
 
-    function ft(t, e, n) {
+    function bt(t, e, n) {
         if (void 0 !== n && e.top > t.top - n) return n + e.top
     }
 
-    function ht(t, e, n) {
+    function vt(t, e, n) {
         if (void 0 !== n && e.bottom < t.bottom + n) return n + (window.innerHeight - e.bottom)
     }
-    var mt = ["resize", "scroll", "touchstart", "touchmove", "touchend", "pageshow", "load"],
-        gt = [];
+    var yt = ["resize", "scroll", "touchstart", "touchmove", "touchend", "pageshow", "load"],
+        xt = [];
 
-    function bt(e, t) {
+    function _t(e, t) {
         var n;
-        e && ((n = gt.find(function(t) {
+        e && ((n = xt.find(function(t) {
             return t.target === e
         })) ? n.affixList.push(t) : (n = {
             target: e,
             affixList: [t],
             eventHandlers: {}
-        }, gt.push(n), mt.forEach(function(t) {
-            n.eventHandlers[t] = Object(it.a)(e, t, function() {
+        }, xt.push(n), yt.forEach(function(t) {
+            n.eventHandlers[t] = Object(ut.a)(e, t, function() {
                 n.affixList.forEach(function(t) {
                     t.lazyUpdatePosition()
                 })
             })
         })))
     }
 
-    function vt(n) {
-        var e = gt.find(function(t) {
+    function Ot(n) {
+        var e = xt.find(function(t) {
             var e = t.affixList.some(function(t) {
                 return t === n
             });
             return e && (t.affixList = t.affixList.filter(function(t) {
                 return t !== n
             })), e
         });
-        e && 0 === e.affixList.length && (gt = gt.filter(function(t) {
+        e && 0 === e.affixList.length && (xt = xt.filter(function(t) {
             return t !== e
-        }), mt.forEach(function(t) {
+        }), yt.forEach(function(t) {
             t = e.eventHandlers[t];
             t && t.remove && t.remove()
         }))
     }
 
-    function yt(t, e, n, a) {
+    function wt(t, e, n, a) {
         var r, o = arguments.length,
             i = o < 3 ? e : null === a ? a = Object.getOwnPropertyDescriptor(e, n) : a;
         if ("object" === ("undefined" == typeof Reflect ? "undefined" : Object(qt.a)(Reflect)) && "function" == typeof Reflect.decorate) i = Reflect.decorate(t, e, n, a);
         else
             for (var l = t.length - 1; 0 <= l; l--)(r = t[l]) && (i = (o < 3 ? r(i) : 3 < o ? r(e, n, i) : r(e, n)) || i);
         3 < o && i && Object.defineProperty(e, n, i)
     }
-    var xt;
+    var kt;
 
-    function _t() {
+    function jt() {
         return "undefined" != typeof window ? window : null
-    }(l = xt = xt || {})[l.None = 0] = "None", l[l.Prepare = 1] = "Prepare";
-    l = Wt.Component, Object(r.a)(kt, l), Ot = Object(o.a)(kt), Object(a.a)(kt, [{
+    }(l = kt = kt || {})[l.None = 0] = "None", l[l.Prepare = 1] = "Prepare";
+    l = Wt.Component, Object(r.a)(Lt, l), Mt = Object(o.a)(Lt), Object(a.a)(Lt, [{
         key: "getTargetFunc",
         value: function() {
             var t = this.context.getTargetContainer,
                 e = this.props.target;
-            return void 0 !== e ? e : null != t ? t : _t
+            return void 0 !== e ? e : null != t ? t : jt
         }
     }, {
         key: "componentDidMount",
         value: function() {
             var t = this,
                 e = this.getTargetFunc();
             e && (this.timeout = setTimeout(function() {
-                bt(e(), t), t.updatePosition()
+                _t(e(), t), t.updatePosition()
             }))
         }
     }, {
         key: "componentDidUpdate",
         value: function(t) {
             var e = this.state.prevTarget,
                 n = this.getTargetFunc(),
                 n = (null == n ? void 0 : n()) || null;
-            e !== n && (vt(this), n && (bt(n, this), this.updatePosition()), this.setState({
+            e !== n && (Ot(this), n && (_t(n, this), this.updatePosition()), this.setState({
                 prevTarget: n
             })), t.offsetTop === this.props.offsetTop && t.offsetBottom === this.props.offsetBottom || this.updatePosition(), this.measure()
         }
     }, {
         key: "componentWillUnmount",
         value: function() {
-            clearTimeout(this.timeout), vt(this), this.updatePosition.cancel(), this.lazyUpdatePosition.cancel()
+            clearTimeout(this.timeout), Ot(this), this.updatePosition.cancel(), this.lazyUpdatePosition.cancel()
         }
     }, {
         key: "updatePosition",
         value: function() {
             this.prepareMeasure()
         }
     }, {
@@ -104735,18 +104817,18 @@
             var t = this.getTargetFunc(),
                 e = this.state.affixStyle;
             if (t && e) {
                 var n = this.getOffsetTop(),
                     a = this.getOffsetBottom(),
                     t = t();
                 if (t && this.placeholderNode) {
-                    var t = pt(t),
-                        r = pt(this.placeholderNode),
-                        n = ft(r, t, n),
-                        r = ht(r, t, a);
+                    var t = gt(t),
+                        r = gt(this.placeholderNode),
+                        n = bt(r, t, n),
+                        r = vt(r, t, a);
                     if (void 0 !== n && e.top === n || void 0 !== r && e.bottom === r) return
                 }
             }
             this.prepareMeasure()
         }
     }, {
         key: "render",
@@ -104755,41 +104837,41 @@
                 e = this.state,
                 n = e.affixStyle,
                 e = e.placeholderStyle,
                 a = this.props,
                 r = a.affixPrefixCls,
                 a = a.children,
                 r = Kt()(Object(Vt.a)({}, r, !!n)),
-                o = Object(ct.a)(this.props, ["prefixCls", "offsetTop", "offsetBottom", "target", "onChange", "affixPrefixCls"]);
-            return Wt.createElement(lt.a, {
+                o = Object(pt.a)(this.props, ["prefixCls", "offsetTop", "offsetBottom", "target", "onChange", "affixPrefixCls"]);
+            return Wt.createElement(dt.a, {
                 onResize: function() {
                     t.updatePosition()
                 }
             }, Wt.createElement("div", Object(Et.a)({}, o, {
                 ref: this.savePlaceholderNode
             }), n && Wt.createElement("div", {
                 style: e,
                 "aria-hidden": "true"
             }), Wt.createElement("div", {
                 className: r,
                 ref: this.saveFixedNode,
                 style: n
-            }, Wt.createElement(lt.a, {
+            }, Wt.createElement(dt.a, {
                 onResize: function() {
                     t.updatePosition()
                 }
             }, a))))
         }
     }]);
-    var Ot, wt = kt;
+    var Mt, St = Lt;
 
-    function kt() {
+    function Lt() {
         var l;
-        return Object(i.a)(this, kt), (l = Ot.apply(this, arguments)).state = {
-            status: xt.None,
+        return Object(i.a)(this, Lt), (l = Mt.apply(this, arguments)).state = {
+            status: kt.None,
             lastAffix: !1,
             prevTarget: null
         }, l.getOffsetTop = function() {
             var t = l.props,
                 e = t.offsetBottom,
                 t = t.offsetTop;
             return void 0 === e && void 0 === t ? 0 : t
@@ -104801,17 +104883,17 @@
             l.fixedNode = t
         }, l.measure = function() {
             var t, e, n, a = l.state,
                 r = a.status,
                 a = a.lastAffix,
                 o = l.props.onChange,
                 i = l.getTargetFunc();
-            r === xt.Prepare && l.fixedNode && l.placeholderNode && i && (r = l.getOffsetTop(), t = l.getOffsetBottom(), i = i()) && (e = {
-                status: xt.None
-            }, i = pt(i), r = ft(n = pt(l.placeholderNode), i, r), i = ht(n, i, t), 0 === n.top && 0 === n.left && 0 === n.width && 0 === n.height || (void 0 !== r ? (e.affixStyle = {
+            r === kt.Prepare && l.fixedNode && l.placeholderNode && i && (r = l.getOffsetTop(), t = l.getOffsetBottom(), i = i()) && (e = {
+                status: kt.None
+            }, i = gt(i), r = bt(n = gt(l.placeholderNode), i, r), i = vt(n, i, t), 0 === n.top && 0 === n.left && 0 === n.width && 0 === n.height || (void 0 !== r ? (e.affixStyle = {
                 position: "fixed",
                 top: r,
                 width: n.width,
                 height: n.height
             }, e.placeholderStyle = {
                 width: n.width,
                 height: n.height
@@ -104822,45 +104904,45 @@
                 height: n.height
             }, e.placeholderStyle = {
                 width: n.width,
                 height: n.height
             }), e.lastAffix = !!e.affixStyle, o && a !== e.lastAffix && o(e.lastAffix), l.setState(e)))
         }, l.prepareMeasure = function() {
             l.setState({
-                status: xt.Prepare,
+                status: kt.Prepare,
                 affixStyle: void 0,
                 placeholderStyle: void 0
             })
         }, l
     }
-    wt.contextType = q.b, yt([dt()], wt.prototype, "updatePosition", null), yt([dt()], wt.prototype, "lazyUpdatePosition", null);
-    var jt = Wt.forwardRef(function(t, e) {
+    St.contextType = q.b, wt([mt()], St.prototype, "updatePosition", null), wt([mt()], St.prototype, "lazyUpdatePosition", null);
+    var Pt = Wt.forwardRef(function(t, e) {
             var n = t.prefixCls,
                 n = (0, Wt.useContext(q.b).getPrefixCls)("affix", n),
                 t = Object(Et.a)(Object(Et.a)({}, t), {
                     affixPrefixCls: n
                 });
-            return Wt.createElement(wt, Object(Et.a)({}, t, {
+            return Wt.createElement(St, Object(Et.a)({}, t, {
                 ref: e
             }))
         }),
-        Mt = e(160),
-        St = e(196),
-        Lt = Wt.createContext(void 0);
+        Dt = e(160),
+        Tt = e(196),
+        zt = Wt.createContext(void 0);
 
-    function Pt() {
+    function At() {
         return window
     }
 
-    function Dt(t, e) {
+    function Rt(t, e) {
         var n;
         return t.getClientRects().length ? (n = t.getBoundingClientRect()).width || n.height ? e === window ? (e = t.ownerDocument.documentElement, n.top - e.clientTop) : n.top - e.getBoundingClientRect().top : n.top : 0
     }
 
-    function Tt(t) {
+    function It(t) {
         function a(t) {
             var e;
             y.current !== t && (e = "function" == typeof h ? h(t) : t, v(e), y.current = e, null != p) && p(t)
         }
         var e = t.anchorPrefixCls,
             n = void 0 === (n = t.className) ? "" : n,
             r = t.style,
@@ -104882,15 +104964,15 @@
             v = t[1],
             y = Wt.useRef(b),
             x = Wt.useRef(null),
             _ = Wt.useRef(null),
             O = Wt.useRef(!1),
             w = (t = Wt.useContext(q.b)).direction,
             t = t.getTargetContainer,
-            k = null != (f = null != f ? f : t) ? f : Pt,
+            k = null != (f = null != f ? f : t) ? f : At,
             t = JSON.stringify(m),
             j = Wt.useCallback(function(e) {
                 m.includes(e) || g(function(t) {
                     return [].concat(Object(Ut.a)(t), [e])
                 })
             }, [t]),
             M = Wt.useCallback(function(e) {
@@ -104904,30 +104986,30 @@
                 var t;
                 O.current || "function" == typeof h || (t = function(t, e, n) {
                     var a = 1 < arguments.length && void 0 !== e ? e : 0,
                         r = 2 < arguments.length && void 0 !== n ? n : 5,
                         o = [],
                         i = k();
                     return t.forEach(function(t) {
-                        var e = Rt.exec(null == t ? void 0 : t.toString());
-                        e && (e = document.getElementById(e[1])) && (e = Dt(e, i)) < a + r && o.push({
+                        var e = Bt.exec(null == t ? void 0 : t.toString());
+                        e && (e = document.getElementById(e[1])) && (e = Rt(e, i)) < a + r && o.push({
                             link: t,
                             top: e
                         })
                     }), o.length ? o.reduce(function(t, e) {
                         return e.top > t.top ? e : t
                     }).link : ""
                 }(m, void 0 !== u ? u : o || 0, s), a(t))
             }, [t, u, o]),
             C = Wt.useCallback(function(t) {
                 a(t);
                 var e = k(),
-                    n = Object(Mt.a)(e, !0),
-                    t = Rt.exec(t);
-                t && (t = document.getElementById(t[1])) && (n = n + Dt(t, e), n -= void 0 !== u ? u : o || 0, O.current = !0, Object(St.a)(n, {
+                    n = Object(Dt.a)(e, !0),
+                    t = Bt.exec(t);
+                t && (t = document.getElementById(t[1])) && (n = n + Rt(t, e), n -= void 0 !== u ? u : o || 0, O.current = !0, Object(Tt.a)(n, {
                     getContainer: k,
                     callback: function() {
                         O.current = !1
                     }
                 }))
             }, [u, o]),
             f = Kt()(Object(Vt.a)({}, "".concat(e, "-ink-ball-visible"), b), "".concat(e, "-ink-ball")),
@@ -104946,15 +105028,15 @@
                 className: "".concat(e, "-ink")
             }, Wt.createElement("span", {
                 className: f,
                 ref: _
             })), c)),
             w = (Wt.useEffect(function() {
                 var t = k(),
-                    e = Object(it.a)(t, "scroll", E);
+                    e = Object(ut.a)(t, "scroll", E);
                 return E(),
                     function() {
                         null != e && e.remove()
                     }
             }, [t]), Wt.useEffect(function() {
                 "function" == typeof h && a(h(y.current || ""))
             }, [h]), Wt.useEffect(function() {
@@ -104965,31 +105047,31 @@
                     registerLink: j,
                     unregisterLink: M,
                     scrollTo: C,
                     activeLink: b,
                     onClick: d
                 }
             }, [b, d, C]));
-        return Wt.createElement(Lt.Provider, {
+        return Wt.createElement(zt.Provider, {
             value: w
-        }, i ? Wt.createElement(jt, {
+        }, i ? Wt.createElement(Pt, {
             offsetTop: o,
             target: k
         }, r) : r)
     }
 
-    function zt(t) {
+    function Nt(t) {
         var e = t.prefixCls,
             e = (0, Wt.useContext(q.b).getPrefixCls)("anchor", e);
-        return Wt.createElement(Tt, Object(Et.a)({}, t, {
+        return Wt.createElement(It, Object(Et.a)({}, t, {
             anchorPrefixCls: e
         }))
     }
 
-    function At(t) {
+    function Yt(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.linkDict,
             i = t.align,
             l = t.containerId,
@@ -105000,15 +105082,15 @@
             p = t.loading_state,
             f = t.setProps;
         return H.a.createElement("div", {
             style: {
                 float: i
             },
             "data-dash-is-loading": p && p.is_loading || void 0
-        }, H.a.createElement(It, {
+        }, H.a.createElement(Ft, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             onClick: function(t, e) {
                 f({
                     clickedLink: e
@@ -105018,44 +105100,44 @@
                 return document.getElementById(l)
             } : void 0,
             targetOffset: c,
             affix: s,
             bounds: u,
             offsetTop: d
         }, function t(e) {
-            if (e.hasOwnProperty("href")) e = e.hasOwnProperty("children") ? H.a.createElement(Nt, {
+            if (e.hasOwnProperty("href")) e = e.hasOwnProperty("children") ? H.a.createElement(Ht, {
                 href: e.href,
                 title: e.title,
                 target: e.target
-            }, t(e.children)) : H.a.createElement(Nt, {
+            }, t(e.children)) : H.a.createElement(Ht, {
                 href: e.href,
                 title: e.title,
                 target: e.target
             });
             else
                 for (var n = 0; n < e.length; n++) e[n] = t(e[n]);
             return e
         }(o)))
     }
-    var Rt = /#([\S ]+)$/,
-        It = (zt.Link = function(t) {
+    var Bt = /#([\S ]+)$/,
+        Ft = (Nt.Link = function(t) {
             function a(t) {
                 null != p && p(t, {
                     title: o,
                     href: r
                 }), null != d && d(r)
             }
             var e = t.href,
                 r = void 0 === e ? "#" : e,
                 o = t.title,
                 i = t.prefixCls,
                 l = t.children,
                 c = t.className,
                 s = t.target,
-                e = Wt.useContext(Lt) || {},
+                e = Wt.useContext(zt) || {},
                 n = e.registerLink,
                 u = e.unregisterLink,
                 d = e.scrollTo,
                 p = e.onClick,
                 f = e.activeLink;
             Wt.useEffect(function() {
                 return null != n && n(r),
@@ -105074,24 +105156,24 @@
                     className: t,
                     href: r,
                     title: "string" == typeof o ? o : "",
                     target: s,
                     onClick: a
                 }, o), l)
             })
-        }, zt),
-        Nt = It.Link,
+        }, Nt),
+        Ht = Ft.Link,
         l = {
             title: n.a.string,
             href: n.a.string,
             target: n.a.string
         },
         c = n.a.shape(l),
         l = (l.children = n.a.arrayOf(c), n.a.arrayOf(c)),
-        Yt = (At.propTypes = {
+        Xt = (Yt.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             linkDict: l.isRequired,
             align: n.a.oneOf(["left", "right"]),
             containerId: n.a.string,
@@ -105102,41 +105184,41 @@
             clickedLink: n.a.object,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, At.defaultProps = {
+        }, Yt.defaultProps = {
             align: "right",
             affix: !0,
             bounds: 5
-        }, At),
+        }, Yt),
         c = e(91),
-        Xt = e.n(c),
-        $t = e(30),
-        Bt = e(16),
+        $t = e.n(c),
+        Zt = e(30),
+        Jt = e(16),
         Ct = e(4),
         X = e(15),
-        Zt = Wt.createContext({
+        Qt = Wt.createContext({
             min: 0,
             max: 0,
             direction: "ltr",
             step: 1,
             includedStart: 0,
             includedEnd: 0,
             tabIndex: 0
         });
 
-    function Ft(t, e, n) {
+    function te(t, e, n) {
         return (t - e) / (n - e)
     }
 
-    function Ht(t, e, n, a) {
-        var r = Ft(e, n, a),
+    function ee(t, e, n, a) {
+        var r = te(e, n, a),
             o = {};
         switch (t) {
             case "rtl":
                 o.right = "".concat(100 * r, "%"), o.transform = "translateX(50%)";
                 break;
             case "btt":
                 o.bottom = "".concat(100 * r, "%"), o.transform = "translateY(50%)";
@@ -105146,43 +105228,43 @@
                 break;
             default:
                 o.left = "".concat(100 * r, "%"), o.transform = "translateX(-50%)"
         }
         return o
     }
 
-    function Jt(t, e) {
+    function ne(t, e) {
         return Array.isArray(t) ? t[e] : t
     }
-    var Qt = ["prefixCls", "value", "valueIndex", "onStartMove", "style", "render", "dragging", "onOffsetChange"],
-        te = Wt.forwardRef(function(t, e) {
+    var ae = ["prefixCls", "value", "valueIndex", "onStartMove", "style", "render", "dragging", "onOffsetChange"],
+        re = Wt.forwardRef(function(t, e) {
             function n(t) {
                 m || i(t, o)
             }
             var a = t.prefixCls,
                 r = t.value,
                 o = t.valueIndex,
                 i = t.onStartMove,
                 l = t.style,
                 c = t.render,
                 s = t.dragging,
                 u = t.onOffsetChange,
-                t = Object(Bt.a)(t, Qt),
-                d = Wt.useContext(Zt),
+                t = Object(Jt.a)(t, ae),
+                d = Wt.useContext(Qt),
                 p = d.min,
                 f = d.max,
                 h = d.direction,
                 m = d.disabled,
                 g = d.range,
                 b = d.tabIndex,
                 v = d.ariaLabelForHandle,
                 y = d.ariaLabelledByForHandle,
                 d = d.ariaValueTextFormatterForHandle,
                 x = "".concat(a, "-handle"),
-                _ = Ht(h, r, p, f),
+                _ = ee(h, r, p, f),
                 x = Wt.createElement("div", Object(Et.a)({
                     ref: e,
                     className: Kt()(x, (e = {}, Object(Vt.a)(e, "".concat(x, "-").concat(o + 1), g), Object(Vt.a)(e, "".concat(x, "-dragging"), s), e)),
                     style: Object(Ct.a)(Object(Ct.a)({}, _), l),
                     onMouseDown: n,
                     onTouchStart: n,
                     onKeyDown: function(t) {
@@ -105212,93 +105294,93 @@
                                     break;
                                 case X.a.PAGE_DOWN:
                                     e = -2
                             }
                             null !== e && (t.preventDefault(), u(e, o))
                         }
                     },
-                    tabIndex: m ? null : Jt(b, o),
+                    tabIndex: m ? null : ne(b, o),
                     role: "slider",
                     "aria-valuemin": p,
                     "aria-valuemax": f,
                     "aria-valuenow": r,
                     "aria-disabled": m,
-                    "aria-label": Jt(v, o),
-                    "aria-labelledby": Jt(y, o),
-                    "aria-valuetext": null == (g = Jt(d, o)) ? void 0 : g(r)
+                    "aria-label": ne(v, o),
+                    "aria-labelledby": ne(y, o),
+                    "aria-valuetext": null == (g = ne(d, o)) ? void 0 : g(r)
                 }, t));
             return x = c ? c(x, {
                 index: o,
                 prefixCls: a,
                 value: r,
                 dragging: s
             }) : x
         }),
-        ee = ["prefixCls", "style", "onStartMove", "onOffsetChange", "values", "handleRender", "draggingIndex"],
-        ne = Wt.forwardRef(function(t, e) {
+        oe = ["prefixCls", "style", "onStartMove", "onOffsetChange", "values", "handleRender", "draggingIndex"],
+        ie = Wt.forwardRef(function(t, e) {
             var n = t.prefixCls,
                 a = t.style,
                 r = t.onStartMove,
                 o = t.onOffsetChange,
                 i = t.values,
                 l = t.handleRender,
                 c = t.draggingIndex,
-                s = Object(Bt.a)(t, ee),
+                s = Object(Jt.a)(t, oe),
                 u = Wt.useRef({});
             return Wt.useImperativeHandle(e, function() {
                 return {
                     focus: function(t) {
                         null != (t = u.current[t]) && t.focus()
                     }
                 }
             }), Wt.createElement(Wt.Fragment, null, i.map(function(t, e) {
-                return Wt.createElement(te, Object(Et.a)({
+                return Wt.createElement(re, Object(Et.a)({
                     ref: function(t) {
                         t ? u.current[e] = t : delete u.current[e]
                     },
                     dragging: c === e,
                     prefixCls: n,
-                    style: Jt(a, e),
+                    style: ne(a, e),
                     key: e,
                     value: t,
                     valueIndex: e,
                     onStartMove: r,
                     onOffsetChange: o,
                     render: l
                 }, s))
             }))
         });
 
-    function ae(t) {
+    function le(t) {
         t = "touches" in t ? t.touches[0] : t;
         return {
             pageX: t.pageX,
             pageY: t.pageY
         }
     }
 
-    function re(t) {
+    function ce(t) {
         function e(t) {
             !d && l && l(t, -1)
         }
         var n = t.prefixCls,
             a = t.style,
             r = t.start,
             o = t.end,
             i = t.index,
             l = t.onStartMove,
-            t = Wt.useContext(Zt),
+            t = Wt.useContext(Qt),
             c = t.direction,
             s = t.min,
             u = t.max,
             d = t.disabled,
             t = t.range,
             n = "".concat(n, "-track"),
-            p = Ft(r, s, u),
-            f = Ft(o, s, u),
+            p = te(r, s, u),
+            f = te(o, s, u),
             h = {};
         switch (c) {
             case "rtl":
                 h.right = "".concat(100 * p, "%"), h.width = "".concat(100 * f - 100 * p, "%");
                 break;
             case "btt":
                 h.bottom = "".concat(100 * p, "%"), h.height = "".concat(100 * f - 100 * p, "%");
@@ -105313,21 +105395,21 @@
             className: Kt()(n, t && "".concat(n, "-").concat(i + 1)),
             style: Object(Ct.a)(Object(Ct.a)({}, h), a),
             onMouseDown: e,
             onTouchStart: e
         })
     }
 
-    function oe(t) {
+    function se(t) {
         var a = t.prefixCls,
             r = t.style,
             o = t.values,
             i = t.startPoint,
             l = t.onStartMove,
-            t = Wt.useContext(Zt),
+            t = Wt.useContext(Qt),
             e = t.included,
             c = t.range,
             s = t.min,
             t = Wt.useMemo(function() {
                 var t, e;
                 if (!c) return 0 === o.length ? [] : (t = null != i ? i : s, e = o[0], [{
                     start: Math.min(t, e),
@@ -105338,127 +105420,127 @@
                     end: o[a + 1]
                 });
                 return n
             }, [o, c, i, s]);
         return e ? t.map(function(t, e) {
             var n = t.start,
                 t = t.end;
-            return Wt.createElement(re, {
+            return Wt.createElement(ce, {
                 index: e,
                 prefixCls: a,
-                style: Jt(r, e),
+                style: ne(r, e),
                 start: n,
                 end: t,
                 key: e,
                 onStartMove: l
             })
         }) : null
     }
 
-    function ie(t) {
+    function ue(t) {
         var e = t.prefixCls,
             n = t.style,
             a = t.children,
             r = t.value,
             o = t.onClick,
-            t = Wt.useContext(Zt),
+            t = Wt.useContext(Qt),
             i = t.min,
             l = t.max,
             c = t.direction,
             s = t.includedStart,
             u = t.includedEnd,
             t = t.included,
             e = "".concat(e, "-text"),
-            c = Ht(c, r, i, l);
+            c = ee(c, r, i, l);
         return Wt.createElement("span", {
             className: Kt()(e, Object(Vt.a)({}, "".concat(e, "-active"), t && s <= r && r <= u)),
             style: Object(Ct.a)(Object(Ct.a)({}, c), n),
             onMouseDown: function(t) {
                 t.stopPropagation()
             },
             onClick: function() {
                 o(r)
             }
         }, a)
     }
 
-    function le(t) {
+    function de(t) {
         var e = t.prefixCls,
             n = t.marks,
             a = t.onClick,
             r = "".concat(e, "-mark");
         return n.length ? Wt.createElement("div", {
             className: r
         }, n.map(function(t) {
             var e = t.value,
                 n = t.style,
                 t = t.label;
-            return Wt.createElement(ie, {
+            return Wt.createElement(ue, {
                 key: e,
                 prefixCls: r,
                 style: n,
                 value: e,
                 onClick: a
             }, t)
         })) : null
     }
 
-    function ce(t) {
+    function pe(t) {
         var e = t.prefixCls,
             n = t.value,
             a = t.style,
             t = t.activeStyle,
-            r = Wt.useContext(Zt),
+            r = Wt.useContext(Qt),
             o = r.min,
             i = r.max,
             l = r.direction,
             c = r.included,
             s = r.includedStart,
             r = r.includedEnd,
             e = "".concat(e, "-dot"),
             c = c && s <= n && n <= r,
-            s = Object(Ct.a)(Object(Ct.a)({}, Ht(l, n, o, i)), "function" == typeof a ? a(n) : a);
+            s = Object(Ct.a)(Object(Ct.a)({}, ee(l, n, o, i)), "function" == typeof a ? a(n) : a);
         return c && (s = Object(Ct.a)(Object(Ct.a)({}, s), "function" == typeof t ? t(n) : t)), Wt.createElement("span", {
             className: Kt()(e, Object(Vt.a)({}, "".concat(e, "-active"), c)),
             style: s
         })
     }
 
-    function se(t) {
+    function fe(t) {
         var e = t.prefixCls,
             n = t.marks,
             a = t.dots,
             r = t.style,
             o = t.activeStyle,
-            t = Wt.useContext(Zt),
+            t = Wt.useContext(Qt),
             i = t.min,
             l = t.max,
             c = t.step,
             t = Wt.useMemo(function() {
                 var e = new Set;
                 if (n.forEach(function(t) {
                         e.add(t.value)
                     }), a && null !== c)
                     for (var t = i; t <= l;) e.add(t), t += c;
                 return Array.from(e)
             }, [i, l, c, a, n]);
         return Wt.createElement("div", {
             className: "".concat(e, "-step")
         }, t.map(function(t) {
-            return Wt.createElement(ce, {
+            return Wt.createElement(pe, {
                 prefixCls: e,
                 key: t,
                 value: t,
                 style: r,
                 activeStyle: o
             })
         }))
     }
 
-    function ue(t) {
+    function he(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.railStyle,
             o = t.key,
             i = t.value,
             l = t.defaultValue,
@@ -105483,15 +105565,15 @@
             u ? i || x({
                 value: l || [d, p],
                 defaultValue: l || [d, p]
             }) : i || 0 === i || x({
                 value: l || 0 === l ? l : p,
                 defaultValue: l || 0 === l ? l : p
             })
-        }, []), H.a.createElement(me, {
+        }, []), H.a.createElement(ye, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             railStyle: r,
             key: o,
             value: i,
             defaultValue: l,
@@ -105518,16 +105600,16 @@
             },
             persistence: _,
             persisted_props: O,
             persistence_type: t,
             "data-dash-is-loading": y && y.is_loading || void 0
         })
     }
-    var de = e(19),
-        pe = Wt.forwardRef(function(t, R) {
+    var me = e(19),
+        ge = Wt.forwardRef(function(t, R) {
             var d, p, f, h, I, b, o, m, N, e = t.prefixCls,
                 e = void 0 === e ? "rc-slider" : e,
                 Y = t.className,
                 B = t.style,
                 F = t.disabled,
                 i = void 0 !== F && F,
                 H = t.autoFocus,
@@ -105654,15 +105736,15 @@
                         value: r[n],
                         values: r
                     }
                 }]),
                 _ = Object(Gt.a)(g, 2),
                 st = _[0],
                 ut = _[1],
-                g = Object($t.a)(r, {
+                g = Object(Zt.a)(r, {
                     value: n
                 }),
                 _ = Object(Gt.a)(g, 2),
                 E = _[0],
                 dt = _[1],
                 C = Wt.useMemo(function() {
                     var t = null == E ? [] : Array.isArray(E) ? E : [E],
@@ -105714,15 +105796,15 @@
             function S(t) {
                 return l ? t : t[0]
             }
 
             function gt(t) {
                 t = Object(Ut.a)(t).sort(function(t, e) {
                     return t - e
-                }), U && !Xt()(t, pt.current) && U(S(t)), dt(t)
+                }), U && !$t()(t, pt.current) && U(S(t)), dt(t)
             }
 
             function bt(n) {
                 var a, r, t;
                 i || (a = 0, r = j - k, C.forEach(function(t, e) {
                     t = Math.abs(n - t);
                     t <= r && (r = t, a = e)
@@ -105761,15 +105843,15 @@
                         return t === n[e]
                     }) ? P : L
                 }, [L, P]), [Ct, r, _, function(t, l) {
                     t.stopPropagation();
 
                     function e(t) {
                         t.preventDefault();
-                        var e, n = (t = ae(t)).pageX,
+                        var e, n = (t = le(t)).pageX,
                             t = t.pageY,
                             a = n - c,
                             r = t - s,
                             o = (n = yt.current.getBoundingClientRect()).width,
                             i = n.height;
                         switch (xt) {
                             case "btt":
@@ -105787,15 +105869,15 @@
                         Dt.current(l, e)
                     }
 
                     function n(t) {
                         t.preventDefault(), document.removeEventListener("mouseup", n), document.removeEventListener("mousemove", e), document.removeEventListener("touchend", n), document.removeEventListener("touchmove", e), T.current = null, z.current = null, St(-1), jt()
                     }
                     var a = L[l],
-                        a = (St(l), Et(a), Pt(L), ae(t)),
+                        a = (St(l), Et(a), Pt(L), le(t)),
                         c = a.pageX,
                         s = a.pageY;
                     document.addEventListener("mouseup", n), document.addEventListener("mousemove", e), document.addEventListener("touchend", n), document.addEventListener("touchmove", e), T.current = e, z.current = n
                 }]),
                 r = Object(Gt.a)(n, 4),
                 _ = r[0],
                 At = r[1],
@@ -105854,15 +105936,15 @@
                         range: l,
                         tabIndex: rt,
                         ariaLabelForHandle: ot,
                         ariaLabelledByForHandle: it,
                         ariaValueTextFormatterForHandle: lt
                     }
                 }, [k, j, ct, i, M, X, Ft, Ht, l, rt, ot, it, lt]));
-            return Wt.createElement(Zt.Provider, {
+            return Wt.createElement(Qt.Provider, {
                 value: n
             }, Wt.createElement("div", {
                 ref: w,
                 className: Kt()(e, Y, (r = {}, Object(Vt.a)(r, "".concat(e, "-disabled"), i), Object(Vt.a)(r, "".concat(e, "-vertical"), x), Object(Vt.a)(r, "".concat(e, "-horizontal"), !x), Object(Vt.a)(r, "".concat(e, "-with-marks"), t.length), r)),
                 style: B,
                 onMouseDown: function(t) {
                     t.preventDefault();
@@ -105889,64 +105971,64 @@
                             e = (s - o) / a
                     }
                     bt(st(k + e * (j - k)))
                 }
             }, Wt.createElement("div", {
                 className: "".concat(e, "-rail"),
                 style: J
-            }), Wt.createElement(oe, {
+            }), Wt.createElement(se, {
                 prefixCls: e,
                 style: $,
                 values: A,
                 startPoint: v,
                 onStartMove: g ? vt : null
-            }), Wt.createElement(se, {
+            }), Wt.createElement(fe, {
                 prefixCls: e,
                 marks: t,
                 dots: nt,
                 style: Q,
                 activeStyle: tt
-            }), Wt.createElement(ne, {
+            }), Wt.createElement(ie, {
                 ref: O,
                 prefixCls: e,
                 style: Z,
                 values: Rt,
                 draggingIndex: _,
                 onStartMove: vt,
                 onOffsetChange: function(t, e) {
                     i || (t = ut(C, t, e), null != s && s(S(C)), gt(t.values), null != u && u(S(t.values)), zt(t.value))
                 },
                 onFocus: F,
                 onBlur: W,
                 handleRender: at
-            }), Wt.createElement(le, {
+            }), Wt.createElement(de, {
                 prefixCls: e,
                 marks: t,
                 onClick: bt
             })))
         }),
-        fe = e(37),
-        he = Wt.forwardRef(function(t, e) {
+        be = e(37),
+        ve = Wt.forwardRef(function(t, e) {
             var n = t.open,
                 a = Object(Wt.useRef)(null),
                 r = Object(Wt.useRef)(null);
 
             function o() {
-                st.a.cancel(r.current), r.current = null
+                ft.a.cancel(r.current), r.current = null
             }
             return Wt.useEffect(function() {
-                return n ? r.current = Object(st.a)(function() {
+                return n ? r.current = Object(ft.a)(function() {
                     var t;
                     null != (t = a.current) && t.forcePopupAlign(), r.current = null
                 }) : o(), o
             }, [n, t.title]), Wt.createElement(D.a, Object(Et.a)({
-                ref: Object(fe.a)(a, e)
+                ref: Object(be.a)(a, e)
             }, t))
         }),
-        me = Wt.forwardRef(function(d, t) {
+        ye = Wt.forwardRef(function(d, t) {
             function p(e, n) {
                 a(function(t) {
                     return Object(Et.a)(Object(Et.a)({}, t), Object(Vt.a)({}, e, n))
                 })
             }
             var e = Wt.useContext(q.b),
                 f = e.getPrefixCls,
@@ -105970,15 +106052,15 @@
                 e = Kt()(r, Object(Vt.a)({}, "".concat(b, "-rtl"), "rtl" === h)),
                 r = ("rtl" !== h || o.vertical || (o.reverse = !o.reverse), Wt.useMemo(function() {
                     return n ? "object" === Object(qt.a)(n) ? [!0, n.draggableTrack] : [!0, !1] : [!1]
                 }, [n])),
                 r = Object(Gt.a)(r, 2),
                 i = r[0],
                 r = r[1];
-            return Wt.createElement(pe, Object(Et.a)({}, o, {
+            return Wt.createElement(ge, Object(Et.a)({}, o, {
                 step: o.step,
                 range: i,
                 draggableTrack: r,
                 className: e,
                 ref: t,
                 prefixCls: b,
                 handleRender: function(t, e) {
@@ -106008,28 +106090,28 @@
                                 return p(n, !0)
                             },
                             onMouseLeave: function() {
                                 return p(n, !1)
                             }
                         }),
                         u = f("tooltip", u);
-                    return Wt.createElement(he, {
+                    return Wt.createElement(ve, {
                         prefixCls: u,
                         title: l ? l(e.value) : "",
                         open: o,
                         placement: c || (i ? "rtl" === h ? "left" : "right" : "top"),
                         transitionName: "".concat(r, "-zoom-down"),
                         key: n,
                         overlayClassName: "".concat(b, "-tooltip"),
                         getPopupContainer: s || m
                     }, Wt.cloneElement(t, a))
                 }
             }))
         }),
-        ge = (ue.propTypes = {
+        xe = (he.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             railStyle: n.a.object,
             key: n.a.string,
             vertical: n.a.bool,
             range: n.a.bool,
@@ -106049,104 +106131,103 @@
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func,
             persistence: n.a.oneOfType([n.a.bool, n.a.string, n.a.number]),
             persisted_props: n.a.arrayOf(n.a.oneOf(["value"])),
             persistence_type: n.a.oneOf(["local", "session", "memory"])
-        }, ue.defaultProps = {
+        }, he.defaultProps = {
             vertical: !1,
             range: !1,
             min: 0,
             max: 100,
             step: 1,
             tooltipPrefix: "",
             tooltipSuffix: "",
             disabled: !1,
             popupContainer: "body",
             persisted_props: ["value"],
             persistence_type: "local"
-        }, ue),
-        be = e(100),
-        ve = e(32),
-        ye = e(63),
-        xe = e(74),
-        _e = e(48),
-        Oe = e(101),
-        we = e(112),
-        ke = e(147),
-        je = e(29),
-        Me = e(273),
-        l = e(57),
-        Ee = e(284),
-        Ce = e(156),
-        Se = Wt.memo(function(t) {
+        }, he),
+        _e = e(100),
+        Oe = e(32),
+        we = e(63),
+        ke = e(74),
+        je = e(48),
+        Me = e(101),
+        Ee = e(112),
+        Ce = e(29),
+        Se = e(273),
+        l = e(58),
+        Le = e(284),
+        Pe = e(157),
+        De = Wt.memo(function(t) {
             var a, e = t.renderedText,
                 r = t.renderedEl,
                 o = t.item,
                 i = t.checked,
                 l = t.disabled,
                 c = t.prefixCls,
                 s = t.onClick,
                 u = t.onRemove,
                 d = t.showRemove,
                 p = Kt()((t = {}, Object(Vt.a)(t, "".concat(c, "-content-item"), !0), Object(Vt.a)(t, "".concat(c, "-content-item-disabled"), l || o.disabled), Object(Vt.a)(t, "".concat(c, "-content-item-checked"), i), t));
-            return "string" != typeof e && "number" != typeof e || (a = String(e)), Wt.createElement(ye.a, {
+            return "string" != typeof e && "number" != typeof e || (a = String(e)), Wt.createElement(we.a, {
                 componentName: "Transfer",
-                defaultLocale: xe.a.Transfer
+                defaultLocale: ke.a.Transfer
             }, function(t) {
                 var e = {
                         className: p,
                         title: a
                     },
                     n = Wt.createElement("span", {
                         className: "".concat(c, "-content-item-text")
                     }, r);
-                return d ? Wt.createElement("li", Object(Et.a)({}, e), n, Wt.createElement(Ce.a, {
+                return d ? Wt.createElement("li", Object(Et.a)({}, e), n, Wt.createElement(Pe.a, {
                     disabled: l || o.disabled,
                     className: "".concat(c, "-content-item-remove"),
                     "aria-label": t.remove,
                     onClick: function() {
                         null != u && u(o)
                     }
-                }, Wt.createElement(Ee.a, null))) : (e.onClick = l || o.disabled ? void 0 : function() {
+                }, Wt.createElement(Le.a, null))) : (e.onClick = l || o.disabled ? void 0 : function() {
                     return s(o)
-                }, Wt.createElement("li", Object(Et.a)({}, e), Wt.createElement(we.a, {
+                }, Wt.createElement("li", Object(Et.a)({}, e), Wt.createElement(Ee.a, {
                     className: "".concat(c, "-checkbox"),
                     checked: i,
                     disabled: l || o.disabled
                 }), n))
             })
         }),
-        Le = Object(l.a)("handleFilter", "handleClear", "checkedKeys");
+        Te = Object(l.a)("handleFilter", "handleClear", "checkedKeys");
 
-    function Pe(t) {
+    function ze(t) {
         var e;
         return t ? (e = {
             pageSize: 10,
             simple: !0,
             showSizeChanger: !1,
             showLessItems: !1
         }, "object" === Object(qt.a)(t) ? Object(Et.a)(Object(Et.a)({}, e), t) : e) : null
     }
-    c = Wt.Component, Object(r.a)(Re, c), De = Object(o.a)(Re), Object(a.a)(Re, [{
+    c = Wt.Component, Object(r.a)(Ye, c), Ae = Object(o.a)(Ye), Object(a.a)(Ye, [{
         key: "render",
         value: function() {
             var o = this,
                 t = this.state.current,
                 e = this.props,
                 i = e.prefixCls,
                 n = e.onScroll,
                 a = e.filteredRenderItems,
                 l = e.selectedKeys,
                 c = e.disabled,
                 s = e.showRemove,
-                e = Pe(e.pagination),
+                e = ze(e.pagination),
                 r = null;
-            return e && (r = Wt.createElement(Me.a, {
+            return e && (r = Wt.createElement(Se.a, {
                 simple: e.simple,
                 showSizeChanger: e.showSizeChanger,
                 showLessItems: e.showLessItems,
                 size: "small",
                 disabled: c,
                 className: "".concat(i, "-pagination"),
                 total: a.length,
@@ -106158,15 +106239,15 @@
                 onScroll: n
             }, this.getItems().map(function(t) {
                 var e = t.renderedEl,
                     n = t.renderedText,
                     t = t.item,
                     a = t.disabled,
                     r = l.includes(t.key);
-                return Wt.createElement(Se, {
+                return Wt.createElement(De, {
                     disabled: c || a,
                     key: t.key,
                     item: t,
                     renderedText: n,
                     renderedEl: e,
                     checked: r,
                     prefixCls: i,
@@ -106178,31 +106259,31 @@
         }
     }], [{
         key: "getDerivedStateFromProps",
         value: function(t, e) {
             var n = t.filteredRenderItems,
                 t = t.pagination,
                 e = e.current,
-                t = Pe(t);
+                t = ze(t);
             if (t) {
                 n = Math.ceil(n.length / t.pageSize);
                 if (n < e) return {
                     current: n
                 }
             }
             return null
         }
     }]);
-    var De, Te = Re,
-        ze = e(127),
-        Ae = e(198);
+    var Ae, Re = Ye,
+        Ie = e(127),
+        Ne = e(198);
 
-    function Re() {
+    function Ye() {
         var r;
-        return Object(i.a)(this, Re), (r = De.apply(this, arguments)).state = {
+        return Object(i.a)(this, Ye), (r = Ae.apply(this, arguments)).state = {
             current: 1
         }, r.onItemSelect = function(t) {
             var e = r.props,
                 n = e.onItemSelect,
                 e = e.selectedKeys.includes(t.key);
             n(t.key, !e)
         }, r.onItemRemove = function(t) {
@@ -106213,51 +106294,51 @@
                 current: t
             })
         }, r.getItems = function() {
             var t = r.state.current,
                 e = r.props,
                 n = e.pagination,
                 e = e.filteredRenderItems,
-                n = Pe(n),
+                n = ze(n),
                 a = e;
             return a = n ? e.slice((t - 1) * n.pageSize, t * n.pageSize) : a
         }, r
     }
 
-    function Ie(t) {
+    function Be(t) {
         var e = t.placeholder,
             e = void 0 === e ? "" : e,
             n = t.value,
             a = t.prefixCls,
             r = t.disabled,
             o = t.onChange,
             i = t.handleClear,
             t = Wt.useCallback(function(t) {
                 null != o && o(t), "" !== t.target.value || null != i && i()
             }, [o]);
-        return Wt.createElement(Ae.a, {
+        return Wt.createElement(Ne.a, {
             placeholder: e,
             className: a,
             value: n,
             onChange: t,
             disabled: r,
             allowClear: !0,
-            prefix: Wt.createElement(ze.a, null)
+            prefix: Wt.createElement(Ie.a, null)
         })
     }
 
-    function Ne(t) {
+    function Fe(t) {
         return t.filter(function(t) {
             return !t.disabled
         }).map(function(t) {
             return t.key
         })
     }
 
-    function Ye(t) {
+    function He(t) {
         var e = t.disabled,
             n = t.moveToLeft,
             a = t.moveToRight,
             r = void 0 === (r = t.leftArrowText) ? "" : r,
             o = void 0 === (o = t.rightArrowText) ? "" : o,
             i = t.leftActive,
             l = t.rightActive,
@@ -106269,24 +106350,24 @@
             className: c,
             style: s
         }, Wt.createElement(z.a, {
             type: "primary",
             size: "small",
             disabled: e || !l,
             onClick: a,
-            icon: "rtl" !== u ? Wt.createElement(Ve.a, null) : Wt.createElement(We.a, null)
+            icon: "rtl" !== u ? Wt.createElement(Ge.a, null) : Wt.createElement(Ue.a, null)
         }, o), !t && Wt.createElement(z.a, {
             type: "primary",
             size: "small",
             disabled: e || !i,
             onClick: n,
-            icon: "rtl" !== u ? Wt.createElement(We.a, null) : Wt.createElement(Ve.a, null)
+            icon: "rtl" !== u ? Wt.createElement(Ue.a, null) : Wt.createElement(Ge.a, null)
         }, r))
     }
-    c = Wt.PureComponent, Object(r.a)(Ue, c), Fe = Object(o.a)(Ue), Object(a.a)(Ue, [{
+    c = Wt.PureComponent, Object(r.a)(Xe, c), Ve = Object(o.a)(Xe), Object(a.a)(Xe, [{
         key: "componentWillUnmount",
         value: function() {
             clearTimeout(this.triggerScrollTimer)
         }
     }, {
         key: "getCheckStatus",
         value: function(t) {
@@ -106312,22 +106393,22 @@
             }
         }
     }, {
         key: "getListBody",
         value: function(t, e, n, a, r, o, i, l, c, s) {
             e = c ? Wt.createElement("div", {
                 className: "".concat(t, "-body-search-wrapper")
-            }, Wt.createElement(Ie, {
+            }, Wt.createElement(Be, {
                 prefixCls: "".concat(t, "-search"),
                 onChange: this.handleFilter,
                 handleClear: this.handleClear,
                 placeholder: e,
                 value: n,
                 disabled: s
-            })) : null, n = this.renderListBody(l, Object(Et.a)(Object(Et.a)({}, Object(ct.a)(this.props, Le)), {
+            })) : null, n = this.renderListBody(l, Object(Et.a)(Object(Et.a)({}, Object(pt.a)(this.props, Te)), {
                 filteredItems: a,
                 filteredRenderItems: o,
                 selectedKeys: i
             })), s = n.bodyContent, o = n.customize ? Wt.createElement("div", {
                 className: "".concat(t, "-body-customize-wrapper")
             }, s) : a.length ? s : Wt.createElement("div", {
                 className: "".concat(t, "-body-not-found")
@@ -106341,15 +106422,15 @@
         value: function(t) {
             var e = t.filteredItems,
                 n = t.onItemSelectAll,
                 a = t.disabled,
                 t = t.prefixCls,
                 r = this.getCheckStatus(e),
                 o = "all" === r;
-            return Wt.createElement(we.a, {
+            return Wt.createElement(Ee.a, {
                 disabled: a,
                 checked: o,
                 indeterminate: "part" === r,
                 className: "".concat(t, "-checkbox"),
                 onChange: function() {
                     n(e.filter(function(t) {
                         return !t.disabled
@@ -106407,82 +106488,82 @@
                     onItemSelectAll: y,
                     disabled: l,
                     prefixCls: n
                 }),
                 a = O ? [w ? {
                     key: "removeCurrent",
                     onClick: function() {
-                        var t = Ne(((null == (t = r.defaultListBodyRef.current) ? void 0 : t.getItems()) || []).map(function(t) {
+                        var t = Fe(((null == (t = r.defaultListBodyRef.current) ? void 0 : t.getItems()) || []).map(function(t) {
                             return t.item
                         }));
                         null != x && x(t)
                     },
                     label: b
                 } : null, {
                     key: "removeAll",
                     onClick: function() {
-                        null != x && x(Ne(k))
+                        null != x && x(Fe(k))
                     },
                     label: g
                 }].filter(function(t) {
                     return t
                 }) : [{
                     key: "selectAll",
                     onClick: function() {
-                        var t = Ne(k);
+                        var t = Fe(k);
                         y(t, t.length !== i.length)
                     },
                     label: f
                 }, w ? {
                     key: "selectCurrent",
                     onClick: function() {
                         var t = (null == (t = r.defaultListBodyRef.current) ? void 0 : t.getItems()) || [];
-                        y(Ne(t.map(function(t) {
+                        y(Fe(t.map(function(t) {
                             return t.item
                         })), !0)
                     },
                     label: h
                 } : null, {
                     key: "selectInvert",
                     onClick: function() {
-                        var t = Ne(w ? ((null == (t = r.defaultListBodyRef.current) ? void 0 : t.getItems()) || []).map(function(t) {
+                        var t = Fe(w ? ((null == (t = r.defaultListBodyRef.current) ? void 0 : t.getItems()) || []).map(function(t) {
                                 return t.item
                             }) : k),
                             e = new Set(i),
                             n = [],
                             a = [];
                         t.forEach(function(t) {
                             (e.has(t) ? a : n).push(t)
                         }), y(n, !0), y(a, !1)
                     },
                     label: m
                 }],
-                v = Wt.createElement(ke.a, {
+                v = Wt.createElement(R.a, {
                     className: "".concat(n, "-header-dropdown"),
                     menu: {
                         items: a
                     },
                     disabled: l
-                }, Wt.createElement(Oe.a, null));
+                }, Wt.createElement(Me.a, null));
             return Wt.createElement("div", {
                 className: e,
                 style: u
             }, Wt.createElement("div", {
                 className: "".concat(n, "-header")
             }, _ ? Wt.createElement(Wt.Fragment, null, p, v) : null, Wt.createElement("span", {
                 className: "".concat(n, "-header-selected")
             }, this.getSelectAllLabel(i.length, k.length)), Wt.createElement("span", {
                 className: "".concat(n, "-header-title")
             }, o)), d, t)
         }
     }]);
-    var Be, Fe, He = Ue,
-        We = e(102),
-        Ve = e(88),
-        c = (c = Wt.Component, Object(r.a)(Ke, c), Be = Object(o.a)(Ke), Object(a.a)(Ke, [{
+    var We, Ve, Ke = Xe,
+        Ue = e(102),
+        Ge = e(88),
+        c = (c = Wt.Component, Object(r.a)(qe, c), We = Object(o.a)(qe), Object(a.a)(qe, [{
             key: "getTitles",
             value: function(t) {
                 var e;
                 return null != (e = null != (e = this.props.titles) ? e : t.titles) ? e : []
             }
         }, {
             key: "handleSelectChange",
@@ -106514,23 +106595,23 @@
                     rightDataSource: o
                 }
             }
         }, {
             key: "render",
             value: function() {
                 var S = this;
-                return Wt.createElement(ye.a, {
+                return Wt.createElement(we.a, {
                     componentName: "Transfer",
-                    defaultLocale: xe.a.Transfer
+                    defaultLocale: ke.a.Transfer
                 }, function(C) {
                     return Wt.createElement(q.a, null, function(t) {
                         var j = t.getPrefixCls,
                             M = t.renderEmpty,
                             E = t.direction;
-                        return Wt.createElement(ve.b.Consumer, null, function(t) {
+                        return Wt.createElement(Oe.b.Consumer, null, function(t) {
                             var e = t.hasFeedback,
                                 t = t.status,
                                 n = S.props,
                                 a = n.prefixCls,
                                 r = n.className,
                                 o = n.disabled,
                                 i = n.operations,
@@ -106546,32 +106627,32 @@
                                 f = n.render,
                                 h = n.children,
                                 m = n.showSelectAll,
                                 g = n.oneWay,
                                 b = n.pagination,
                                 n = n.status,
                                 a = j("transfer", a),
-                                v = S.getLocale(C, M || be.a),
+                                v = S.getLocale(C, M || _e.a),
                                 y = S.state,
                                 x = y.sourceSelectedKeys,
                                 y = y.targetSelectedKeys,
-                                t = Object(_e.a)(t, n),
+                                t = Object(je.a)(t, n),
                                 n = !h && b,
                                 b = S.separateDataSource(),
                                 _ = b.leftDataSource,
                                 b = b.rightDataSource,
                                 O = 0 < y.length,
                                 w = 0 < x.length,
-                                k = Kt()(a, (k = {}, Object(Vt.a)(k, "".concat(a, "-disabled"), o), Object(Vt.a)(k, "".concat(a, "-customize-list"), !!h), Object(Vt.a)(k, "".concat(a, "-rtl"), "rtl" === E), k), Object(_e.b)(a, t, e), r),
+                                k = Kt()(a, (k = {}, Object(Vt.a)(k, "".concat(a, "-disabled"), o), Object(Vt.a)(k, "".concat(a, "-customize-list"), !!h), Object(Vt.a)(k, "".concat(a, "-rtl"), "rtl" === E), k), Object(je.b)(a, t, e), r),
                                 t = S.getTitles(v),
                                 e = S.props.selectAllLabels || [];
                             return Wt.createElement("div", {
                                 className: k,
                                 style: s
-                            }, Wt.createElement(He, Object(Et.a)({
+                            }, Wt.createElement(Ke, Object(Et.a)({
                                 prefixCls: "".concat(a, "-list"),
                                 titleText: null == t ? void 0 : t[0],
                                 dataSource: _,
                                 filterOption: p,
                                 style: S.handleListStyle(u, "left"),
                                 checkedKeys: x,
                                 handleFilter: S.handleLeftFilter,
@@ -106584,27 +106665,27 @@
                                 footer: c,
                                 onScroll: S.handleLeftScroll,
                                 disabled: o,
                                 direction: "rtl" === E ? "right" : "left",
                                 showSelectAll: m,
                                 selectAllLabel: e[0],
                                 pagination: n
-                            }, v)), Wt.createElement(Ye, {
+                            }, v)), Wt.createElement(He, {
                                 className: "".concat(a, "-operation"),
                                 rightActive: w,
                                 rightArrowText: i[0],
                                 moveToRight: S.moveToRight,
                                 leftActive: O,
                                 leftArrowText: i[1],
                                 moveToLeft: S.moveToLeft,
                                 style: d,
                                 disabled: o,
                                 direction: E,
                                 oneWay: g
-                            }), Wt.createElement(He, Object(Et.a)({
+                            }), Wt.createElement(Ke, Object(Et.a)({
                                 prefixCls: "".concat(a, "-list"),
                                 titleText: null == t ? void 0 : t[1],
                                 dataSource: b,
                                 filterOption: p,
                                 style: S.handleListStyle(u, "right"),
                                 checkedKeys: y,
                                 handleFilter: S.handleRightFilter,
@@ -106638,18 +106719,18 @@
                         return !e.includes(t)
                     }),
                     targetSelectedKeys: n.filter(function(t) {
                         return e.includes(t)
                     })
                 }) : null
             }
-        }]), Ke);
+        }]), qe);
 
-    function Ke(t) {
-        Object(i.a)(this, Ke), (l = Be.call(this, t)).separatedDataSource = null, l.setStateKeys = function(t, e) {
+    function qe(t) {
+        Object(i.a)(this, qe), (l = We.call(this, t)).separatedDataSource = null, l.setStateKeys = function(t, e) {
             "left" === t ? l.setState(function(t) {
                 t = t.sourceSelectedKeys;
                 return {
                     sourceSelectedKeys: "function" == typeof e ? e(t || []) : e
                 }
             }) : l.setState(function(t) {
                 t = t.targetSelectedKeys;
@@ -106753,17 +106834,17 @@
             }),
             targetSelectedKeys: e.filter(function(t) {
                 return n.includes(t)
             })
         }, l
     }
 
-    function Ue(t) {
+    function Xe(t) {
         var o;
-        return Object(i.a)(this, Ue), (o = Fe.call(this, t)).defaultListBodyRef = Wt.createRef(), o.handleFilter = function(t) {
+        return Object(i.a)(this, Xe), (o = Ve.call(this, t)).defaultListBodyRef = Wt.createRef(), o.handleFilter = function(t) {
             var e = o.props.handleFilter,
                 n = t.target.value;
             o.setState({
                 filterValue: n
             }), e(t)
         }, o.handleClear = function() {
             var t = o.props.handleClear;
@@ -106775,24 +106856,24 @@
                 a = o.props.filterOption;
             return a ? a(n, e) : t.includes(n)
         }, o.renderListBody = function(t, e) {
             var t = t ? t(e) : null,
                 n = !!t;
             return {
                 customize: n,
-                bodyContent: t = n ? t : Wt.createElement(Te, Object(Et.a)({
+                bodyContent: t = n ? t : Wt.createElement(Re, Object(Et.a)({
                     ref: o.defaultListBodyRef
                 }, e))
             }
         }, o.renderItem = function(t) {
             var e = o.props.render,
                 e = (void 0 === e ? function() {
                     return null
                 } : e)(t),
-                n = !(!(n = e) || Object(je.c)(n) || "[object Object]" !== Object.prototype.toString.call(n));
+                n = !(!(n = e) || Object(Ce.c)(n) || "[object Object]" !== Object.prototype.toString.call(n));
             return {
                 renderedText: n ? e.value : e,
                 renderedEl: n ? e.label : e,
                 item: t
             }
         }, o.getSelectAllLabel = function(t, e) {
             var n = o.props,
@@ -106803,17 +106884,17 @@
                 selectedCount: t,
                 totalCount: e
             }) : n : (n = 1 < e ? a : r, Wt.createElement(Wt.Fragment, null, (0 < t ? "".concat(t, "/") : "") + e, " ", n))
         }, o.state = {
             filterValue: ""
         }, o
     }
-    c.List = He, c.Operation = Ye, c.Search = Ie;
+    c.List = Ke, c.Operation = He, c.Search = Be;
 
-    function Ge(t) {
+    function $e(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.locale,
             i = t.setProps,
             l = t.dataSource,
@@ -106831,15 +106912,15 @@
             y = t.persistence_type,
             t = t.loading_state,
             x = Object(Wt.useContext)(G.a),
             o = x && x.locale || o,
             f = f || K.a.AntdTransfer[o].titles;
         return H.a.createElement(W.a, {
             locale: K.b.get(o)
-        }, H.a.createElement(qe, {
+        }, H.a.createElement(Ze, {
             id: e,
             style: a,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             key: r,
             dataSource: l,
             targetKeys: m,
             onChange: function(t, e, n) {
@@ -106866,16 +106947,16 @@
                 overflowX: "auto",
                 height: c,
                 width: "100%"
             },
             "data-dash-is-loading": t && t.is_loading || void 0
         }))
     }
-    var qe = c,
-        Xe = (Ge.propTypes = {
+    var Ze = c,
+        Je = ($e.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             locale: n.a.oneOf(["zh-cn", "en-us"]),
             dataSource: n.a.arrayOf(n.a.exact({
                 key: n.a.oneOfType([n.a.string, n.a.number]),
@@ -106899,61 +106980,61 @@
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             persistence: n.a.oneOfType([n.a.bool, n.a.string, n.a.number]),
             persisted_props: n.a.arrayOf(n.a.oneOf(["targetKeys"])),
             persistence_type: n.a.oneOf(["local", "session", "memory"])
-        }, Ge.defaultProps = {
+        }, $e.defaultProps = {
             targetKeys: [],
             pagination: !1,
             operations: ["", ""],
             showSearch: !1,
             showSelectAll: !0,
             disabled: !1,
             persisted_props: ["targetKeys"],
             persistence_type: "local",
             locale: "zh-cn"
-        }, Ge),
-        $e = e(145),
-        Ze = e(76),
+        }, $e),
+        Qe = e(145),
+        tn = e(76),
         s = e(20),
-        Je = ["className", "prefixCls", "style", "active", "status", "iconPrefix", "icon", "wrapperStyle", "stepNumber", "disabled", "description", "title", "subTitle", "progressDot", "stepIcon", "tailContent", "icons", "stepIndex", "onStepClick", "onClick"];
+        en = ["className", "prefixCls", "style", "active", "status", "iconPrefix", "icon", "wrapperStyle", "stepNumber", "disabled", "description", "title", "subTitle", "progressDot", "stepIcon", "tailContent", "icons", "stepIndex", "onStepClick", "onClick"];
 
-    function Qe(t) {
+    function nn(t) {
         return "string" == typeof t
     }
-    c = Wt.Component, Object(r.a)(on, c), en = Object(o.a)(on), Object(a.a)(on, [{
+    c = Wt.Component, Object(r.a)(sn, c), rn = Object(o.a)(sn), Object(a.a)(sn, [{
         key: "renderIconNode",
         value: function() {
             var t = this.props,
                 e = t.prefixCls,
                 n = t.progressDot,
                 a = t.stepIcon,
                 r = t.stepNumber,
                 o = t.status,
                 i = t.title,
                 l = t.description,
                 c = t.icon,
                 s = t.iconPrefix,
                 t = t.icons,
-                s = Kt()("".concat(e, "-icon"), "".concat(s, "icon"), (u = {}, Object(Vt.a)(u, "".concat(s, "icon-").concat(c), c && Qe(c)), Object(Vt.a)(u, "".concat(s, "icon-check"), !c && "finish" === o && (t && !t.finish || !t)), Object(Vt.a)(u, "".concat(s, "icon-cross"), !c && "error" === o && (t && !t.error || !t)), u)),
+                s = Kt()("".concat(e, "-icon"), "".concat(s, "icon"), (u = {}, Object(Vt.a)(u, "".concat(s, "icon-").concat(c), c && nn(c)), Object(Vt.a)(u, "".concat(s, "icon-check"), !c && "finish" === o && (t && !t.finish || !t)), Object(Vt.a)(u, "".concat(s, "icon-cross"), !c && "error" === o && (t && !t.error || !t)), u)),
                 u = Wt.createElement("span", {
                     className: "".concat(e, "-icon-dot")
                 }),
                 n = n ? "function" == typeof n ? Wt.createElement("span", {
                     className: "".concat(e, "-icon")
                 }, n(u, {
                     index: r - 1,
                     status: o,
                     title: i,
                     description: l
                 })) : Wt.createElement("span", {
                     className: "".concat(e, "-icon")
-                }, u) : c && !Qe(c) ? Wt.createElement("span", {
+                }, u) : c && !nn(c) ? Wt.createElement("span", {
                     className: "".concat(e, "-icon")
                 }, c) : t && t.finish && "finish" === o ? Wt.createElement("span", {
                     className: "".concat(e, "-icon")
                 }, t.finish) : t && t.error && "error" === o ? Wt.createElement("span", {
                     className: "".concat(e, "-icon")
                 }, t.error) : c || "finish" === o || "error" === o ? Wt.createElement("span", {
                     className: s
@@ -106982,15 +107063,15 @@
                 l = (t.wrapperStyle, t.stepNumber, t.disabled),
                 c = t.description,
                 s = t.title,
                 u = t.subTitle,
                 d = (t.progressDot, t.stepIcon, t.tailContent),
                 p = (t.icons, t.stepIndex, t.onStepClick),
                 f = t.onClick,
-                t = Object(Bt.a)(t, Je),
+                t = Object(Jt.a)(t, en),
                 e = Kt()("".concat(n, "-item"), "".concat(n, "-item-").concat(o), e, (o = {}, Object(Vt.a)(o, "".concat(n, "-item-custom"), i), Object(Vt.a)(o, "".concat(n, "-item-active"), r), Object(Vt.a)(o, "".concat(n, "-item-disabled"), !0 === l), o)),
                 i = Object(Ct.a)({}, a),
                 r = {};
             return p && !l && (r.role = "button", r.tabIndex = 0, r.onClick = this.onClick), Wt.createElement("div", Object(Et.a)({}, t, {
                 className: e,
                 style: i
             }), Wt.createElement("div", Object(Et.a)({
@@ -107009,17 +107090,17 @@
                 title: "string" == typeof u ? u : void 0,
                 className: "".concat(n, "-item-subtitle")
             }, u)), c && Wt.createElement("div", {
                 className: "".concat(n, "-item-description")
             }, c))))
         }
     }]);
-    var tn, en, nn = on,
-        an = ["prefixCls", "style", "className", "children", "direction", "type", "labelPlacement", "iconPrefix", "status", "size", "current", "progressDot", "stepIcon", "initial", "icons", "onChange", "items"],
-        c = (c = H.a.Component, Object(r.a)(rn, c), tn = Object(o.a)(rn), Object(a.a)(rn, [{
+    var an, rn, on = sn,
+        ln = ["prefixCls", "style", "className", "children", "direction", "type", "labelPlacement", "iconPrefix", "status", "size", "current", "progressDot", "stepIcon", "initial", "icons", "onChange", "items"],
+        c = (c = H.a.Component, Object(r.a)(cn, c), an = Object(o.a)(cn), Object(a.a)(cn, [{
             key: "render",
             value: function() {
                 var a = this,
                     t = this.props,
                     r = t.prefixCls,
                     e = t.style,
                     o = void 0 === e ? {} : e,
@@ -107034,123 +107115,123 @@
                     p = t.progressDot,
                     f = t.stepIcon,
                     h = t.initial,
                     m = t.icons,
                     g = t.onChange,
                     b = t.items,
                     b = void 0 === b ? [] : b,
-                    t = Object(Bt.a)(t, an),
+                    t = Object(Jt.a)(t, ln),
                     i = "navigation" === i,
                     l = p ? "vertical" : l,
                     u = Kt()(r, "".concat(r, "-").concat(n), e, (e = {}, Object(Vt.a)(e, "".concat(r, "-").concat(u), u), Object(Vt.a)(e, "".concat(r, "-label-").concat(l), "horizontal" === n), Object(Vt.a)(e, "".concat(r, "-dot"), !!p), Object(Vt.a)(e, "".concat(r, "-navigation"), i), e));
                 return H.a.createElement("div", Object(Et.a)({
                     className: u,
                     style: o
                 }, t), b.filter(function(t) {
                     return t
                 }).map(function(t, e) {
                     var t = Object(Ct.a)({}, t),
                         n = h + e;
-                    return "error" === s && e === d - 1 && (t.className = "".concat(r, "-next-error")), t.status || (t.status = n === d ? s : n < d ? "finish" : "wait"), H.a.createElement(nn, Object(Et.a)({}, t, {
+                    return "error" === s && e === d - 1 && (t.className = "".concat(r, "-next-error")), t.status || (t.status = n === d ? s : n < d ? "finish" : "wait"), H.a.createElement(on, Object(Et.a)({}, t, {
                         active: n === d,
                         stepNumber: n + 1,
                         stepIndex: n,
                         key: n,
                         prefixCls: r,
                         iconPrefix: c,
                         wrapperStyle: o,
                         progressDot: p,
                         stepIcon: f,
                         icons: m,
                         onStepClick: g && a.onStepClick
                     }))
                 }))
             }
-        }]), rn);
+        }]), cn);
 
-    function rn() {
+    function cn() {
         var a;
-        Object(i.a)(this, rn);
+        Object(i.a)(this, cn);
         for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
-        return a = tn.call.apply(tn, [this].concat(e)), Object(Vt.a)(Object(s.a)(a), "onStepClick", function(t) {
+        return a = an.call.apply(an, [this].concat(e)), Object(Vt.a)(Object(s.a)(a), "onStepClick", function(t) {
             var e = a.props,
                 n = e.onChange,
                 e = e.current;
             n && e !== t && n(t)
         }), a
     }
 
-    function on() {
+    function sn() {
         var a;
-        Object(i.a)(this, on);
+        Object(i.a)(this, sn);
         for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
-        return a = en.call.apply(en, [this].concat(e)), Object(Vt.a)(Object(s.a)(a), "onClick", function() {
+        return a = rn.call.apply(rn, [this].concat(e)), Object(Vt.a)(Object(s.a)(a), "onClick", function() {
             var t = a.props,
                 e = t.onClick,
                 n = t.onStepClick,
                 t = t.stepIndex;
             e && e.apply(void 0, arguments), n(t)
         }), a
     }
-    Object(Vt.a)(c, "Step", nn), Object(Vt.a)(c, "defaultProps", {
+    Object(Vt.a)(c, "Step", on), Object(Vt.a)(c, "defaultProps", {
         type: "default",
         prefixCls: "rc-steps",
         iconPrefix: "rc",
         direction: "horizontal",
         labelPlacement: "horizontal",
         initial: 0,
         current: 0,
         status: "process",
         size: "",
         progressDot: !1
     });
 
-    function ln() {
+    function un() {
         var t = Object(Wt.useRef)([]),
             a = Object(Wt.useRef)(null);
         return Object(Wt.useEffect)(function() {
             var e = Date.now(),
                 n = !1;
             t.current.forEach(function(t) {
                 t && (n = !0, (t = t.style).transitionDuration = ".3s, .3s, .3s, .06s", a.current) && e - a.current < 100 && (t.transitionDuration = "0s, 0s")
             }), n && (a.current = Date.now())
         }), t.current
     }
-    var cn = c,
-        sn = e(142),
-        un = e(121),
-        dn = e(75),
-        pn = e(124),
+    var dn = c,
+        pn = e(142),
+        fn = e(121),
+        hn = e(75),
+        mn = e(124),
         c = {
             className: "",
             percent: 0,
             prefixCls: "rc-progress",
             strokeColor: "#2db7f5",
             strokeLinecap: "round",
             strokeWidth: 1,
             style: {},
             trailColor: "#D9D9D9",
             trailWidth: 1,
             gapPosition: "bottom"
         },
         u = e(61),
-        fn = 0,
-        hn = Object(u.a)(),
-        mn = ["id", "prefixCls", "steps", "strokeWidth", "trailWidth", "gapDegree", "gapPosition", "trailColor", "strokeLinecap", "style", "className", "strokeColor", "percent"];
+        gn = 0,
+        bn = Object(u.a)(),
+        vn = ["id", "prefixCls", "steps", "strokeWidth", "trailWidth", "gapDegree", "gapPosition", "trailColor", "strokeLinecap", "style", "className", "strokeColor", "percent"];
 
-    function gn(t) {
+    function yn(t) {
         return +t.replace("%", "")
     }
 
-    function bn(t) {
+    function xn(t) {
         t = null != t ? t : [];
         return Array.isArray(t) ? t : [t]
     }
 
-    function vn(t, e, n, a, r, o, i, l, c, s) {
+    function _n(t, e, n, a, r, o, i, l, c, s) {
         var u = 10 < arguments.length && void 0 !== arguments[10] ? arguments[10] : 0,
             n = n / 100 * 360 * ((360 - o) / 360),
             o = 0 === o ? 0 : {
                 bottom: 0,
                 top: 180,
                 left: 90,
                 right: -90
@@ -107163,65 +107244,65 @@
             transform: "rotate(".concat(r + n + o, "deg)"),
             transformOrigin: "0 0",
             transition: "stroke-dashoffset .3s ease 0s, stroke-dasharray .3s ease 0s, stroke .3s, stroke-width .06s ease .3s, opacity .3s ease 0s",
             fillOpacity: 0
         }
     }
 
-    function yn(t) {
+    function On(t) {
         var r, o, i, e, l, n = t.id,
             c = t.prefixCls,
             a = t.steps,
             s = t.strokeWidth,
             u = t.trailWidth,
             d = void 0 === (m = t.gapDegree) ? 0 : m,
             p = t.gapPosition,
             f = t.trailColor,
             h = t.strokeLinecap,
             m = t.style,
             g = t.className,
             b = t.strokeColor,
             v = t.percent,
-            t = Object(Bt.a)(t, mn),
+            t = Object(Jt.a)(t, vn),
             y = (j = n, y = Wt.useState(), y = Object(Gt.a)(y, 2), M = y[0], e = y[1], Wt.useEffect(function() {
                 var t;
-                e("rc_progress_".concat((hn ? (t = fn, fn += 1) : t = "TEST_OR_SSR", t)))
+                e("rc_progress_".concat((bn ? (t = gn, gn += 1) : t = "TEST_OR_SSR", t)))
             }, []), j || M),
             x = "".concat(y, "-gradient"),
             _ = 50 - s / 2,
             O = 2 * Math.PI * _,
             w = 0 < d ? 90 + d / 2 : -90,
             k = (360 - d) / 360 * O,
             j = "object" === Object(qt.a)(a) ? a : {
                 count: a,
                 space: 2
             },
             M = j.count,
             E = j.space,
-            y = vn(O, k, 0, 100, w, d, p, f, h, s),
-            a = bn(v),
-            C = bn(b),
+            y = _n(O, k, 0, 100, w, d, p, f, h, s),
+            a = xn(v),
+            C = xn(b),
             S = C.find(function(t) {
                 return t && "object" === Object(qt.a)(t)
             }),
-            L = ln();
+            L = un();
         return Wt.createElement("svg", Object(Et.a)({
             className: Kt()("".concat(c, "-circle"), g),
             viewBox: "".concat(-50, " ").concat(-50, " ").concat(100, " ").concat(100),
             style: m,
             id: n,
             role: "presentation"
         }, t), S && Wt.createElement("defs", null, Wt.createElement("linearGradient", {
             id: x,
             x1: "100%",
             y1: "0%",
             x2: "0%",
             y2: "0%"
         }, Object.keys(S).sort(function(t, e) {
-            return gn(t) - gn(e)
+            return yn(t) - yn(e)
         }).map(function(t, e) {
             return Wt.createElement("stop", {
                 key: e,
                 offset: t,
                 stopColor: S[t]
             })
         }))), !M && Wt.createElement("circle", {
@@ -107232,15 +107313,15 @@
             stroke: f,
             strokeLinecap: h,
             strokeWidth: u || s,
             style: y
         }), M ? (r = Math.round(M * (a[0] / 100)), o = 100 / M, i = 0, new Array(M).fill(null).map(function(t, e) {
             var n = e <= r - 1 ? C[0] : f,
                 a = n && "object" === Object(qt.a)(n) ? "url(#".concat(x, ")") : void 0,
-                n = vn(O, k, i, o, w, d, p, n, "butt", s, E);
+                n = _n(O, k, i, o, w, d, p, n, "butt", s, E);
             return i += 100 * (k - n.strokeDashoffset + E) / k, Wt.createElement("circle", {
                 key: e,
                 className: "".concat(c, "-circle-path"),
                 r: _,
                 cx: 0,
                 cy: 0,
                 stroke: a,
@@ -107250,15 +107331,15 @@
                 ref: function(t) {
                     L[e] = t
                 }
             })
         })) : (l = 0, a.map(function(t, e) {
             var n = C[e] || C[C.length - 1],
                 a = n && "object" === Object(qt.a)(n) ? "url(#".concat(x, ")") : void 0,
-                n = vn(O, k, l, t, w, d, p, n, h, s);
+                n = _n(O, k, l, t, w, d, p, n, h, s);
             return l += t, Wt.createElement("circle", {
                 key: e,
                 className: "".concat(c, "-circle-path"),
                 r: _,
                 cx: 0,
                 cy: 0,
                 stroke: a,
@@ -107268,30 +107349,30 @@
                 style: n,
                 ref: function(t) {
                     L[e] = t
                 }
             })
         }).reverse()))
     }
-    yn.defaultProps = c, yn.displayName = "Circle";
-    var xn = yn;
+    On.defaultProps = c, On.displayName = "Circle";
+    var wn = On;
 
-    function _n(t) {
+    function kn(t) {
         return !t || t < 0 ? 0 : 100 < t ? 100 : t
     }
 
-    function On(t) {
+    function jn(t) {
         var e = t.success,
             t = t.successPercent;
         return e && "progress" in e && (t = e.progress), t = e && "percent" in e ? e.percent : t
     }
 
-    function wn(t, e) {
-        var n, a, r = void 0 === (r = t.from) ? pn.b.blue : r,
-            o = void 0 === (o = t.to) ? pn.b.blue : o,
+    function Mn(t, e) {
+        var n, a, r = void 0 === (r = t.from) ? mn.b.blue : r,
+            o = void 0 === (o = t.to) ? mn.b.blue : o,
             e = void 0 === (i = t.direction) ? "rtl" === e ? "to left" : "to right" : i,
             i = function(t, e) {
                 var n = {};
                 for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
                 if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                     for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
                 return n
@@ -107311,56 +107392,56 @@
         }).join(", "), {
             backgroundImage: "linear-gradient(".concat(e, ", ").concat(t, ")")
         }) : {
             backgroundImage: "linear-gradient(".concat(e, ", ").concat(r, ", ").concat(o, ")")
         }
     }
 
-    function kn(t) {
+    function En(t) {
         var e, n, a, r = t.prefixCls,
             o = t.className,
             i = t.steps,
             l = t.strokeColor,
             c = void 0 === (c = t.percent) ? 0 : c,
             s = void 0 === (s = t.size) ? "default" : s,
             u = void 0 === (u = t.showInfo) || u,
             d = void 0 === (d = t.type) ? "line" : d,
-            p = Ln(t, ["prefixCls", "className", "steps", "strokeColor", "percent", "size", "showInfo", "type"]),
+            p = Tn(t, ["prefixCls", "className", "steps", "strokeColor", "percent", "size", "showInfo", "type"]),
             f = (h = Wt.useContext(q.b)).getPrefixCls,
             h = h.direction,
             f = f("progress", r),
-            m = (r = t.status, !Pn.includes(r) && (m = On(t), 100 <= parseInt((void 0 !== m ? m : c).toString(), 10)) ? "success" : r || "normal"),
-            g = (r = f, n = m, g = t.format, b = On(t), u ? (v = "line" === d, g || "exception" !== n && "success" !== n ? a = (g || function(t) {
+            m = (r = t.status, !zn.includes(r) && (m = jn(t), 100 <= parseInt((void 0 !== m ? m : c).toString(), 10)) ? "success" : r || "normal"),
+            g = (r = f, n = m, g = t.format, b = jn(t), u ? (v = "line" === d, g || "exception" !== n && "success" !== n ? a = (g || function(t) {
                 return "".concat(t, "%")
-            })(_n(c), _n(b)) : "exception" === n ? a = v ? Wt.createElement(dn.a, null) : Wt.createElement(Ze.a, null) : "success" === n && (a = v ? Wt.createElement(un.a, null) : Wt.createElement($e.a, null)), Wt.createElement("span", {
+            })(kn(c), kn(b)) : "exception" === n ? a = v ? Wt.createElement(hn.a, null) : Wt.createElement(tn.a, null) : "success" === n && (a = v ? Wt.createElement(fn.a, null) : Wt.createElement(Qe.a, null)), Wt.createElement("span", {
                 className: "".concat(r, "-text"),
                 title: "string" == typeof a ? a : void 0
             }, a)) : null),
             c = Array.isArray(l) ? l[0] : l,
             b = "string" == typeof l || Array.isArray(l) ? l : void 0,
-            v = ("line" === d ? e = i ? Wt.createElement(Sn, Object(Et.a)({}, t, {
+            v = ("line" === d ? e = i ? Wt.createElement(Dn, Object(Et.a)({}, t, {
                 strokeColor: b,
                 prefixCls: f,
                 steps: i
-            }), g) : Wt.createElement(Cn, Object(Et.a)({}, t, {
+            }), g) : Wt.createElement(Pn, Object(Et.a)({}, t, {
                 strokeColor: c,
                 prefixCls: f,
                 direction: h
-            }), g) : "circle" !== d && "dashboard" !== d || (e = Wt.createElement(En, Object(Et.a)({}, t, {
+            }), g) : "circle" !== d && "dashboard" !== d || (e = Wt.createElement(Ln, Object(Et.a)({}, t, {
                 strokeColor: c,
                 prefixCls: f,
                 progressStatus: m
             }), g)), Kt()(f, (n = {}, Object(Vt.a)(n, "".concat(f, "-").concat(("dashboard" === d ? "circle" : i && "steps") || d), !0), Object(Vt.a)(n, "".concat(f, "-status-").concat(m), !0), Object(Vt.a)(n, "".concat(f, "-show-info"), u), Object(Vt.a)(n, "".concat(f, "-").concat(s), s), Object(Vt.a)(n, "".concat(f, "-rtl"), "rtl" === h), n), o));
-        return Wt.createElement("div", Object(Et.a)({}, Object(ct.a)(p, ["status", "format", "trailColor", "strokeWidth", "width", "gapDegree", "gapPosition", "strokeLinecap", "success", "successPercent"]), {
+        return Wt.createElement("div", Object(Et.a)({}, Object(pt.a)(p, ["status", "format", "trailColor", "strokeWidth", "width", "gapDegree", "gapPosition", "strokeLinecap", "success", "successPercent"]), {
             className: v,
             role: "progressbar"
         }), e)
     }
 
-    function jn(t) {
+    function Cn(t) {
         var n = t.percent,
             a = t.size,
             e = t.className,
             r = t.direction,
             o = t.items,
             i = void 0 === (l = t.responsive) || l,
             l = void 0 === (l = t.current) ? 0 : l,
@@ -107368,52 +107449,52 @@
             s = function(t, e) {
                 var n = {};
                 for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
                 if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                     for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
                 return n
             }(t, ["percent", "size", "className", "direction", "items", "responsive", "current", "children"]),
-            u = Object(sn.a)(i).xs,
+            u = Object(pn.a)(i).xs,
             d = (p = Wt.useContext(q.b)).getPrefixCls,
             p = p.direction,
             f = Wt.useCallback(function() {
                 return i && u ? "vertical" : r
             }, [u, r]),
             h = d("steps", t.prefixCls),
             d = d("", t.iconPrefix),
-            c = (t = c, o || Object(Dn.a)(t).map(function(t) {
+            c = (t = c, o || Object(An.a)(t).map(function(t) {
                 if (Wt.isValidElement(t)) {
                     var e = t.props;
                     return Object(Et.a)({}, e)
                 }
                 return null
             }).filter(function(t) {
                 return t
             })),
             t = Kt()((o = {}, Object(Vt.a)(o, "".concat(h, "-rtl"), "rtl" === p), Object(Vt.a)(o, "".concat(h, "-with-progress"), void 0 !== n), o), e),
             p = {
-                finish: Wt.createElement($e.a, {
+                finish: Wt.createElement(Qe.a, {
                     className: "".concat(h, "-finish-icon")
                 }),
-                error: Wt.createElement(Ze.a, {
+                error: Wt.createElement(tn.a, {
                     className: "".concat(h, "-error-icon")
                 })
             };
-        return Wt.createElement(cn, Object(Et.a)({
+        return Wt.createElement(dn, Object(Et.a)({
             icons: p
         }, s, {
             current: l,
             size: a,
             items: c,
             direction: f(),
             stepIcon: function(t) {
                 var e = t.node;
                 return "process" === t.status && void 0 !== n ? (t = "small" === a ? 32 : 40, Wt.createElement("div", {
                     className: "".concat(h, "-progress-icon")
-                }, Wt.createElement(kn, {
+                }, Wt.createElement(En, {
                     type: "circle",
                     percent: n,
                     width: t,
                     strokeWidth: 4,
                     format: function() {
                         return null
                     }
@@ -107421,15 +107502,15 @@
             },
             prefixCls: h,
             iconPrefix: d,
             className: t
         }))
     }
 
-    function Mn(t) {
+    function Sn(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.current,
             i = t.direction,
             l = t.labelPlacement,
@@ -107442,15 +107523,15 @@
             h = t.responsive,
             m = t.setProps,
             t = t.loading_state;
         return m({
             current: o < p.length ? o : p.length
         }), m({
             current: 0 <= o ? o : 0
-        }), H.a.createElement(Tn, {
+        }), H.a.createElement(Rn, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             "data-dash-is-loading": t && t.is_loading || void 0,
             current: o,
             direction: i,
@@ -107462,22 +107543,22 @@
             responsive: h,
             onChange: f ? function(t) {
                 return m({
                     current: t
                 })
             } : void 0
         }, p.map(function(t) {
-            return H.a.createElement(zn, {
+            return H.a.createElement(In, {
                 title: t.title,
                 subTitle: t.subTitle,
                 description: t.description
             })
         }))
     }
-    var En = function(t) {
+    var Ln = function(t) {
             var e = t.prefixCls,
                 n = t.width,
                 a = t.strokeWidth,
                 r = t.trailColor,
                 r = void 0 === r ? null : r,
                 o = t.strokeLinecap,
                 o = void 0 === o ? "round" : o,
@@ -107494,63 +107575,63 @@
                 },
                 a = a || 6,
                 i = i || ("dashboard" === c ? "bottom" : void 0),
                 d = "[object Object]" === Object.prototype.toString.call(t.strokeColor),
                 p = (u = {
                     success: u,
                     strokeColor: t.strokeColor
-                }, [(void 0 === (p = u.success) ? {} : p).strokeColor || pn.b.green, u.strokeColor || null]),
+                }, [(void 0 === (p = u.success) ? {} : p).strokeColor || mn.b.green, u.strokeColor || null]),
                 u = Kt()("".concat(e, "-inner"), Object(Vt.a)({}, "".concat(e, "-circle-gradient"), d));
             return Wt.createElement("div", {
                 className: u,
                 style: n
-            }, Wt.createElement(xn, {
-                percent: (d = t.percent, [u = _n(On({
+            }, Wt.createElement(wn, {
+                percent: (d = t.percent, [u = kn(jn({
                     success: t.success,
                     successPercent: t.successPercent
-                })), _n(_n(d) - u)]),
+                })), kn(kn(d) - u)]),
                 strokeWidth: a,
                 trailWidth: a,
                 strokeColor: p,
                 strokeLinecap: o,
                 trailColor: r,
                 prefixCls: e,
                 gapDegree: l || 0 === l ? l : "dashboard" === c ? 75 : void 0,
                 gapPosition: i
             }), s)
         },
-        Cn = function(t) {
+        Pn = function(t) {
             var e = t.prefixCls,
                 n = t.direction,
                 a = t.percent,
                 r = t.strokeWidth,
                 o = t.size,
                 i = t.strokeColor,
                 l = t.strokeLinecap,
                 l = void 0 === l ? "round" : l,
                 c = t.children,
                 s = t.trailColor,
                 s = void 0 === s ? null : s,
                 u = t.success,
-                n = i && "string" != typeof i ? wn(i, n) : {
+                n = i && "string" != typeof i ? Mn(i, n) : {
                     background: i
                 },
                 i = "square" === l || "butt" === l ? 0 : void 0,
                 l = {
                     backgroundColor: s || void 0,
                     borderRadius: i
                 },
                 s = Object(Et.a)({
-                    width: "".concat(_n(a), "%"),
+                    width: "".concat(kn(a), "%"),
                     height: r || ("small" === o ? 6 : 8),
                     borderRadius: i
                 }, n),
-                a = On(t),
+                a = jn(t),
                 n = {
-                    width: "".concat(_n(a), "%"),
+                    width: "".concat(kn(a), "%"),
                     height: r || ("small" === o ? 6 : 8),
                     borderRadius: i,
                     backgroundColor: null == u ? void 0 : u.strokeColor
                 },
                 t = void 0 !== a ? Wt.createElement("div", {
                     className: "".concat(e, "-success-bg"),
                     style: n
@@ -107561,15 +107642,15 @@
                 className: "".concat(e, "-inner"),
                 style: l
             }, Wt.createElement("div", {
                 className: "".concat(e, "-bg"),
                 style: s
             }), t)), c)
         },
-        Sn = function(t) {
+        Dn = function(t) {
             for (var e = t.size, n = t.steps, a = t.percent, r = t.strokeWidth, o = void 0 === r ? 8 : r, i = t.strokeColor, r = t.trailColor, l = void 0 === r ? null : r, c = t.prefixCls, r = t.children, s = Math.round(n * ((void 0 === a ? 0 : a) / 100)), u = "small" === e ? 2 : 14, d = new Array(n), p = 0; p < n; p++) {
                 var f = Array.isArray(i) ? i[p] : i;
                 d[p] = Wt.createElement("div", {
                     key: p,
                     className: Kt()("".concat(c, "-steps-item"), Object(Vt.a)({}, "".concat(c, "-steps-item-active"), p <= s - 1)),
                     style: {
                         backgroundColor: p <= s - 1 ? f : l,
@@ -107578,26 +107659,26 @@
                     }
                 })
             }
             return Wt.createElement("div", {
                 className: "".concat(c, "-steps-outer")
             }, d, r)
         },
-        Ln = function(t, e) {
+        Tn = function(t, e) {
             var n = {};
             for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
             if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                 for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
             return n
         },
-        Pn = (Object(l.a)("line", "circle", "dashboard"), Object(l.a)("normal", "exception", "active", "success")),
-        Dn = e(43),
-        Tn = (jn.Step = cn.Step, jn),
-        zn = Tn.Step,
-        An = (Mn.propTypes = {
+        zn = (Object(l.a)("line", "circle", "dashboard"), Object(l.a)("normal", "exception", "active", "success")),
+        An = e(43),
+        Rn = (Cn.Step = dn.Step, Cn),
+        In = Rn.Step,
+        Nn = (Sn.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             steps: n.a.arrayOf(n.a.exact({
                 title: n.a.node.isRequired,
                 subTitle: n.a.node,
@@ -107614,124 +107695,124 @@
             responsive: n.a.bool,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, Mn.defaultProps = {
+        }, Sn.defaultProps = {
             current: 0,
             direction: "horizontal",
             progressDot: !1,
             size: "default",
             status: "process",
             type: "default",
             allowClick: !1,
             responsive: !0
-        }, Mn);
-    const Rn = /^[a-zA-Z][a-zA-Z\d+\-.]*?:/,
-        In = /^[a-zA-Z]:\\/;
-    var Nn = e(105),
-        Yn = e(714),
-        Bn = e(713);
+        }, Sn);
+    const Yn = /^[a-zA-Z][a-zA-Z\d+\-.]*?:/,
+        Bn = /^[a-zA-Z]:\\/;
+    var Fn = e(105),
+        Hn = e(714),
+        Wn = e(713);
 
-    function Fn(t) {
-        return (Fn = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
+    function Vn(t) {
+        return (Vn = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
             return typeof t
         } : function(t) {
             return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
         })(t)
     }
-    var Hn = ["children", "external_link", "preOnClick", "target", "href", "download"];
+    var Kn = ["children", "external_link", "preOnClick", "target", "href", "download"];
 
-    function Wn() {
-        return (Wn = Object.assign ? Object.assign.bind() : function(t) {
+    function Un() {
+        return (Un = Object.assign ? Object.assign.bind() : function(t) {
             for (var e = 1; e < arguments.length; e++) {
                 var n, a = arguments[e];
                 for (n in a) Object.prototype.hasOwnProperty.call(a, n) && (t[n] = a[n])
             }
             return t
         }).apply(this, arguments)
     }
 
-    function Vn(t, e) {
+    function Gn(t, e) {
         for (var n, a = 0; a < e.length; a++) {
             var r = e[a];
             r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(t, (n = function(t) {
-                if ("object" !== Fn(t) || null === t) return t;
+                if ("object" !== Vn(t) || null === t) return t;
                 var e = t[Symbol.toPrimitive];
                 if (void 0 === e) return String(t);
                 e = e.call(t, "string");
-                if ("object" !== Fn(e)) return e;
+                if ("object" !== Vn(e)) return e;
                 throw new TypeError("@@toPrimitive must return a primitive value.")
-            }(r.key), "symbol" === Fn(n) ? n : String(n)), r)
+            }(r.key), "symbol" === Vn(n) ? n : String(n)), r)
         }
     }
 
-    function Kn(t, e) {
-        return (Kn = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(t, e) {
+    function qn(t, e) {
+        return (qn = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(t, e) {
             return t.__proto__ = e, t
         })(t, e)
     }
 
-    function Un(n) {
+    function Xn(n) {
         var a = function() {
             if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
             if (Reflect.construct.sham) return !1;
             if ("function" == typeof Proxy) return !0;
             try {
                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], function() {})), !0
             } catch (t) {
                 return !1
             }
         }();
         return function() {
-            var t, e = qn(n),
-                e = (t = a ? (t = qn(this).constructor, Reflect.construct(e, arguments, t)) : e.apply(this, arguments), this);
-            if (t && ("object" === Fn(t) || "function" == typeof t)) return t;
+            var t, e = Zn(n),
+                e = (t = a ? (t = Zn(this).constructor, Reflect.construct(e, arguments, t)) : e.apply(this, arguments), this);
+            if (t && ("object" === Vn(t) || "function" == typeof t)) return t;
             if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-            return Gn(e)
+            return $n(e)
         }
     }
 
-    function Gn(t) {
+    function $n(t) {
         if (void 0 === t) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
         return t
     }
 
-    function qn(t) {
-        return (qn = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(t) {
+    function Zn(t) {
+        return (Zn = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(t) {
             return t.__proto__ || Object.getPrototypeOf(t)
         })(t)
     }
-    var Xn = Nn.a.SubMenu,
-        $n = Nn.a.Item,
-        Zn = Nn.a.ItemGroup,
-        Jn = Nn.a.Divider;
+    var Jn = Fn.a.SubMenu,
+        Qn = Fn.a.Item,
+        ta = Fn.a.ItemGroup,
+        ea = Fn.a.Divider;
 
-    function Qn(t, e) {
+    function na(t, e) {
         e = e || {
             bubbles: !1,
             cancelable: !1,
             detail: void 0
         };
         var n = document.createEvent("CustomEvent");
         return n.initCustomEvent(t, e.bubbles, e.cancelable, e.detail), n
     }
 
-    function ta(t, e) {
+    function aa(t, e) {
         if (Object(V.isUndefined)(t) || Object(V.isNull)(t)) {
             if ("string" != typeof e) throw new TypeError(`Expected a \`string\`, got \`${typeof e}\``);
-            return !In.test(e) && Rn.test(e)
+            return !Bn.test(e) && Yn.test(e)
         }
         return t
     }
-    Qn.prototype = window.Event.prototype;
+    na.prototype = window.Event.prototype;
 
-    function ea(t) {
+    function ra(t) {
         function e(t) {
             g({
                 currentKey: t.key
             })
         }
         var n = t.id,
             a = t.className,
@@ -107761,65 +107842,65 @@
             }, []), function e(t, n) {
                 return Array.isArray(t) ? t = t.map(function(t) {
                     return e(t, n)
                 }) : t.hasOwnProperty("component") && (t = t.hasOwnProperty("children") ? (Object.assign(t, {
                     children: t.children.map(function(t) {
                         return e(t, n)
                     })
-                }), "SubMenu" === t.component ? H.a.createElement(Xn, {
+                }), "SubMenu" === t.component ? H.a.createElement(Jn, {
                     key: t.props.key,
                     title: t.props.title,
                     disabled: t.props.disabled,
                     icon: H.a.createElement(I.a, {
                         icon: t.props.icon
                     })
-                }, t.children) : H.a.createElement(Zn, {
+                }, t.children) : H.a.createElement(ta, {
                     key: t.props.key,
                     title: t.props.title,
                     disabled: t.props.disabled,
                     icon: H.a.createElement(I.a, {
                         icon: t.props.icon
                     })
-                }, t.children)) : "Divider" === t.component ? H.a.createElement(Jn, {
+                }, t.children)) : "Divider" === t.component ? H.a.createElement(ea, {
                     dashed: t.props && t.props.dashed
-                }) : t.props.href ? H.a.createElement($n, {
+                }) : t.props.href ? H.a.createElement(Qn, {
                     key: t.props.key,
                     title: t.props.title,
                     disabled: t.props.disabled,
                     danger: t.props.danger,
                     icon: H.a.createElement(I.a, {
                         icon: t.props.icon
                     }),
                     name: t.props && t.props.name
-                }, H.a.createElement(ra, {
+                }, H.a.createElement(la, {
                     href: t.props.href,
                     target: t.props.target
-                }, t.props.title)) : H.a.createElement($n, {
+                }, t.props.title)) : H.a.createElement(Qn, {
                     key: t.props.key,
                     title: t.props.title,
                     disabled: t.props.disabled,
                     danger: t.props.danger,
                     icon: H.a.createElement(I.a, {
                         icon: t.props.icon
                     }),
                     name: t.props && t.props.name
                 }, t.props.title)), t
-            }(i, oa));
+            }(i, ca));
         return f ? H.a.createElement("div", {
             style: {
                 width: "100%"
             }
         }, H.a.createElement(z.a, {
             type: "primary",
             onClick: function() {
                 return g({
                     inlineCollapsed: !m
                 })
             }
-        }, H.a.createElement((m ? Yn : Bn).a)), H.a.createElement(Nn.a, {
+        }, H.a.createElement((m ? Hn : Wn).a)), H.a.createElement(Fn.a, {
             id: n,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             mode: l,
             theme: c,
             selectedKeys: [u],
@@ -107836,15 +107917,15 @@
                 return t.parentNode
             } : void 0,
             inlineCollapsed: m,
             persistence: b,
             persisted_props: v,
             persistence_type: y,
             "data-dash-is-loading": t && t.is_loading || void 0
-        }, i)) : H.a.createElement(Nn.a, {
+        }, i)) : H.a.createElement(Fn.a, {
             id: n,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             mode: l,
             theme: c,
             selectedKeys: [u],
@@ -107863,15 +107944,15 @@
             persistence: b,
             persisted_props: v,
             persistence_type: y,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, i)
     }
 
-    function na(t) {
+    function oa(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.title,
             l = t.isOpen,
@@ -107882,15 +107963,15 @@
             p = t.forceRender,
             f = t.setProps,
             h = t.persistence,
             m = t.persisted_props,
             g = t.persistence_type,
             t = t.loading_state,
             n = j(n);
-        return H.a.createElement(la.a, {
+        return H.a.createElement(ua.a, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             activeKey: l ? ["1"] : [],
             style: r,
             key: o,
             bordered: c,
             ghost: d,
@@ -107902,69 +107983,69 @@
                     isOpen: !1
                 })
             },
             persistence: h,
             persisted_props: m,
             persistence_type: g,
             "data-dash-is-loading": t && t.is_loading || void 0
-        }, H.a.createElement(ca, {
+        }, H.a.createElement(da, {
             key: "1",
             header: i,
             showArrow: s,
             forceRender: p
         }, n))
     }
 
-    function aa(t) {
+    function ia(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.align,
             l = t.gutter,
             c = t.justify,
             s = t.wrap,
             t = (t.setProps, t.loading_state),
             n = j(n);
-        return H.a.createElement(ua, {
+        return H.a.createElement(fa, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             align: i,
             gutter: l,
             justify: c,
             wrap: s,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
-    var ra = function(t) {
+    var la = function(t) {
             var e = a;
             if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
             e.prototype = Object.create(t && t.prototype, {
                 constructor: {
                     value: e,
                     writable: !0,
                     configurable: !0
                 }
             }), Object.defineProperty(e, "prototype", {
                 writable: !1
-            }), t && Kn(e, t);
-            var n = Un(a);
+            }), t && qn(e, t);
+            var n = Xn(a);
 
             function a(t) {
-                if (this instanceof a) return (t = n.call(this, t)).updateLocation = t.updateLocation.bind(Gn(t)), t;
+                if (this instanceof a) return (t = n.call(this, t)).updateLocation = t.updateLocation.bind($n(t)), t;
                 throw new TypeError("Cannot call a class as a function")
             }
-            return Vn((e = a).prototype, [{
+            return Gn((e = a).prototype, [{
                 key: "updateLocation",
                 value: function(t) {
                     var e, n;
-                    t.metaKey || t.shiftKey || t.altKey || t.ctrlKey || (this.props.disabled ? t.preventDefault() : (this.props.preOnClick && this.props.preOnClick(), n = (e = this.props).external_link, (e = e.href) && !ta(n, e) && (t.preventDefault(), n = this.props.href, window.history.pushState({}, "", n), window.dispatchEvent(new Qn("_dashprivate_pushstate")), window.scrollTo(0, 0))))
+                    t.metaKey || t.shiftKey || t.altKey || t.ctrlKey || (this.props.disabled ? t.preventDefault() : (this.props.preOnClick && this.props.preOnClick(), n = (e = this.props).external_link, (e = e.href) && !aa(n, e) && (t.preventDefault(), n = this.props.href, window.history.pushState({}, "", n), window.dispatchEvent(new na("_dashprivate_pushstate")), window.scrollTo(0, 0))))
                 }
             }, {
                 key: "render",
                 value: function() {
                     var e = this,
                         t = this.props,
                         n = t.children,
@@ -107978,37 +108059,37 @@
                                 if (null == t) return {};
                                 for (var n, a = {}, r = Object.keys(t), o = 0; o < r.length; o++) n = r[o], 0 <= e.indexOf(n) || (a[n] = t[n]);
                                 return a
                             }(t, e);
                             if (Object.getOwnPropertySymbols)
                                 for (var r = Object.getOwnPropertySymbols(t), o = 0; o < r.length; o++) n = r[o], 0 <= e.indexOf(n) || Object.prototype.propertyIsEnumerable.call(t, n) && (a[n] = t[n]);
                             return a
-                        }(t, Hn),
-                        a = o && ta(a, o);
-                    return H.a.createElement("a", Wn({
+                        }(t, Kn),
+                        a = o && aa(a, o);
+                    return H.a.createElement("a", Un({
                         href: o,
                         target: a ? r : null,
                         download: i && a ? i : null
                     }, t, {
                         onClick: function(t) {
                             return e.updateLocation(t)
                         }
                     }), n)
                 }
             }]), Object.defineProperty(e, "prototype", {
                 writable: !1
             }), a
         }(Wt.Component),
-        oa = new Map([
-            ["SubMenu", Xn],
-            ["Item", $n],
-            ["ItemGroup", Zn],
-            ["Divider", Jn]
+        ca = new Map([
+            ["SubMenu", Jn],
+            ["Item", Qn],
+            ["ItemGroup", ta],
+            ["Divider", ea]
         ]),
-        ia = (ea.propTypes = {
+        sa = (ra.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             menuItems: n.a.array,
             mode: n.a.oneOf(["vertical", "horizontal", "inline"]),
             theme: n.a.oneOf(["light", "dark"]),
@@ -108024,26 +108105,26 @@
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func,
             persistence: n.a.oneOfType([n.a.bool, n.a.string, n.a.number]),
             persisted_props: n.a.arrayOf(n.a.oneOf(["currentKey", "openKeys"])),
             persistence_type: n.a.oneOf(["local", "session", "memory"])
-        }, ea.defaultProps = {
+        }, ra.defaultProps = {
             mode: "vertical",
             theme: "light",
             renderCollapsedButton: !1,
             popupContainer: "body",
             inlineCollapsed: !1,
             persisted_props: ["currentKey", "openKeys"],
             persistence_type: "local"
-        }, ea),
-        la = e(709),
-        ca = la.a.Panel,
-        sa = (na.propTypes = {
+        }, ra),
+        ua = e(709),
+        da = ua.a.Panel,
+        pa = (oa.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             title: n.a.node,
             isOpen: n.a.bool,
@@ -108057,25 +108138,25 @@
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func,
             persistence: n.a.oneOfType([n.a.bool, n.a.string, n.a.number]),
             persisted_props: n.a.arrayOf(n.a.oneOf(["isOpen"])),
             persistence_type: n.a.oneOf(["local", "session", "memory"])
-        }, na.defaultProps = {
+        }, oa.defaultProps = {
             isOpen: !0,
             bordered: !0,
             showArrow: !0,
             ghost: !1,
             forceRender: !1,
             persisted_props: ["isOpen"],
             persistence_type: "local"
-        }, na),
-        ua = e(704).a;
-    aa.propTypes = {
+        }, oa),
+        fa = e(704).a;
+    ia.propTypes = {
         id: n.a.string,
         children: n.a.node,
         className: n.a.oneOfType([n.a.string, n.a.object]),
         style: n.a.object,
         key: n.a.string,
         align: n.a.oneOf(["top", "middle", "bottom"]),
         gutter: n.a.oneOfType([n.a.number, n.a.arrayOf(n.a.number), n.a.exact({
@@ -108090,56 +108171,56 @@
         wrap: n.a.bool,
         loading_state: n.a.shape({
             is_loading: n.a.bool,
             prop_name: n.a.string,
             component_name: n.a.string
         }),
         setProps: n.a.func
-    }, aa.defaultProps = {
+    }, ia.defaultProps = {
         align: "top",
         gutter: 0,
         justify: "start",
         wrap: !0
     };
-    var da = aa,
-        pa = e(257).a;
+    var ha = ia,
+        ma = e(257).a;
 
-    function fa(t) {
-        return (fa = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
+    function ga(t) {
+        return (ga = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
             return typeof t
         } : function(t) {
             return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
         })(t)
     }
 
-    function ha(e, t) {
+    function ba(e, t) {
         var n, a = Object.keys(e);
         return Object.getOwnPropertySymbols && (n = Object.getOwnPropertySymbols(e), t && (n = n.filter(function(t) {
             return Object.getOwnPropertyDescriptor(e, t).enumerable
         })), a.push.apply(a, n)), a
     }
 
-    function ma(t, e, n) {
+    function va(t, e, n) {
         var a;
         a = function(t) {
-            if ("object" !== fa(t) || null === t) return t;
+            if ("object" !== ga(t) || null === t) return t;
             var e = t[Symbol.toPrimitive];
             if (void 0 === e) return String(t);
             e = e.call(t, "string");
-            if ("object" !== fa(e)) return e;
+            if ("object" !== ga(e)) return e;
             throw new TypeError("@@toPrimitive must return a primitive value.")
-        }(e), (e = "symbol" === fa(a) ? a : String(a)) in t ? Object.defineProperty(t, e, {
+        }(e), (e = "symbol" === ga(a) ? a : String(a)) in t ? Object.defineProperty(t, e, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : t[e] = n
     }
 
-    function ga(t) {
+    function ya(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.span,
             l = t.offset,
@@ -108151,23 +108232,23 @@
             f = t.sm,
             h = t.md,
             m = t.lg,
             g = t.xl,
             b = t.xxl,
             t = (t.setProps, t.loading_state),
             n = j(n);
-        return H.a.createElement(pa, {
+        return H.a.createElement(ma, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: function(e) {
                 for (var t = 1; t < arguments.length; t++) {
                     var n = null != arguments[t] ? arguments[t] : {};
-                    t % 2 ? ha(Object(n), !0).forEach(function(t) {
-                        ma(e, t, n[t])
-                    }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : ha(Object(n)).forEach(function(t) {
+                    t % 2 ? ba(Object(n), !0).forEach(function(t) {
+                        va(e, t, n[t])
+                    }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : ba(Object(n)).forEach(function(t) {
                         Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                     })
                 }
                 return e
             }({
                 height: "100%"
             }, r),
@@ -108184,83 +108265,83 @@
             lg: m,
             xl: g,
             xxl: b,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
 
-    function ba(t) {
+    function xa(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             t = (t.setProps, t.loading_state),
             n = j(n);
-        return H.a.createElement(ka, {
+        return H.a.createElement(Ea, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
 
-    function va(t) {
+    function _a(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             t = (t.setProps, t.loading_state),
             n = j(n);
-        return H.a.createElement(Ma, {
+        return H.a.createElement(Sa, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
 
-    function ya(t) {
+    function Oa(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             t = (t.setProps, t.loading_state),
             n = j(n);
-        return H.a.createElement(Ca, {
+        return H.a.createElement(Pa, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
 
-    function xa(t) {
+    function wa(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             t = (t.setProps, t.loading_state),
             n = j(n);
-        return H.a.createElement(La, {
+        return H.a.createElement(Ta, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
 
-    function _a(t) {
+    function ka(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.breakpoint,
             l = t.collapsed,
@@ -108270,15 +108351,15 @@
             d = t.reverseArrow,
             p = t.theme,
             f = t.width,
             h = t.trigger,
             m = t.setProps,
             t = t.loading_state,
             n = j(n);
-        return H.a.createElement(Da, {
+        return H.a.createElement(Aa, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             collapsed: l,
             collapsedWidth: c,
             collapsible: s,
@@ -108293,66 +108374,66 @@
                     collapsed: t
                 })
             },
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
 
-    function Oa(t) {
+    function ja(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.align,
             l = t.direction,
             c = t.size,
             s = t.split,
             u = t.wrap,
             d = t.addSplitLine,
             t = (t.setProps, t.loading_state),
             n = j(n);
-        return d ? "horizontal" === l ? H.a.createElement(za.b, {
+        return d ? "horizontal" === l ? H.a.createElement(Ia.b, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             align: i,
             direction: l,
             size: c,
             split: H.a.createElement(b, {
                 type: "vertical"
             }),
             wrap: u,
             "data-dash-is-loading": t && t.is_loading || void 0
-        }, n) : H.a.createElement(za.b, {
+        }, n) : H.a.createElement(Ia.b, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             align: i,
             direction: l,
             size: c,
             split: H.a.createElement(b, null),
             wrap: u,
             "data-dash-is-loading": t && t.is_loading || void 0
-        }, n) : H.a.createElement(za.b, {
+        }, n) : H.a.createElement(Ia.b, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             align: i,
             direction: l,
             size: c,
             split: s,
             wrap: u,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
-    ga.propTypes = {
+    ya.propTypes = {
         id: n.a.string,
         children: n.a.node,
         className: n.a.oneOfType([n.a.string, n.a.object]),
         style: n.a.object,
         key: n.a.string,
         span: n.a.number,
         offset: n.a.number,
@@ -108404,79 +108485,79 @@
         })]),
         loading_state: n.a.shape({
             is_loading: n.a.bool,
             prop_name: n.a.string,
             component_name: n.a.string
         }),
         setProps: n.a.func
-    }, ga.defaultProps = (ma(u = {
+    }, ya.defaultProps = (va(u = {
         offset: 0
-    }, "offset", 0), ma(u, "order", 0), ma(u, "pull", 0), ma(u, "push", 0), u);
-    var wa = ga,
+    }, "offset", 0), va(u, "order", 0), va(u, "pull", 0), va(u, "push", 0), u);
+    var Ma = ya,
         c = e(164),
         u = e(195),
         d = c.e,
-        ka = (d.Header = c.c, d.Footer = c.b, d.Content = c.a, d.Sider = u.b, d),
-        ja = (ba.propTypes = {
+        Ea = (d.Header = c.c, d.Footer = c.b, d.Content = c.a, d.Sider = u.b, d),
+        Ca = (xa.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, ba.defaultProps = {}, ba),
-        Ma = ka.Header,
-        Ea = (va.propTypes = {
+        }, xa.defaultProps = {}, xa),
+        Sa = Ea.Header,
+        La = (_a.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, va.defaultProps = {}, va),
-        Ca = ka.Content,
-        Sa = (ya.propTypes = {
+        }, _a.defaultProps = {}, _a),
+        Pa = Ea.Content,
+        Da = (Oa.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, ya.defaultProps = {}, ya),
-        La = ka.Footer,
-        Pa = (xa.propTypes = {
+        }, Oa.defaultProps = {}, Oa),
+        Ta = Ea.Footer,
+        za = (wa.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, xa.defaultProps = {}, xa),
-        Da = ka.Sider,
-        Ta = (_a.propTypes = {
+        }, wa.defaultProps = {}, wa),
+        Aa = Ea.Sider,
+        Ra = (ka.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             collapsed: n.a.bool,
             defaultCollapsed: n.a.bool,
@@ -108489,25 +108570,25 @@
             breakpoint: n.a.oneOf(["xs", "sm", "md", "lg", "xl", "xxl"]),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, _a.defaultProps = {
+        }, ka.defaultProps = {
             collapsed: !1,
             defaultCollapsed: !1,
             collapsedWidth: 80,
             collapsible: !1,
             reverseArrow: !1,
             theme: "dark",
             width: 200
-        }, _a),
-        za = e(166);
-    Oa.propTypes = {
+        }, ka),
+        Ia = e(166);
+    ja.propTypes = {
         id: n.a.string,
         children: n.a.node,
         className: n.a.oneOfType([n.a.string, n.a.object]),
         style: n.a.object,
         key: n.a.string,
         align: n.a.oneOf(["start", "end", "center", "baseline"]),
         direction: n.a.oneOf(["vertical", "horizontal"]),
@@ -108516,22 +108597,22 @@
         wrap: n.a.bool,
         loading_state: n.a.shape({
             is_loading: n.a.bool,
             prop_name: n.a.string,
             component_name: n.a.string
         }),
         setProps: n.a.func
-    }, Oa.defaultProps = {
+    }, ja.defaultProps = {
         addSplitLine: !1,
         direction: "horizontal",
         size: "small",
         wrap: !1
     };
 
-    function Aa(t) {
+    function Na(t) {
         var e = t.icon,
             n = t.onCancel,
             a = t.onOk,
             r = t.close,
             o = t.zIndex,
             i = t.afterClose,
             l = t.visible,
@@ -108559,39 +108640,39 @@
             S = !("okCancel" in t) || t.okCancel,
             L = t.width || 416,
             P = t.style || {},
             D = void 0 === t.mask || t.mask,
             T = void 0 !== t.maskClosable && t.maskClosable,
             z = null !== t.autoFocusButton && (t.autoFocusButton || "ok"),
             A = Kt()(C, "".concat(C, "-").concat(t.type), Object(Vt.a)({}, "".concat(C, "-rtl"), "rtl" === b), t.className),
-            S = S && Wt.createElement(Wa.a, {
+            S = S && Wt.createElement(Ua.a, {
                 actionFn: n,
                 close: r,
                 autoFocus: "cancel" === z,
                 buttonProps: g,
                 prefixCls: "".concat(x, "-btn")
             }, m);
         return Wt.createElement(W.a, {
             prefixCls: x,
             iconPrefixCls: _,
             direction: b
-        }, Wt.createElement(Xa, {
+        }, Wt.createElement(Ja, {
             prefixCls: v,
             className: A,
             wrapClassName: Kt()(Object(Vt.a)({}, "".concat(C, "-centered"), !!t.centered), y),
             onCancel: function() {
                 return null == r ? void 0 : r({
                     triggerCancel: !0
                 })
             },
             open: c || l,
             title: "",
             footer: "",
-            transitionName: Object(Va.c)(x, "zoom", t.transitionName),
-            maskTransitionName: Object(Va.c)(x, "fade", t.maskTransitionName),
+            transitionName: Object(Ga.c)(x, "zoom", t.transitionName),
+            maskTransitionName: Object(Ga.c)(x, "fade", t.maskTransitionName),
             mask: D,
             maskClosable: T,
             maskStyle: p,
             style: P,
             bodyStyle: O,
             width: L,
             zIndex: o,
@@ -108609,42 +108690,42 @@
             className: "".concat(C, "-body")
         }, e, void 0 === t.title ? null : Wt.createElement("span", {
             className: "".concat(C, "-title")
         }, t.title), Wt.createElement("div", {
             className: "".concat(C, "-content")
         }, t.content)), Wt.createElement("div", {
             className: "".concat(C, "-btns")
-        }, S, Wt.createElement(Wa.a, {
+        }, S, Wt.createElement(Ua.a, {
             type: E,
             actionFn: a,
             close: r,
             autoFocus: "ok" === z,
             buttonProps: h,
             prefixCls: "".concat(x, "-btn")
         }, f)))))
     }
-    var Ra, Ia = Oa,
-        Na = e(189),
-        Ya = e(191),
-        Ba = e(163),
-        Fa = e(190),
-        Ha = e(197),
-        Wa = e(218),
-        Va = e(45),
-        Ka = e(274),
-        Ua = e(144),
-        Ga = e(59),
+    var Ya, Ba = ja,
+        Fa = e(189),
+        Ha = e(191),
+        Wa = e(163),
+        Va = e(190),
+        Ka = e(197),
+        Ua = e(218),
+        Ga = e(45),
+        qa = e(274),
+        Xa = e(144),
+        $a = e(59),
         c = e(207),
-        qa = e(154),
-        Xa = (Object(c.a)() && document.documentElement.addEventListener("click", function(t) {
-            Ra = {
+        Za = e(154),
+        Ja = (Object(c.a)() && document.documentElement.addEventListener("click", function(t) {
+            Ya = {
                 x: t.pageX,
                 y: t.pageY
             }, setTimeout(function() {
-                Ra = null
+                Ya = null
             }, 100)
         }, !0), function(o) {
             function i(t) {
                 var e = o.onCancel;
                 null != e && e(t)
             }
 
@@ -108674,60 +108755,60 @@
                     for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
                     if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                         for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
                     return n
                 }(o, ["prefixCls", "footer", "visible", "open", "wrapClassName", "centered", "getContainer", "closeIcon", "focusTriggerAfterClose", "width"]),
                 a = n("modal", a),
                 n = n(),
-                b = Wt.createElement(ye.a, {
+                b = Wt.createElement(we.a, {
                     componentName: "Modal",
-                    defaultLocale: Object(qa.b)()
+                    defaultLocale: Object(Za.b)()
                 }, function(t) {
                     var e = o.okText,
                         n = o.okType,
                         n = void 0 === n ? "primary" : n,
                         a = o.cancelText,
                         r = o.confirmLoading,
                         r = void 0 !== r && r;
                     return Wt.createElement(Wt.Fragment, null, Wt.createElement(z.a, Object(Et.a)({
                         onClick: i
-                    }, o.cancelButtonProps), a || t.cancelText), Wt.createElement(z.a, Object(Et.a)({}, Object(Ua.a)(n), {
+                    }, o.cancelButtonProps), a || t.cancelText), Wt.createElement(z.a, Object(Et.a)({}, Object(Xa.a)(n), {
                         loading: r,
                         onClick: l
                     }, o.okButtonProps), null != e ? e : t.okText))
                 }),
                 f = Wt.createElement("span", {
                     className: "".concat(a, "-close-x")
-                }, f || Wt.createElement(Ze.a, {
+                }, f || Wt.createElement(tn.a, {
                     className: "".concat(a, "-close-icon")
                 })),
                 d = Kt()(u, (u = {}, Object(Vt.a)(u, "".concat(a, "-centered"), !!d), Object(Vt.a)(u, "".concat(a, "-wrap-rtl"), "rtl" === t), u));
-            return Wt.createElement(Ga.a, null, Wt.createElement(ve.e, {
+            return Wt.createElement($a.a, null, Wt.createElement(Oe.e, {
                 status: !0,
                 override: !0
-            }, Wt.createElement(Ka.a, Object(Et.a)({
+            }, Wt.createElement(qa.a, Object(Et.a)({
                 width: m
             }, g, {
                 getContainer: void 0 === p ? e : p,
                 prefixCls: a,
                 wrapClassName: d,
                 footer: void 0 === r ? b : r,
                 visible: s || c,
-                mousePosition: null != (t = g.mousePosition) ? t : Ra,
+                mousePosition: null != (t = g.mousePosition) ? t : Ya,
                 onClose: i,
                 closeIcon: f,
                 focusTriggerAfterClose: h,
-                transitionName: Object(Va.c)(n, "zoom", o.transitionName),
-                maskTransitionName: Object(Va.c)(n, "fade", o.maskTransitionName)
+                transitionName: Object(Ga.c)(n, "zoom", o.transitionName),
+                maskTransitionName: Object(Ga.c)(n, "fade", o.maskTransitionName)
             }))))
         }),
-        $a = [],
-        Za = "";
+        Qa = [],
+        tr = "";
 
-    function Ja(o) {
+    function er(o) {
         var e, c = document.createDocumentFragment(),
             r = Object(Et.a)(Object(Et.a)({}, o), {
                 close: l,
                 open: !0
             });
 
         function i(t) {
@@ -108738,22 +108819,22 @@
                     var n = {};
                     for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
                     if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                         for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
                     return n
                 }(t, ["okText", "cancelText", "prefixCls"]);
             clearTimeout(e), e = setTimeout(function() {
-                var t = Object(qa.b)(),
+                var t = Object(Za.b)(),
                     e = Object(W.b)(),
                     n = e.getPrefixCls,
                     e = e.getIconPrefixCls,
-                    n = n(void 0, Za),
+                    n = n(void 0, tr),
                     a = i || "".concat(n, "-modal"),
                     e = e();
-                Object(Ha.a)(Wt.createElement(Aa, Object(Et.a)({}, l, {
+                Object(Ka.a)(Wt.createElement(Na, Object(Et.a)({}, l, {
                     prefixCls: a,
                     rootPrefixCls: n,
                     iconPrefixCls: e,
                     okText: r || (l.okCancel ? t.okText : t.justOkText),
                     cancelText: o || t.cancelText
                 })), c)
             })
@@ -108767,76 +108848,76 @@
                     "function" == typeof o.afterClose && o.afterClose(),
                         function() {
                             for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
                             var a = e.some(function(t) {
                                 return t && t.triggerCancel
                             });
                             o.onCancel && a && o.onCancel.apply(o, [function() {}].concat(Object(Ut.a)(e.slice(1))));
-                            for (var r = 0; r < $a.length; r++)
-                                if ($a[r] === l) {
-                                    $a.splice(r, 1);
+                            for (var r = 0; r < Qa.length; r++)
+                                if (Qa[r] === l) {
+                                    Qa.splice(r, 1);
                                     break
-                                } Object(Ha.b)(c)
+                                } Object(Ka.b)(c)
                         }.apply(t, n)
                 }
             })).visible && delete r.visible, i(r)
         }
-        return i(r), $a.push(l), {
+        return i(r), Qa.push(l), {
             destroy: l,
             update: function(t) {
                 i(r = "function" == typeof t ? t(r) : Object(Et.a)(Object(Et.a)({}, r), t))
             }
         }
     }
 
-    function Qa(t) {
+    function nr(t) {
         return Object(Et.a)(Object(Et.a)({
-            icon: Wt.createElement(Ba.a, null),
+            icon: Wt.createElement(Wa.a, null),
             okCancel: !1
         }, t), {
             type: "warning"
         })
     }
 
-    function tr(t) {
+    function ar(t) {
         return Object(Et.a)(Object(Et.a)({
-            icon: Wt.createElement(Fa.a, null),
+            icon: Wt.createElement(Va.a, null),
             okCancel: !1
         }, t), {
             type: "info"
         })
     }
 
-    function er(t) {
+    function rr(t) {
         return Object(Et.a)(Object(Et.a)({
-            icon: Wt.createElement(Na.a, null),
+            icon: Wt.createElement(Fa.a, null),
             okCancel: !1
         }, t), {
             type: "success"
         })
     }
 
-    function nr(t) {
+    function or(t) {
         return Object(Et.a)(Object(Et.a)({
-            icon: Wt.createElement(Ya.a, null),
+            icon: Wt.createElement(Ha.a, null),
             okCancel: !1
         }, t), {
             type: "error"
         })
     }
 
-    function ar(t) {
+    function ir(t) {
         return Object(Et.a)(Object(Et.a)({
-            icon: Wt.createElement(Ba.a, null),
+            icon: Wt.createElement(Wa.a, null),
             okCancel: !0
         }, t), {
             type: "confirm"
         })
     }
-    var rr = Wt.forwardRef(function(t, e) {
+    var lr = Wt.forwardRef(function(t, e) {
             function n() {
                 i(!1);
                 for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
                 var a = e.some(function(t) {
                     return t && t.triggerCancel
                 });
                 l.onCancel && a && l.onCancel.apply(l, [function() {}].concat(Object(Ut.a)(e.slice(1))))
@@ -108861,33 +108942,33 @@
                     destroy: n,
                     update: function(e) {
                         c(function(t) {
                             return Object(Et.a)(Object(Et.a)({}, t), e)
                         })
                     }
                 }
-            }), Wt.createElement(ye.a, {
+            }), Wt.createElement(we.a, {
                 componentName: "Modal",
-                defaultLocale: xe.a.Modal
+                defaultLocale: ke.a.Modal
             }, function(t) {
-                return Wt.createElement(Aa, Object(Et.a)({
+                return Wt.createElement(Na, Object(Et.a)({
                     prefixCls: u,
                     rootPrefixCls: d
                 }, l, {
                     close: n,
                     open: o,
                     afterClose: a,
                     okText: l.okText || (l.okCancel ? t.okText : t.justOkText),
                     direction: s,
                     cancelText: l.cancelText || t.cancelText
                 }))
             })
         }),
-        or = 0,
-        ir = Wt.memo(Wt.forwardRef(function(t, e) {
+        cr = 0,
+        sr = Wt.memo(Wt.forwardRef(function(t, e) {
             a = Wt.useState([]), a = Object(Gt.a)(a, 2), r = a[0], n = a[1];
             var n, a = [r, Wt.useCallback(function(e) {
                     return n(function(t) {
                             return [].concat(Object(Ut.a)(t), [e])
                         }),
                         function() {
                             n(function(t) {
@@ -108903,19 +108984,19 @@
             return Wt.useImperativeHandle(e, function() {
                 return {
                     patchElement: o
                 }
             }, []), Wt.createElement(Wt.Fragment, null, a)
         }));
 
-    function lr(t) {
-        return Ja(Qa(t))
+    function ur(t) {
+        return er(nr(t))
     }
 
-    function cr(t) {
+    function dr(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.key,
             o = t.style,
             i = t.locale,
             l = t.setProps,
@@ -108944,15 +109025,15 @@
             L = t.confirmAutoSpin,
             P = t.transitionType,
             t = t.loading_state,
             D = Object(Wt.useContext)(G.a),
             i = D && D.locale || i;
         return H.a.createElement(W.a, {
             locale: K.b.get(i)
-        }, H.a.createElement(dr, {
+        }, H.a.createElement(hr, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: o,
             key: r,
             title: c,
             open: s,
             okText: S && h || f,
@@ -108994,44 +109075,44 @@
             footer: u ? void 0 : null,
             confirmLoading: S,
             destroyOnClose: !0,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n))
     }
 
-    function sr(e, n) {
+    function pr(e, n) {
         var a, r;
         return window.requestAnimationFrame || window.webkitRequestAnimationFrame || window.mozRequestAnimationFrame && window.mozCancelRequestAnimationFrame || window.oRequestAnimationFrame || window.msRequestAnimationFrame ? (a = (new Date).getTime(), (r = {
             value: 0
-        }).value = gr(function t() {
-            (new Date).getTime() - a >= n ? e.call(null) : r.value = gr(t)
+        }).value = yr(function t() {
+            (new Date).getTime() - a >= n ? e.call(null) : r.value = yr(t)
         }), r) : window.setTimeout(e, n)
     }
 
-    function ur(t) {
+    function fr(t) {
         window.cancelAnimationFrame ? window.cancelAnimationFrame(t.value) : window.webkitCancelAnimationFrame ? window.webkitCancelAnimationFrame(t.value) : window.webkitCancelRequestAnimationFrame ? window.webkitCancelRequestAnimationFrame(t.value) : window.mozCancelRequestAnimationFrame ? window.mozCancelRequestAnimationFrame(t.value) : window.oCancelRequestAnimationFrame ? window.oCancelRequestAnimationFrame(t.value) : window.msCancelRequestAnimationFrame ? window.msCancelRequestAnimationFrame(t.value) : clearTimeout(t)
     }
-    var u = Xa,
-        dr = (u.useModal = function() {
+    var u = Ja,
+        hr = (u.useModal = function() {
             var o = Wt.useRef(null),
                 t = Wt.useState([]),
                 t = Object(Gt.a)(t, 2),
                 e = t[0],
                 i = t[1],
                 n = (Wt.useEffect(function() {
                     e.length && (Object(Ut.a)(e).forEach(function(t) {
                         t()
                     }), i([]))
                 }, [e]), Wt.useCallback(function(r) {
                     return function(t) {
                         var e;
-                        or += 1;
+                        cr += 1;
                         var a = Wt.createRef(),
-                            t = Wt.createElement(rr, {
-                                key: "modal-".concat(or),
+                            t = Wt.createElement(lr, {
+                                key: "modal-".concat(cr),
                                 config: r(t),
                                 ref: a,
                                 afterClose: function() {
                                     null != n && n()
                                 }
                             }),
                             n = null == (e = o.current) ? void 0 : e.patchElement(t);
@@ -109055,41 +109136,41 @@
                                 })
                             }
                         }
                     }
                 }, []));
             return [Wt.useMemo(function() {
                 return {
-                    info: n(tr),
-                    success: n(er),
-                    error: n(nr),
-                    warning: n(Qa),
-                    confirm: n(ar)
+                    info: n(ar),
+                    success: n(rr),
+                    error: n(or),
+                    warning: n(nr),
+                    confirm: n(ir)
                 }
-            }, []), Wt.createElement(ir, {
+            }, []), Wt.createElement(sr, {
                 ref: o
             })]
         }, u.info = function(t) {
-            return Ja(tr(t))
+            return er(ar(t))
         }, u.success = function(t) {
-            return Ja(er(t))
+            return er(rr(t))
         }, u.error = function(t) {
-            return Ja(nr(t))
-        }, u.warning = lr, u.warn = lr, u.confirm = function(t) {
-            return Ja(ar(t))
+            return er(or(t))
+        }, u.warning = ur, u.warn = ur, u.confirm = function(t) {
+            return er(ir(t))
         }, u.destroyAll = function() {
-            for (; $a.length;) {
-                var t = $a.pop();
+            for (; Qa.length;) {
+                var t = Qa.pop();
                 t && t()
             }
         }, u.config = function(t) {
             t = t.rootPrefixCls;
-            Za = t
+            tr = t
         }, u),
-        pr = (cr.propTypes = {
+        mr = (dr.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             locale: n.a.oneOf(["zh-cn", "en-us"]),
             visible: n.a.bool,
@@ -109130,15 +109211,15 @@
             transitionType: n.a.oneOf(["none", "fade", "zoom", "zoom-big", "zoom-big-fast", "slide-up", "slide-down", "slide-left", "slide-right", "move-up", "move-down", "move-left", "move-right"]),
             setProps: n.a.func,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             })
-        }, cr.defaultProps = {
+        }, dr.defaultProps = {
             visible: !1,
             renderFooter: !1,
             width: 520,
             centered: !1,
             keyboard: !0,
             closable: !0,
             mask: !0,
@@ -109148,78 +109229,78 @@
             okCounts: 0,
             cancelCounts: 0,
             closeCounts: 0,
             confirmLoading: !1,
             confirmAutoSpin: !1,
             transitionType: "zoom",
             locale: "zh-cn"
-        }, cr),
-        fr = e(199),
+        }, dr),
+        gr = e(199),
         d = e(306),
-        hr = e.n(d),
+        br = e.n(d),
         c = e(518),
-        mr = e.n(c),
-        gr = "undefined" != typeof window ? window.requestAnimationFrame || window.webkitRequestAnimationFrame || window.mozRequestAnimationFrame || window.oRequestAnimationFrame || window.msRequestAnimationFrame || function(t) {
+        vr = e.n(c),
+        yr = "undefined" != typeof window ? window.requestAnimationFrame || window.webkitRequestAnimationFrame || window.mozRequestAnimationFrame || window.oRequestAnimationFrame || window.msRequestAnimationFrame || function(t) {
             window.setTimeout(t, 1e3 / 60)
         } : function() {};
 
-    function br() {
-        return (br = Object.assign || function(t) {
+    function xr() {
+        return (xr = Object.assign || function(t) {
             for (var e = 1; e < arguments.length; e++) {
                 var n, a = arguments[e];
                 for (n in a) Object.prototype.hasOwnProperty.call(a, n) && (t[n] = a[n])
             }
             return t
         }).apply(this, arguments)
     }
 
-    function vr(t) {
+    function _r(t) {
         if (void 0 === t) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
         return t
     }
 
-    function yr(t, e, n) {
+    function Or(t, e, n) {
         e in t ? Object.defineProperty(t, e, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : t[e] = n
     }
-    xr = H.a.PureComponent, u = xr, (d = _r).prototype = Object.create(u.prototype), (d.prototype.constructor = d).__proto__ = u, (d = _r.prototype).componentDidMount = function() {
+    wr = H.a.PureComponent, u = wr, (d = kr).prototype = Object.create(u.prototype), (d.prototype.constructor = d).__proto__ = u, (d = kr.prototype).componentDidMount = function() {
         var t = this,
             e = this.props.delay,
             n = this.state,
             a = n.currentInterval,
             n = n.elements;
-        0 < a && 1 < n.length && (this.tickDelay = sr(function() {
-            t.tickLoop = sr(t.tick, a)
+        0 < a && 1 < n.length && (this.tickDelay = pr(function() {
+            t.tickLoop = pr(t.tick, a)
         }, e))
     }, d.componentDidUpdate = function(t, e) {
         var n = this,
             a = this.props,
             r = a.interval,
             o = a.children,
             a = a.delay,
             i = this.state.currentWordIndex,
             l = Array.isArray(r) ? r[i % r.length] : r;
-        e.currentInterval !== l && (this.clearTimeouts(), 0 < l && 1 < H.a.Children.count(o) ? this.tickDelay = sr(function() {
-            n.tickLoop = sr(n.tick, l)
+        e.currentInterval !== l && (this.clearTimeouts(), 0 < l && 1 < H.a.Children.count(o) ? this.tickDelay = pr(function() {
+            n.tickLoop = pr(n.tick, l)
         }, a) : this.setState(function(t, e) {
             t = t.currentWordIndex;
             return {
                 currentInterval: Array.isArray(e.interval) ? e.interval[t % e.interval.length] : e.interval
             }
-        })), mr()(t.children, o) || this.setState({
+        })), vr()(t.children, o) || this.setState({
             elements: H.a.Children.toArray(o)
         })
     }, d.componentWillUnmount = function() {
         this.isUnMounting = !0, this.clearTimeouts()
     }, d.clearTimeouts = function() {
-        null != this.tickLoop && ur(this.tickLoop), null != this.tickDelay && ur(this.tickDelay)
+        null != this.tickLoop && fr(this.tickLoop), null != this.tickDelay && fr(this.tickDelay)
     }, d.getOpacity = function() {
         return this.props.fade ? 0 : 1
     }, d.getDimensions = function() {
         return null == this.wordBox ? {
             width: 0,
             height: 0
         } : this.wordBox.getBoundingClientRect()
@@ -109228,83 +109309,83 @@
             e = this.state;
         return [{
             key: "step-" + e.wordCount,
             data: {
                 currentEl: e.currentEl
             },
             style: {
-                opacity: Object(fr.spring)(1, t),
-                translate: Object(fr.spring)(0, t)
+                opacity: Object(gr.spring)(1, t),
+                translate: Object(gr.spring)(0, t)
             }
         }]
     };
-    var xr, c = _r;
+    var wr, c = kr;
 
-    function _r(t) {
-        yr(vr(e = xr.call(this, t) || this), "isUnMounting", !1), yr(vr(e), "tickDelay", 0), yr(vr(e), "tickLoop", 0), yr(vr(e), "wordBox", null), yr(vr(e), "willLeave", function() {
+    function kr(t) {
+        Or(_r(e = wr.call(this, t) || this), "isUnMounting", !1), Or(_r(e), "tickDelay", 0), Or(_r(e), "tickLoop", 0), Or(_r(e), "wordBox", null), Or(_r(e), "willLeave", function() {
             var t = e.getDimensions().height;
             return {
-                opacity: Object(fr.spring)(e.getOpacity(), e.props.springConfig),
-                translate: Object(fr.spring)(-t, e.props.springConfig)
+                opacity: Object(gr.spring)(e.getOpacity(), e.props.springConfig),
+                translate: Object(gr.spring)(-t, e.props.springConfig)
             }
-        }), yr(vr(e), "willEnter", function() {
+        }), Or(_r(e), "willEnter", function() {
             var t = e.getDimensions().height;
             return {
                 opacity: e.getOpacity(),
                 translate: t
             }
-        }), yr(vr(e), "tick", function() {
+        }), Or(_r(e), "tick", function() {
             e.isUnMounting || e.setState(function(t, e) {
                 var n = (t.currentWordIndex + 1) % t.elements.length,
                     t = {
                         currentWordIndex: n,
                         currentEl: t.elements[n],
                         wordCount: (t.wordCount + 1) % 1e3,
                         currentInterval: Array.isArray(e.interval) ? e.interval[n % e.interval.length] : e.interval
                     };
                 return e.onChange && e.onChange(t), t
             }, function() {
-                0 < e.state.currentInterval && (e.clearTimeouts(), e.tickLoop = sr(e.tick, e.state.currentInterval))
+                0 < e.state.currentInterval && (e.clearTimeouts(), e.tickLoop = pr(e.tick, e.state.currentInterval))
             })
-        }), yr(vr(e), "wrapperStyles", hr()(br({}, e.props.mask && {
+        }), Or(_r(e), "wrapperStyles", br()(xr({}, e.props.mask && {
             overflow: "hidden"
         }, {}, {
             display: "inline-block",
             position: "relative",
             verticalAlign: "top"
-        }))), yr(vr(e), "elementStyles", hr()({
+        }))), Or(_r(e), "elementStyles", br()({
             display: "inline-block",
             left: 0,
             top: 0,
             whiteSpace: e.props.noWrap ? "nowrap" : "normal"
         }));
         var e, n = H.a.Children.toArray(t.children);
         return e.state = {
             elements: n,
             currentEl: n[0],
             currentWordIndex: 0,
             wordCount: 0,
             currentInterval: Array.isArray(t.interval) ? t.interval[0] : t.interval
         }, e
     }
-    yr(c, "defaultProps", {
+    Or(c, "defaultProps", {
         interval: 3e3,
         delay: 0,
         adjustingSpeed: 150,
         springConfig: {
             stiffness: 340,
             damping: 30
         },
         fade: !0,
         mask: !(d.render = function() {
             var a = this,
                 t = this.props.className;
             return H.a.createElement("div", {
                 className: this.wrapperStyles + " " + (void 0 === t ? "" : t)
-            }, H.a.createElement(fr.TransitionMotion, {
+            }, H.a.createElement(gr.TransitionMotion, {
                 willLeave: this.willLeave,
                 willEnter: this.willEnter,
                 styles: this.getTransitionMotionStyles()
             }, function(t) {
                 var e = a.getDimensions(),
                     n = e.height,
                     e = e.width,
@@ -109331,32 +109412,32 @@
                     }, t.data.currentEl)
                 }))
             }))
         }),
         noWrap: !0
     });
 
-    function Or(t) {
+    function jr(t) {
         var e = t.description,
             n = t.icon,
             a = t.prefixCls,
             t = t.type,
-            e = (e ? Lr : Sr)[t] || null;
-        return n ? Object(je.d)(n, Wt.createElement("span", {
+            e = (e ? Tr : Dr)[t] || null;
+        return n ? Object(Ce.d)(n, Wt.createElement("span", {
             className: "".concat(a, "-icon")
         }, n), function() {
             return {
                 className: Kt()("".concat(a, "-icon"), Object(Vt.a)({}, n.props.className, n.props.className))
             }
         }) : Wt.createElement(e, {
             className: "".concat(a, "-icon")
         })
     }
 
-    function wr(t) {
+    function Mr(t) {
         var e = t.isClosable,
             n = t.closeText,
             a = t.prefixCls,
             r = t.closeIcon,
             t = t.handleClose;
         return e ? Wt.createElement("button", {
             type: "button",
@@ -109364,15 +109445,15 @@
             className: "".concat(a, "-close-icon"),
             tabIndex: 0
         }, n ? Wt.createElement("span", {
             className: "".concat(a, "-close-text")
         }, n) : r) : null
     }
 
-    function kr(t) {
+    function Er(t) {
         function n(t) {
             var e;
             x(!0), null != (e = b.onClose) && e.call(b, t)
         }
         var a = t.description,
             e = t.prefixCls,
             r = t.message,
@@ -109382,15 +109463,15 @@
             c = t.onMouseEnter,
             s = t.onMouseLeave,
             u = t.onClick,
             d = t.afterClose,
             p = t.showIcon,
             f = t.closable,
             h = t.closeText,
-            m = void 0 === (v = t.closeIcon) ? Wt.createElement(Ze.a, null) : v,
+            m = void 0 === (v = t.closeIcon) ? Wt.createElement(tn.a, null) : v,
             g = t.action,
             b = function(t, e) {
                 var n = {};
                 for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
                 if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                     for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
                 return n
@@ -109402,16 +109483,16 @@
             t = (v = Wt.useContext(q.b)).getPrefixCls,
             v = v.direction,
             O = t("alert", e),
             w = !!h || f,
             k = void 0 !== (t = b.type) ? t : o ? "warning" : "info",
             j = !(!o || void 0 !== p) || p,
             M = Kt()(O, "".concat(O, "-").concat(k), (e = {}, Object(Vt.a)(e, "".concat(O, "-with-description"), !!a), Object(Vt.a)(e, "".concat(O, "-no-icon"), !j), Object(Vt.a)(e, "".concat(O, "-banner"), !!o), Object(Vt.a)(e, "".concat(O, "-rtl"), "rtl" === v), e), i),
-            E = Object(Cr.a)(b);
-        return Wt.createElement(Er.b, {
+            E = Object(Pr.a)(b);
+        return Wt.createElement(Lr.b, {
             visible: !y,
             motionName: "".concat(O, "-motion"),
             motionAppear: !1,
             motionEnter: !1,
             onLeaveStart: function(t) {
                 return {
                     maxHeight: t.offsetHeight
@@ -109426,42 +109507,42 @@
                 "data-show": !y,
                 className: Kt()(M, e),
                 style: Object(Et.a)(Object(Et.a)({}, l), t),
                 onMouseEnter: c,
                 onMouseLeave: s,
                 onClick: u,
                 role: "alert"
-            }, E), j ? Wt.createElement(Or, {
+            }, E), j ? Wt.createElement(jr, {
                 description: a,
                 icon: b.icon,
                 prefixCls: O,
                 type: k
             }) : null, Wt.createElement("div", {
                 className: "".concat(O, "-content")
             }, r ? Wt.createElement("div", {
                 className: "".concat(O, "-message")
             }, r) : null, a ? Wt.createElement("div", {
                 className: "".concat(O, "-description")
             }, a) : null), g ? Wt.createElement("div", {
                 className: "".concat(O, "-action")
-            }, g) : null, Wt.createElement(wr, {
+            }, g) : null, Wt.createElement(Mr, {
                 isClosable: !!w,
                 closeText: h,
                 prefixCls: O,
                 closeIcon: m,
                 handleClose: n
             }))
         })
     }
-    var jr, Mr = c,
+    var Cr, Sr = c,
         u = e(122),
         d = e(280),
-        Er = e(44),
-        Cr = e(269),
-        c = (c = Wt.Component, Object(r.a)(Pr, c), jr = Object(o.a)(Pr), Object(a.a)(Pr, [{
+        Lr = e(44),
+        Pr = e(269),
+        c = (c = Wt.Component, Object(r.a)(zr, c), Cr = Object(o.a)(zr), Object(a.a)(zr, [{
             key: "componentDidCatch",
             value: function(t, e) {
                 this.setState({
                     error: t,
                     info: e
                 })
             }
@@ -109473,95 +109554,95 @@
                     n = t.description,
                     t = t.children,
                     a = this.state,
                     r = a.error,
                     a = a.info,
                     a = a && a.componentStack ? a.componentStack : null,
                     e = void 0 === e ? (r || "").toString() : e;
-                return r ? Wt.createElement(Kr, {
+                return r ? Wt.createElement(qr, {
                     type: "error",
                     message: e,
                     description: Wt.createElement("pre", null, void 0 === n ? a : n)
                 }) : t
             }
-        }]), Pr),
-        Sr = {
-            success: un.a,
+        }]), zr),
+        Dr = {
+            success: fn.a,
             info: d.a,
-            error: dn.a,
+            error: hn.a,
             warning: u.a
         },
-        Lr = {
-            success: Na.a,
-            info: Fa.a,
-            error: Ya.a,
-            warning: Ba.a
+        Tr = {
+            success: Fa.a,
+            info: Va.a,
+            error: Ha.a,
+            warning: Wa.a
         };
 
-    function Pr() {
+    function zr() {
         var t;
-        return Object(i.a)(this, Pr), (t = jr.apply(this, arguments)).state = {
+        return Object(i.a)(this, zr), (t = Cr.apply(this, arguments)).state = {
             error: void 0,
             info: {
                 componentStack: ""
             }
         }, t
     }
-    kr.ErrorBoundary = c;
+    Er.ErrorBoundary = c;
 
-    function Dr(t) {
+    function Ar(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.type,
             i = t.showIcon,
             l = t.closable,
             c = t.message,
             s = t.messageRenderMode,
             u = t.description,
             d = t.action,
             p = t.banner,
             t = (t.setProps, t.loading_state);
-        return "loop-text" === s && Array.isArray(c) ? H.a.createElement(Kr, {
+        return "loop-text" === s && Array.isArray(c) ? H.a.createElement(qr, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
-            message: H.a.createElement(Mr, {
+            message: H.a.createElement(Sr, {
                 mask: !0
             }, c.map(function(t) {
                 return H.a.createElement("div", null, t)
             })),
             type: o,
             description: u,
             showIcon: i,
             closable: l,
             action: d,
             banner: p,
             "data-dash-is-loading": t && t.is_loading || void 0
-        }) : H.a.createElement(Kr, {
+        }) : H.a.createElement(qr, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
-            message: "marquee" === s ? H.a.createElement(Ur.a, {
+            message: "marquee" === s ? H.a.createElement(Xr.a, {
                 pauseOnHover: !0,
                 gradient: !1
             }, c) : c,
             type: o,
             description: u,
             showIcon: i,
             closable: l,
             action: d,
             banner: p
         })
     }
 
-    function Tr(t) {
+    function Rr(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.message,
             i = t.description,
             l = t.type,
@@ -109583,23 +109664,23 @@
                 closeIcon: p ? void 0 : H.a.createElement("span", {
                     style: {
                         visibility: "hidden"
                     }
                 })
             });
         return Object(Wt.useEffect)(function() {
-            "default" === l ? qr.a.open(h) : "success" === l ? qr.a.success(h) : "error" === l ? qr.a.error(h) : "info" === l ? qr.a.info(h) : "warning" === l && qr.a.warning(h)
+            "default" === l ? Zr.a.open(h) : "success" === l ? Zr.a.success(h) : "error" === l ? Zr.a.error(h) : "info" === l ? Zr.a.info(h) : "warning" === l && Zr.a.warning(h)
         }), H.a.createElement("div", {
             id: e,
             key: r,
             "data-dash-is-loading": f && f.is_loading || void 0
         })
     }
 
-    function zr(t) {
+    function Ir(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.content,
             i = t.type,
             l = t.duration,
@@ -109628,64 +109709,64 @@
         }), H.a.createElement("div", {
             id: e,
             key: r,
             "data-dash-is-loading": d && d.is_loading || void 0
         })
     }
 
-    function Ar(t) {
+    function Nr(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.content,
             i = t.color,
             l = t.href,
             c = t.target,
             t = (t.setProps, t.loading_state);
-        return H.a.createElement(Zr.a, {
+        return H.a.createElement(to.a, {
             id: e,
             key: r,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             color: i,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, l ? H.a.createElement("a", {
             href: l,
             target: c
         }, o) : o)
     }
 
-    function Rr(t, e) {
-        return Wt.createElement(to.a, Object(Ct.a)(Object(Ct.a)({}, t), {}, {
+    function Yr(t, e) {
+        return Wt.createElement(ao.a, Object(Ct.a)(Object(Ct.a)({}, t), {}, {
             ref: e,
-            icon: Qr
+            icon: no
         }))
     }
 
-    function Ir(t) {
+    function Br(t) {
         var e, n = t.prefixCls,
             a = t.icon,
             t = t.status,
             r = Kt()("".concat(n, "-icon"));
-        return ao.includes("".concat(t)) ? (e = no[t], Wt.createElement("div", {
+        return io.includes("".concat(t)) ? (e = oo[t], Wt.createElement("div", {
             className: "".concat(r, " ").concat(n, "-image")
-        }, Wt.createElement(e, null))) : (n = Wt.createElement(eo[t]), null === a || !1 === a ? null : Wt.createElement("div", {
+        }, Wt.createElement(e, null))) : (n = Wt.createElement(ro[t]), null === a || !1 === a ? null : Wt.createElement("div", {
             className: r
         }, a || n))
     }
 
-    function Nr(t) {
+    function Fr(t) {
         var e = t.prefixCls;
         return (t = t.extra) ? Wt.createElement("div", {
             className: "".concat(e, "-extra")
         }, t) : null
     }
 
-    function Yr(t) {
+    function Hr(t) {
         var e = t.prefixCls,
             n = t.className,
             a = t.subTitle,
             r = t.title,
             o = t.style,
             i = t.children,
             l = void 0 === (l = t.status) ? "info" : l,
@@ -109694,61 +109775,61 @@
             s = (u = Wt.useContext(q.b)).getPrefixCls,
             u = u.direction,
             s = s("result", e),
             e = Kt()(s, "".concat(s, "-").concat(l), n, Object(Vt.a)({}, "".concat(s, "-rtl"), "rtl" === u));
         return Wt.createElement("div", {
             className: e,
             style: o
-        }, Wt.createElement(Ir, {
+        }, Wt.createElement(Br, {
             prefixCls: s,
             status: l,
             icon: c
         }), Wt.createElement("div", {
             className: "".concat(s, "-title")
         }, r), a && Wt.createElement("div", {
             className: "".concat(s, "-subtitle")
-        }, a), Wt.createElement(Nr, {
+        }, a), Wt.createElement(Fr, {
             prefixCls: s,
             extra: t
         }), i && Wt.createElement("div", {
             className: "".concat(s, "-content")
         }, i))
     }
 
-    function Br(t) {
+    function Wr(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.status,
             i = t.title,
             l = t.subTitle,
             c = t.icon,
             s = t.loading_state;
-        return t.setProps, H.a.createElement(ro, {
+        return t.setProps, H.a.createElement(lo, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
-            icon: c || ("loading" === o ? H.a.createElement(oo.a, {
+            icon: c || ("loading" === o ? H.a.createElement(co.a, {
                 style: {
                     color: "#1890ff"
                 }
             }) : void 0),
             status: o,
             title: i,
             subTitle: l,
             "data-dash-is-loading": s && s.is_loading || void 0
         })
     }
 
-    function Fr(t) {
+    function Vr(t) {
         function e(t) {
             S(c && "password" === l ? {
-                md5Value: lo()(t.target.value),
+                md5Value: uo()(t.target.value),
                 value: t.target.value
             } : {
                 value: t.target.value
             })
         }
 
         function n(t) {
@@ -109787,27 +109868,27 @@
             P = t.persistence,
             D = t.persisted_props,
             t = t.persistence_type,
             T = Object(Wt.useContext)(G.a),
             z = (Object(Wt.useEffect)(function() {
                 y && !d && S({
                     value: y,
-                    md5Value: lo()(y)
+                    md5Value: uo()(y)
                 }), d && S({
-                    md5Value: lo()(d)
+                    md5Value: uo()(d)
                 })
             }, []), Object(Z.a)(function(t) {
                 S({
                     debounceValue: t
                 })
             }, {
                 debounceWait: Math.max(E, 200),
                 manual: !0
             }).run);
-        return "default" === l ? React.createElement(Ae.a, {
+        return "default" === l ? React.createElement(Ne.a, {
             id: a,
             className: Object(V.isString)(r) ? r : r ? Object(U.a)(r) : void 0,
             style: o,
             key: i,
             placeholder: u,
             autoComplete: s,
             value: d,
@@ -109827,15 +109908,15 @@
                 e(t), z(t.target.value)
             },
             onPressEnter: n,
             persistence: P,
             persisted_props: D,
             persistence_type: t,
             "data-dash-is-loading": L && L.is_loading || void 0
-        }) : "search" === l ? React.createElement(co, {
+        }) : "search" === l ? React.createElement(po, {
             id: a,
             className: Object(V.isString)(r) ? r : r ? Object(U.a)(r) : void 0,
             style: o,
             key: i,
             placeholder: u,
             autoComplete: s,
             size: T && !Object(V.isUndefined)(T.componentSize) ? T.componentSize : p,
@@ -109856,15 +109937,15 @@
                 e(t), z(t.target.value)
             },
             onPressEnter: n,
             persistence: P,
             persisted_props: D,
             persistence_type: t,
             "data-dash-is-loading": L && L.is_loading || void 0
-        }) : "text-area" === l ? React.createElement(so, {
+        }) : "text-area" === l ? React.createElement(fo, {
             id: a,
             className: Object(V.isString)(r) ? r : r ? Object(U.a)(r) : void 0,
             style: o,
             key: i,
             placeholder: u,
             autoComplete: s,
             size: T && !Object(V.isUndefined)(T.componentSize) ? T.componentSize : p,
@@ -109882,15 +109963,15 @@
                 e(t), z(t.target.value)
             },
             onPressEnter: n,
             persistence: P,
             persisted_props: D,
             persistence_type: t,
             "data-dash-is-loading": L && L.is_loading || void 0
-        }) : "password" === l ? React.createElement(Ae.a.Password, {
+        }) : "password" === l ? React.createElement(Ne.a.Password, {
             id: a,
             className: Object(V.isString)(r) ? r : r ? Object(U.a)(r) : void 0,
             style: o,
             key: i,
             placeholder: u,
             autoComplete: s,
             size: T && !Object(V.isUndefined)(T.componentSize) ? T.componentSize : p,
@@ -109910,15 +109991,15 @@
             persistence: P,
             persisted_props: D,
             persistence_type: t,
             "data-dash-is-loading": L && L.is_loading || void 0
         }) : void 0
     }
 
-    function Hr(t) {
+    function Kr(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.title,
             l = t.placement,
@@ -109962,30 +110043,30 @@
             getPopupContainer: "parent" === y ? function(t) {
                 return t.parentNode
             } : void 0,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
 
-    function Wr(t) {
+    function Ur(t) {
         var e = t.id,
             n = t.style,
             a = t.className,
             r = t.key,
             o = t.label,
             i = t.disabled,
             l = t.checked,
             c = t.indeterminate,
             s = t.setProps,
             u = t.persistence,
             d = t.persisted_props,
             p = t.persistence_type,
             t = t.loading_state,
             f = Object(Wt.useContext)(G.a);
-        return H.a.createElement(we.a, {
+        return H.a.createElement(Ee.a, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: n,
             key: r,
             onChange: function(t) {
                 s({
                     checked: t.target.checked
@@ -109997,29 +110078,29 @@
             persistence: u,
             persisted_props: d,
             persistence_type: p,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, o)
     }
 
-    function Vr(t) {
+    function Gr(t) {
         var e = t.id,
             n = t.style,
             a = t.className,
             r = t.key,
             o = t.options,
             i = t.value,
             l = t.disabled,
             c = t.setProps,
             s = t.persistence,
             u = t.persisted_props,
             d = t.persistence_type,
             t = t.loading_state,
             p = Object(Wt.useContext)(G.a);
-        return H.a.createElement(we.a.Group, {
+        return H.a.createElement(Ee.a.Group, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: n,
             key: r,
             options: o,
             value: i,
             disabled: p && !Object(V.isUndefined)(p.componentDisabled) ? p.componentDisabled : l,
@@ -110030,18 +110111,18 @@
             },
             persistence: s,
             persisted_props: u,
             persistence_type: d,
             "data-dash-is-loading": t && t.is_loading || void 0
         })
     }
-    var Kr = kr,
+    var qr = Er,
         d = e(517),
-        Ur = e.n(d),
-        Gr = (Dr.propTypes = {
+        Xr = e.n(d),
+        $r = (Ar.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             message: n.a.node,
             description: n.a.node,
             type: n.a.oneOf(["success", "info", "warning", "error"]),
@@ -110052,23 +110133,23 @@
             banner: n.a.bool,
             setProps: n.a.func,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             })
-        }, Dr.defaultProps = {
+        }, Ar.defaultProps = {
             type: "info",
             showIcon: !1,
             closable: !1,
             messageRenderMode: "default",
             banner: !1
-        }, Dr),
-        qr = e(524),
-        Xr = (Tr.propTypes = {
+        }, Ar),
+        Zr = e(524),
+        Jr = (Rr.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             message: n.a.string,
             description: n.a.string,
             type: n.a.oneOf(["default", "success", "error", "info", "warning"]),
@@ -110079,24 +110160,24 @@
             closable: n.a.bool,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, Tr.defaultProps = {
+        }, Rr.defaultProps = {
             type: "default",
             placement: "topRight",
             top: 24,
             bottom: 24,
             duration: 4.5,
             closable: !0
-        }, Tr),
+        }, Rr),
         $ = e(308),
-        $r = (zr.propTypes = {
+        Qr = (Ir.propTypes = {
             id: n.a.string,
             className: n.a.string,
             style: n.a.object,
             key: n.a.string,
             content: n.a.string,
             type: n.a.oneOf(["default", "success", "error", "info", "warning"]),
             duration: n.a.number,
@@ -110105,39 +110186,39 @@
             icon: n.a.string,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, zr.defaultProps = {
+        }, Ir.defaultProps = {
             type: "default",
             duration: 3,
             top: 8
-        }, zr),
-        Zr = e(309),
-        Jr = (Ar.propTypes = {
+        }, Ir),
+        to = e(309),
+        eo = (Nr.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             content: n.a.node,
             color: n.a.string,
             href: n.a.string,
             target: n.a.string,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, Ar.defaultProps = {
+        }, Nr.defaultProps = {
             target: "_blank"
-        }, Ar),
-        Qr = {
+        }, Nr),
+        no = {
             icon: {
                 tag: "svg",
                 attrs: {
                     viewBox: "64 64 896 896",
                     focusable: "false"
                 },
                 children: [{
@@ -110146,23 +110227,23 @@
                         d: "M955.7 856l-416-720c-6.2-10.7-16.9-16-27.7-16s-21.6 5.3-27.7 16l-416 720C56 877.4 71.4 904 96 904h832c24.6 0 40-26.6 27.7-48zM480 416c0-4.4 3.6-8 8-8h48c4.4 0 8 3.6 8 8v184c0 4.4-3.6 8-8 8h-48c-4.4 0-8-3.6-8-8V416zm32 352a48.01 48.01 0 010-96 48.01 48.01 0 010 96z"
                     }
                 }]
             },
             name: "warning",
             theme: "filled"
         },
-        to = e(9),
-        c = (Rr.displayName = "WarningFilled", Wt.forwardRef(Rr)),
-        eo = {
-            success: un.a,
-            error: dn.a,
+        ao = e(9),
+        c = (Yr.displayName = "WarningFilled", Wt.forwardRef(Yr)),
+        ro = {
+            success: fn.a,
+            error: hn.a,
             info: u.a,
             warning: c
         },
-        no = {
+        oo = {
             404: function() {
                 return Wt.createElement("svg", {
                     width: "252",
                     height: "294"
                 }, Wt.createElement("defs", null, Wt.createElement("path", {
                     d: "M0 .387h251.772v251.772H0z"
                 })), Wt.createElement("g", {
@@ -110891,40 +110972,40 @@
                     stroke: "#648BD8",
                     strokeWidth: "1.051",
                     strokeLinecap: "round",
                     strokeLinejoin: "round"
                 })))
             }
         },
-        ao = Object.keys(no),
-        ro = (Yr.PRESENTED_IMAGE_403 = no[403], Yr.PRESENTED_IMAGE_404 = no[404], Yr.PRESENTED_IMAGE_500 = no[500], Yr),
-        oo = e(77),
-        io = (Br.propTypes = {
+        io = Object.keys(oo),
+        lo = (Hr.PRESENTED_IMAGE_403 = oo[403], Hr.PRESENTED_IMAGE_404 = oo[404], Hr.PRESENTED_IMAGE_500 = oo[500], Hr),
+        co = e(77),
+        so = (Wr.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             status: n.a.oneOf(["success", "error", "info", "warning", "404", "403", "500", "loading"]),
             title: n.a.node,
             subTitle: n.a.node,
             icon: n.a.node,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, Br.defaultProps = {
+        }, Wr.defaultProps = {
             status: "info"
-        }, Br),
+        }, Wr),
         d = e(287),
-        lo = e.n(d),
-        co = Ae.a.Search,
-        so = Ae.a.TextArea,
-        uo = (Fr.propTypes = {
+        uo = e.n(d),
+        po = Ne.a.Search,
+        fo = Ne.a.TextArea,
+        ho = (Vr.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             mode: n.a.oneOf(["default", "search", "text-area", "password"]),
             autoComplete: n.a.oneOf(["off", "on"]),
             disabled: n.a.bool,
@@ -110957,31 +111038,31 @@
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func,
             persistence: n.a.oneOfType([n.a.bool, n.a.string, n.a.number]),
             persisted_props: n.a.arrayOf(n.a.oneOf(["value", "md5Value"])),
             persistence_type: n.a.oneOf(["local", "session", "memory"])
-        }, Fr.defaultProps = {
+        }, Vr.defaultProps = {
             mode: "default",
             autoComplete: "on",
             disabled: !1,
             size: "middle",
             bordered: !0,
             showCount: !1,
             passwordUseMd5: !1,
             autoSize: !1,
             nClicksSearch: 0,
             nSubmit: 0,
             allowClear: !1,
             debounceWait: 200,
             persisted_props: ["value", "md5Value"],
             persistence_type: "local"
-        }, Fr),
-        po = (Hr.propTypes = {
+        }, Vr),
+        mo = (Kr.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             title: n.a.node,
             placement: n.a.oneOf(["top", "left", "right", "bottom", "topLeft", "topRight", "bottomLeft", "bottomRight"]),
@@ -110999,25 +111080,25 @@
             popupContainer: n.a.oneOf(["parent", "body"]),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, Hr.defaultProps = {
+        }, Kr.defaultProps = {
             mouseEnterDelay: .1,
             mouseLeaveDelay: .1,
             placement: "top",
             trigger: "hover",
             popupContainer: "body",
             arrowPointAtCenter: !1,
             open: !1,
             permanent: !1
-        }, Hr),
-        fo = (Wr.propTypes = {
+        }, Kr),
+        go = (Ur.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             disabled: n.a.bool,
             label: n.a.node,
             checked: n.a.bool,
@@ -111027,22 +111108,22 @@
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func,
             persistence: n.a.oneOfType([n.a.bool, n.a.string, n.a.number]),
             persisted_props: n.a.arrayOf(n.a.oneOf(["checked"])),
             persistence_type: n.a.oneOf(["local", "session", "memory"])
-        }, Wr.defaultProps = {
+        }, Ur.defaultProps = {
             persisted_props: ["checked"],
             persistence_type: "local",
             disabled: !1,
             checked: !1,
             indeterminate: !1
-        }, Wr),
-        ho = (Vr.propTypes = {
+        }, Ur),
+        bo = (Gr.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             disabled: n.a.bool,
             options: n.a.arrayOf(n.a.exact({
                 label: n.a.node,
@@ -111055,27 +111136,27 @@
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func,
             persistence: n.a.oneOfType([n.a.bool, n.a.string, n.a.number]),
             persisted_props: n.a.arrayOf(n.a.oneOf(["value"])),
             persistence_type: n.a.oneOf(["local", "session", "memory"])
-        }, Vr.defaultProps = {
+        }, Gr.defaultProps = {
             persisted_props: ["value"],
             persistence_type: "local",
             disabled: !1
-        }, Vr);
+        }, Gr);
 
-    function mo(t, e) {
+    function vo(t, e) {
         (null == e || e > t.length) && (e = t.length);
         for (var n = 0, a = new Array(e); n < e; n++) a[n] = t[n];
         return a
     }
 
-    function go(t) {
+    function yo(t) {
         var e = t.id,
             n = t.className,
             a = t.wrapperClassName,
             r = t.style,
             o = t.key,
             i = t.children,
             l = t.spinning,
@@ -111112,15 +111193,15 @@
                             if (s) throw r
                         }
                     }
                     return l
                 }
             }(t, l) || function(t, e) {
                 var n;
-                if (t) return "string" == typeof t ? mo(t, e) : "Map" === (n = "Object" === (n = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : n) || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? mo(t, e) : void 0
+                if (t) return "string" == typeof t ? vo(t, e) : "Map" === (n = "Object" === (n = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : n) || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? vo(t, e) : void 0
             }(t, l) || function() {
                 throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
             }())[0],
             v = t[1],
             y = Object(Wt.useRef)();
         return Object(Wt.useEffect)(function() {
             u && (y.current && clearTimeout(y.current), u.is_loading && !b ? "default" === p ? (m && console.log(u.component_name + "." + u.prop_name), v(!0)) : "exclude" === p ? -1 === f.indexOf(u.component_name + "." + u.prop_name) && (m && console.log(u.component_name + "." + u.prop_name), v(!0)) : "include" === p && -1 !== h.indexOf(u.component_name + "." + u.prop_name) && (m && console.log(u.component_name + "." + u.prop_name), v(!0)) : !u.is_loading && b && (y.current = setTimeout(function() {
@@ -111137,15 +111218,15 @@
             delay: s,
             tip: d,
             indicator: g,
             "data-dash-is-loading": u && u.is_loading || void 0
         }, " ", i, " ")
     }
 
-    function bo(t) {
+    function xo(t) {
         var e = t.id,
             n = t.style,
             a = t.className,
             r = t.key,
             o = t.disabled,
             i = t.checked,
             l = t.checkedChildren,
@@ -111158,15 +111239,15 @@
             h = t.persistence_type,
             t = t.loading_state,
             m = Object(Wt.useContext)(G.a);
         return Object(Wt.useEffect)(function() {
             Object(V.isUndefined)(i) && d({
                 checked: !1
             })
-        }, []), H.a.createElement(wo.a, {
+        }, []), H.a.createElement(Mo.a, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: n,
             key: r,
             disabled: m && !Object(V.isUndefined)(m.componentDisabled) ? m.componentDisabled : o,
             defaultChecked: i,
             checkedChildren: l,
@@ -111182,15 +111263,15 @@
             persistence: p,
             persisted_props: f,
             persistence_type: h,
             "data-dash-is-loading": t && t.is_loading || void 0
         })
     }
 
-    function vo(t) {
+    function _o(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.locale,
             l = t.code,
@@ -111204,15 +111285,15 @@
             m = t.type,
             t = (t.setProps, t.loading_state),
             g = Object(Wt.useContext)(G.a),
             i = g && g.locale || i,
             n = j(n);
         return H.a.createElement(W.a, {
             locale: K.b.get(i)
-        }, H.a.createElement(jo, {
+        }, H.a.createElement(Co, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             code: l,
             copyable: c,
             delete: s,
@@ -111222,15 +111303,15 @@
             italic: f,
             underline: h,
             type: m,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n))
     }
 
-    function yo(t) {
+    function Oo(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.locale,
             l = t.code,
@@ -111245,15 +111326,15 @@
             g = t.keyboard,
             t = (t.setProps, t.loading_state),
             b = Object(Wt.useContext)(G.a),
             i = b && b.locale || i,
             n = j(n);
         return H.a.createElement(W.a, {
             locale: K.b.get(i)
-        }, H.a.createElement(Eo, {
+        }, H.a.createElement(Lo, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             code: l,
             copyable: c,
             delete: s,
@@ -111264,15 +111345,15 @@
             underline: h,
             type: m,
             keyboard: g,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n))
     }
 
-    function xo(t) {
+    function wo(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.locale,
             l = t.level,
@@ -111288,15 +111369,15 @@
             b = t.keyboard,
             t = (t.setProps, t.loading_state),
             v = Object(Wt.useContext)(G.a),
             i = v && v.locale || i,
             n = j(n);
         return H.a.createElement(W.a, {
             locale: K.b.get(i)
-        }, H.a.createElement(So, {
+        }, H.a.createElement(Do, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             level: l,
             code: c,
             copyable: s,
@@ -111308,15 +111389,15 @@
             underline: m,
             type: g,
             keyboard: b,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n))
     }
 
-    function _o(t) {
+    function ko(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.tab,
             i = t.key,
             l = t.disabled,
@@ -111333,15 +111414,15 @@
             titleSideInfoPopover: s,
             disabled: l,
             closable: c,
             children: n,
             "data-dash-is-loading": t && t.is_loading || void 0
         })
     }
-    go._dashprivate_isLoadingComponent = !0, go.propTypes = {
+    yo._dashprivate_isLoadingComponent = !0, yo.propTypes = {
         id: n.a.string,
         children: n.a.node,
         className: n.a.oneOfType([n.a.string, n.a.object]),
         wrapperClassName: n.a.oneOfType([n.a.string, n.a.object]),
         style: n.a.object,
         key: n.a.string,
         spinning: n.a.bool,
@@ -111355,25 +111436,25 @@
         indicator: n.a.node,
         loading_state: n.a.shape({
             is_loading: n.a.bool,
             prop_name: n.a.string,
             component_name: n.a.string
         }),
         setProps: n.a.func
-    }, go.defaultProps = {
+    }, yo.defaultProps = {
         size: "middle",
         spinning: !1,
         listenPropsMode: "default",
         excludeProps: [],
         includeProps: [],
         debug: !1
     };
-    var Oo = go,
-        wo = e(698),
-        ko = (bo.propTypes = {
+    var jo = yo,
+        Mo = e(698),
+        Eo = (xo.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             disabled: n.a.bool,
             checked: n.a.bool,
             checkedChildren: n.a.node,
@@ -111385,24 +111466,24 @@
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func,
             persistence: n.a.oneOfType([n.a.bool, n.a.string, n.a.number]),
             persisted_props: n.a.arrayOf(n.a.oneOf(["checked"])),
             persistence_type: n.a.oneOf(["local", "session", "memory"])
-        }, bo.defaultProps = {
+        }, xo.defaultProps = {
             disabled: !1,
             size: "default",
             loading: !1,
             persisted_props: ["checked"],
             persistence_type: "local"
-        }, bo),
+        }, xo),
         u = e(694),
-        jo = u.a.Paragraph,
-        Mo = (vo.propTypes = {
+        Co = u.a.Paragraph,
+        So = (_o.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             locale: n.a.oneOf(["zh-cn", "en-us"]),
             code: n.a.bool,
@@ -111416,19 +111497,19 @@
             type: n.a.oneOf(["secondary", "success", "warning", "danger"]),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, vo.defaultProps = {
+        }, _o.defaultProps = {
             locale: "zh-cn"
-        }, vo),
-        Eo = u.a.Text,
-        Co = (yo.propTypes = {
+        }, _o),
+        Lo = u.a.Text,
+        Po = (Oo.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             locale: n.a.oneOf(["zh-cn", "en-us"]),
             code: n.a.bool,
@@ -111443,19 +111524,19 @@
             type: n.a.oneOf(["secondary", "success", "warning", "danger"]),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, yo.defaultProps = {
+        }, Oo.defaultProps = {
             locale: "zh-cn"
-        }, yo),
-        So = u.a.Title,
-        Lo = (xo.propTypes = {
+        }, Oo),
+        Do = u.a.Title,
+        To = (wo.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             locale: n.a.oneOf(["zh-cn", "en-us"]),
             level: n.a.number,
@@ -111471,19 +111552,19 @@
             type: n.a.oneOf(["secondary", "success", "warning", "danger"]),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, xo.defaultProps = {
+        }, wo.defaultProps = {
             locale: "zh-cn",
             level: 1
-        }, xo),
-        Po = (_o.propTypes = {
+        }, wo),
+        zo = (ko.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.string,
             style: n.a.object,
             tab: n.a.string,
             key: n.a.string,
             disabled: n.a.bool,
@@ -111494,94 +111575,94 @@
             }),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, _o.defaultProps = {}, _o),
-        Do = e(522),
-        To = e(216);
-    zo = function(t, e) {
+        }, ko.defaultProps = {}, ko),
+        Ao = e(522),
+        Ro = e(216);
+    Io = function(t, e) {
         for (var n, a = {}, r = {}, o = 0, i = t.length; o < i;) o += r[t[o]] = 1;
         for (n in e) r.hasOwnProperty(n) || (a[n] = e[n]);
         return a
     };
-    var zo, Ao = function t(e, n) {
+    var Io, No = function t(e, n) {
             switch (arguments.length) {
                 case 0:
                     return t;
                 case 1:
-                    return R(e) ? t : N(function(t) {
-                        return zo(e, t)
+                    return N(e) ? t : Y(function(t) {
+                        return Io(e, t)
                     });
                 default:
-                    return R(e) && R(n) ? t : R(e) ? N(function(t) {
-                        return zo(t, n)
-                    }) : R(n) ? N(function(t) {
-                        return zo(e, t)
-                    }) : zo(e, n)
+                    return N(e) && N(n) ? t : N(e) ? Y(function(t) {
+                        return Io(t, n)
+                    }) : N(n) ? Y(function(t) {
+                        return Io(e, t)
+                    }) : Io(e, n)
             }
         },
-        Ro = ["id", "className", "style", "tab", "key", "disabled", "closable", "titleSideInfoPopover", "loading_state"];
+        Yo = ["id", "className", "style", "tab", "key", "disabled", "closable", "titleSideInfoPopover", "loading_state"];
 
-    function Io(t) {
-        return (Io = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
+    function Bo(t) {
+        return (Bo = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
             return typeof t
         } : function(t) {
             return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
         })(t)
     }
 
-    function No() {
-        return (No = Object.assign ? Object.assign.bind() : function(t) {
+    function Fo() {
+        return (Fo = Object.assign ? Object.assign.bind() : function(t) {
             for (var e = 1; e < arguments.length; e++) {
                 var n, a = arguments[e];
                 for (n in a) Object.prototype.hasOwnProperty.call(a, n) && (t[n] = a[n])
             }
             return t
         }).apply(this, arguments)
     }
 
-    function Yo(e, t) {
+    function Ho(e, t) {
         var n, a = Object.keys(e);
         return Object.getOwnPropertySymbols && (n = Object.getOwnPropertySymbols(e), t && (n = n.filter(function(t) {
             return Object.getOwnPropertyDescriptor(e, t).enumerable
         })), a.push.apply(a, n)), a
     }
 
-    function Bo(a) {
+    function Wo(a) {
         for (var t = 1; t < arguments.length; t++) {
             var r = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? Yo(Object(r), !0).forEach(function(t) {
+            t % 2 ? Ho(Object(r), !0).forEach(function(t) {
                 var e, n;
                 e = a, t = r[n = t], (n = function() {
                     var t = function(t) {
-                        if ("object" !== Io(t) || null === t) return t;
+                        if ("object" !== Bo(t) || null === t) return t;
                         var e = t[Symbol.toPrimitive];
                         if (void 0 === e) return String(t);
                         e = e.call(t, "string");
-                        if ("object" !== Io(e)) return e;
+                        if ("object" !== Bo(e)) return e;
                         throw new TypeError("@@toPrimitive must return a primitive value.")
                     }(n);
-                    return "symbol" === Io(t) ? t : String(t)
+                    return "symbol" === Bo(t) ? t : String(t)
                 }()) in e ? Object.defineProperty(e, n, {
                     value: t,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : e[n] = t
-            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(r)) : Yo(Object(r)).forEach(function(t) {
+            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(r)) : Ho(Object(r)).forEach(function(t) {
                 Object.defineProperty(a, t, Object.getOwnPropertyDescriptor(r, t))
             })
         }
         return a
     }
 
-    function Fo(t) {
+    function Vo(t) {
         function e(t) {
             _({
                 activeKey: t
             })
         }
 
         function n(t, e) {
@@ -111613,18 +111694,18 @@
             k = t.persistence_type,
             t = t.loading_state;
         return Object(Wt.useEffect)(function() {
             p && !f && _({
                 activeKey: p
             })
         }, []), c ? (s && (c = c.map(function(t) {
-            return s.includes(t.key) ? Bo(Bo({}, t), {}, {
+            return s.includes(t.key) ? Wo(Wo({}, t), {}, {
                 disabled: !0
             }) : t
-        })), H.a.createElement(Do.a, {
+        })), H.a.createElement(Ao.a, {
             id: a,
             className: Object(V.isString)(o) ? o : o ? Object(U.a)(o) : void 0,
             style: i,
             key: l,
             items: c,
             defaultActiveKey: p,
             activeKey: f,
@@ -111645,15 +111726,15 @@
             onChange: e,
             onEdit: n,
             persistence: O,
             persisted_props: w,
             persistence_type: k,
             "data-dash-is-loading": t && t.is_loading || void 0
         })) : (c = (r = j(r)).map(function(t) {
-            var e = Y(t),
+            var e = et(t),
                 n = e.id,
                 a = e.className,
                 r = e.style,
                 o = e.tab,
                 i = e.key,
                 l = e.disabled,
                 c = e.closable,
@@ -111665,20 +111746,20 @@
                         if (null == t) return {};
                         for (var n, a = {}, r = Object.keys(t), o = 0; o < r.length; o++) n = r[o], 0 <= e.indexOf(n) || (a[n] = t[n]);
                         return a
                     }(t, e);
                     if (Object.getOwnPropertySymbols)
                         for (var r = Object.getOwnPropertySymbols(t), o = 0; o < r.length; o++) n = r[o], 0 <= e.indexOf(n) || Object.prototype.propertyIsEnumerable.call(t, n) && (a[n] = t[n]);
                     return a
-                }(e, Ro);
-            return H.a.createElement(Wo, No({
+                }(e, Yo);
+            return H.a.createElement(Uo, Fo({
                 id: n,
                 className: a,
                 style: r,
-                tab: s && s.content ? H.a.createElement(H.a.Fragment, null, H.a.createElement("span", null, o), H.a.createElement(To.a, {
+                tab: s && s.content ? H.a.createElement(H.a.Fragment, null, H.a.createElement("span", null, o), H.a.createElement(Ro.a, {
                     title: s.title,
                     content: H.a.createElement("div", {
                         style: {
                             maxWidth: "250px",
                             wordWrap: "break-word",
                             whiteSpace: "normal",
                             wordBreak: "break-all"
@@ -111687,27 +111768,27 @@
                     overlayStyle: {
                         maxWidth: "250px"
                     },
                     placement: "right",
                     getPopupContainer: function(t) {
                         return t.parentNode.parentNode.parentNode.parentNode.parentNode.parentNode
                     }
-                }, H.a.createElement(Fa.a, {
+                }, H.a.createElement(Va.a, {
                     style: {
                         color: "#8c8c8c",
                         paddingLeft: "4px",
                         cursor: "pointer"
                     }
                 }))) : o,
                 key: i,
                 disabled: l,
                 closable: c,
                 loading_state: u
-            }, Ao(["setProps", "persistence", "persistence_type", "persisted_props"], e)), t)
-        }), H.a.createElement(Do.a, {
+            }, No(["setProps", "persistence", "persistence_type", "persisted_props"], e)), t)
+        }), H.a.createElement(Ao.a, {
             id: a,
             className: Object(V.isString)(o) ? o : o ? Object(U.a)(o) : void 0,
             style: i,
             key: l,
             defaultActiveKey: p,
             activeKey: f,
             size: h,
@@ -111729,15 +111810,15 @@
             persistence: O,
             persisted_props: w,
             persistence_type: k,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, c))
     }
 
-    function Ho(t) {
+    function Ko(t) {
         var e = t.id,
             n = t.style,
             a = t.className,
             r = t.key,
             o = t.locale,
             i = t.defaultCurrent,
             l = t.defaultPageSize,
@@ -111765,15 +111846,15 @@
             i && !c && _({
                 current: i
             }), l && !s && _({
                 pageSize: l
             })
         }, []), H.a.createElement(W.a, {
             locale: K.b.get(o)
-        }, H.a.createElement(Me.a, {
+        }, H.a.createElement(Se.a, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: n,
             key: r,
             pageSize: s || l,
             defaultCurrent: i,
             defaultPageSize: l,
@@ -111797,16 +111878,16 @@
             },
             persistence: w,
             persisted_props: k,
             persistence_type: t,
             "data-dash-is-loading": O && O.is_loading || void 0
         }))
     }
-    var Wo = Do.a.TabPane,
-        Vo = (Fo.propTypes = {
+    var Uo = Ao.a.TabPane,
+        Go = (Vo.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             items: n.a.arrayOf(n.a.exact({
                 label: n.a.node,
@@ -111834,26 +111915,26 @@
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func,
             persistence: n.a.oneOfType([n.a.bool, n.a.string, n.a.number]),
             persisted_props: n.a.arrayOf(n.a.oneOf(["activeKey"])),
             persistence_type: n.a.oneOf(["local", "session", "memory"])
-        }, Fo.defaultProps = {
+        }, Vo.defaultProps = {
             disabledTabKeys: [],
             tabPosition: "top",
             size: "default",
             type: "line",
             centered: !1,
             inkBarAnimated: !0,
             tabPaneAnimated: !1,
             persisted_props: ["activeKey"],
             persistence_type: "local"
-        }, Fo),
-        Ko = (Ho.propTypes = {
+        }, Vo),
+        qo = (Ko.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             locale: n.a.oneOf(["zh-cn", "en-us"]),
             defaultCurrent: n.a.number,
             defaultPageSize: n.a.number,
@@ -111875,48 +111956,48 @@
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func,
             persistence: n.a.oneOfType([n.a.bool, n.a.string, n.a.number]),
             persisted_props: n.a.arrayOf(n.a.oneOf(["current", "pageSize"])),
             persistence_type: n.a.oneOf(["local", "session", "memory"])
-        }, Ho.defaultProps = {
+        }, Ko.defaultProps = {
             defaultCurrent: 1,
             defaultPageSize: 10,
             hideOnSinglePage: !1,
             showSizeChanger: !1,
             showQuickJumper: !1,
             simple: !1,
             size: "default",
             locale: "zh-cn",
             showTotal: !0,
             disabled: !1,
             persisted_props: ["current", "pageSize"],
             persistence_type: "local"
-        }, Ho),
-        Uo = e(87),
-        Go = e(83),
-        qo = e(180),
-        Xo = e(92),
-        $o = e(187),
-        Zo = Wt.createContext(null),
-        Jo = Wt.createContext(null);
+        }, Ko),
+        Xo = e(87),
+        $o = e(83),
+        Zo = e(180),
+        Jo = e(92),
+        Qo = e(187),
+        ti = Wt.createContext(null),
+        ei = Wt.createContext(null);
 
-    function Qo(t) {
+    function ni(t) {
         return !t || t.disabled || t.disableCheckbox || !1 === t.checkable
     }
 
-    function ti(t) {
+    function ai(t) {
         return null == t
     }
 
-    function ei() {
+    function ri() {
         return null
     }
-    var ni = {
+    var oi = {
             width: 0,
             height: 0,
             display: "flex",
             overflow: "hidden",
             opacity: 0,
             border: 0,
             padding: 0,
@@ -111924,35 +112005,35 @@
         },
         c = Wt.forwardRef(function(R, t) {
             function e(t) {
                 t.preventDefault()
             }
 
             function a(t, e) {
-                e = e.node, v && Qo(e) || (m(e.key, {
+                e = e.node, v && ni(e) || (m(e.key, {
                     selected: !y.includes(e.key)
                 }), o) || l(!1)
             }
-            var n = Object(Uo.e)(),
+            var n = Object(Xo.e)(),
                 r = n.prefixCls,
                 o = n.multiple,
                 i = n.searchValue,
                 l = n.toggleOpen,
                 c = n.open,
                 n = n.notFoundContent,
-                s = Wt.useContext(Jo),
+                s = Wt.useContext(ei),
                 u = s.virtual,
                 d = s.listHeight,
                 p = s.listItemHeight,
                 f = s.treeData,
                 h = s.fieldNames,
                 m = s.onSelect,
                 g = s.dropdownMatchSelectWidth,
                 s = s.treeExpandAction,
-                b = Wt.useContext(Zo),
+                b = Wt.useContext(ti),
                 v = b.checkable,
                 y = b.checkedKeys,
                 x = b.halfCheckedKeys,
                 _ = b.treeExpandedKeys,
                 O = b.treeDefaultExpandAll,
                 w = b.treeDefaultExpandedKeys,
                 k = b.onTreeExpand,
@@ -111963,15 +112044,15 @@
                 B = b.treeNodeFilterProp,
                 F = b.loadData,
                 M = b.treeLoadedKeys,
                 H = b.treeMotion,
                 W = b.onTreeLoad,
                 b = b.keyEntities,
                 E = Wt.useRef(),
-                C = Object(Xo.a)(function() {
+                C = Object(Jo.a)(function() {
                     return f
                 }, [c, f], function(t, e) {
                     return e[0] && t[1] !== e[1]
                 }),
                 V = Wt.useMemo(function() {
                     return v ? {
                         checked: y,
@@ -112040,17 +112121,17 @@
                 className: "".concat(r, "-empty"),
                 onMouseDown: e
             }, n) : (b = {
                 fieldNames: h
             }, M && (b.loadedKeys = M), w && (b.expandedKeys = w), Wt.createElement("div", {
                 onMouseDown: e
             }, A && c && Wt.createElement("span", {
-                style: ni,
+                style: oi,
                 "aria-live": "assertive"
-            }, A.node.value), Wt.createElement($o.b, Object(Et.a)({
+            }, A.node.value), Wt.createElement(Qo.b, Object(Et.a)({
                 ref: E,
                 focusable: !1,
                 prefixCls: "".concat(r, "-tree"),
                 treeData: C,
                 height: d,
                 itemHeight: p,
                 virtual: !1 !== u && !1 !== g,
@@ -112077,80 +112158,80 @@
                 onLoad: W,
                 filterTreeNode: function(t) {
                     return !!S && String(t[B]).toLowerCase().includes(S)
                 },
                 expandAction: s
             }))))
         }),
-        ai = (c.displayName = "OptionList", c);
+        ii = (c.displayName = "OptionList", c);
 
-    function ri(t, e, n, a) {
+    function li(t, e, n, a) {
         var r = new Set(t);
         return "SHOW_CHILD" === e ? t.filter(function(t) {
             t = n[t];
             return !(t && t.children && t.children.some(function(t) {
                 t = t.node;
                 return r.has(t[a.value])
             }) && t.children.every(function(t) {
                 t = t.node;
-                return Qo(t) || r.has(t[a.value])
+                return ni(t) || r.has(t[a.value])
             }))
         }) : "SHOW_PARENT" === e ? t.filter(function(t) {
             t = n[t], t = t ? t.parent : null;
-            return !(t && !Qo(t.node) && r.has(t.key))
+            return !(t && !ni(t.node) && r.has(t.key))
         }) : t
     }
-    var oi = ["children", "value"];
+    var ci = ["children", "value"];
 
-    function ii(t) {
+    function si(t) {
         var e;
         return t && ("props" in (e = Object(Ct.a)({}, t)) || Object.defineProperty(e, "props", {
             get: function() {
-                return Object(de.a)(!1, "New `rc-tree-select` not support return node instance as argument anymore. Please consider to remove `props` access."), e
+                return Object(me.a)(!1, "New `rc-tree-select` not support return node instance as argument anymore. Please consider to remove `props` access."), e
             }
         }), e)
     }
 
-    function li(l, c, s) {
+    function ui(l, c, s) {
         return Wt.useMemo(function() {
             return l ? s ? (t = l, e = Object(Ct.a)({
                 id: "id",
                 pId: "pId",
                 rootPId: null
             }, !0 !== s ? s : {}), n = e.id, a = e.pId, r = e.rootPId, o = {}, i = [], t.map(function(t) {
                 var t = Object(Ct.a)({}, t),
                     e = t[n];
                 return (o[e] = t).key = t.key || e, t
             }).forEach(function(t) {
                 var e = t[a],
                     n = o[e];
                 n && (n.children = n.children || [], n.children.push(t)), e !== r && (n || null !== r) || i.push(t)
             }), i) : l : function r(t) {
-                return Object(Dn.a)(t).map(function(t) {
+                return Object(An.a)(t).map(function(t) {
                     var e, n, a;
-                    return Wt.isValidElement(t) && t.type ? (n = t.key, e = (t = t.props).children, a = t.value, t = Object(Bt.a)(t, oi), n = Object(Ct.a)({
+                    return Wt.isValidElement(t) && t.type ? (n = t.key, e = (t = t.props).children, a = t.value, t = Object(Jt.a)(t, ci), n = Object(Ct.a)({
                         key: n,
                         value: a
                     }, t), (a = r(e)).length && (n.children = a), n) : null
                 }).filter(function(t) {
                     return t
                 })
             }(c);
             var t, e, n, a, r, o, i
         }, [c, s, l])
     }
 
-    function ci(t) {
+    function di(t) {
         var e = Wt.useRef();
         return e.current = t, Wt.useCallback(function() {
             return e.current.apply(e, arguments)
         }, [])
     }
-    var si = e(42),
-        ui = ["id", "prefixCls", "value", "defaultValue", "onChange", "onSelect", "onDeselect", "searchValue", "inputValue", "onSearch", "autoClearSearchValue", "filterTreeNode", "treeNodeFilterProp", "showCheckedStrategy", "treeNodeLabelProp", "multiple", "treeCheckable", "treeCheckStrictly", "labelInValue", "fieldNames", "treeDataSimpleMode", "treeData", "children", "loadData", "treeLoadedKeys", "onTreeLoad", "treeDefaultExpandAll", "treeExpandedKeys", "treeDefaultExpandedKeys", "onTreeExpand", "treeExpandAction", "virtual", "listHeight", "listItemHeight", "onDropdownVisibleChange", "dropdownMatchSelectWidth", "treeLine", "treeIcon", "showTreeIcon", "switcherIcon", "treeMotion"],
+    var pi = e(42),
+        fi = ["id", "prefixCls", "value", "defaultValue", "onChange", "onSelect", "onDeselect", "searchValue", "inputValue", "onSearch", "autoClearSearchValue", "filterTreeNode", "treeNodeFilterProp", "showCheckedStrategy", "treeNodeLabelProp", "multiple", "treeCheckable", "treeCheckStrictly", "labelInValue", "fieldNames", "treeDataSimpleMode", "treeData", "children", "loadData", "treeLoadedKeys", "onTreeLoad", "treeDefaultExpandAll", "treeExpandedKeys", "treeDefaultExpandedKeys", "onTreeExpand", "treeExpandAction", "virtual", "listHeight", "listItemHeight", "onDropdownVisibleChange", "dropdownMatchSelectWidth", "treeLine", "treeIcon", "showTreeIcon", "switcherIcon", "treeMotion"],
         d = Wt.forwardRef(function(t, R) {
             var e, n, r, o, i, l, a, c, s, u, d, I, p, f = t.id,
                 N = t.prefixCls,
                 N = void 0 === N ? "rc-tree-select" : N,
                 h = t.value,
                 Y = t.defaultValue,
                 B = t.onChange,
@@ -112192,47 +112273,47 @@
                 _ = t.dropdownMatchSelectWidth,
                 dt = void 0 === _ || _,
                 pt = t.treeLine,
                 ft = t.treeIcon,
                 ht = t.showTreeIcon,
                 mt = t.switcherIcon,
                 gt = t.treeMotion,
-                _ = Object(Bt.a)(t, ui),
-                t = Object(qo.a)(f),
+                _ = Object(Jt.a)(t, fi),
+                t = Object(Zo.a)(f),
                 O = v && !y,
                 w = v || y,
                 bt = y || x,
                 k = w || b,
-                f = Object($t.a)(Y, {
+                f = Object(Zt.a)(Y, {
                     value: h
                 }),
                 v = Object(Gt.a)(f, 2),
                 j = v[0],
                 vt = v[1],
                 M = Wt.useMemo(function() {
                     return e = (t = X || {}).label, n = t.value || "value", {
                         _title: e ? [e] : ["title", "label"],
                         value: n,
                         key: n,
                         children: t.children || "children"
                     };
                     var t, e, n
                 }, [JSON.stringify(X)]),
-                x = Object($t.a)("", {
+                x = Object(Zt.a)("", {
                     value: void 0 !== m ? m : W,
                     postState: function(t) {
                         return t || ""
                     }
                 }),
                 b = Object(Gt.a)(x, 2),
                 Y = b[0],
                 yt = b[1],
-                E = li(Z, J, $),
+                E = ui(Z, J, $),
                 h = (I = E, p = M, Wt.useMemo(function() {
-                    return Object(si.a)(I, {
+                    return Object(pi.a)(I, {
                         fieldNames: p,
                         initWrapper: function(t) {
                             return Object(Ct.a)(Object(Ct.a)({}, t), {}, {
                                 valueEntities: new Map
                             })
                         },
                         processEntity: function(t, e) {
@@ -112262,15 +112343,15 @@
                     return c && !1 !== u ? (o = "function" == typeof u ? u : (n = c.toUpperCase(), function(t, e) {
                         e = e[s];
                         return String(e).toUpperCase().includes(n)
                     }), function a(t) {
                         var r = 1 < arguments.length && void 0 !== arguments[1] && arguments[1];
                         return t.map(function(t) {
                             var e = t[d],
-                                n = r || o(c, ii(t)),
+                                n = r || o(c, si(t)),
                                 e = a(e || [], n);
                             return n || e.length ? Object(Ct.a)(Object(Ct.a)({}, t), {}, Object(Vt.a)({
                                 isLeaf: void 0
                             }, d, e)) : null
                         }).filter(function(t) {
                             return t
                         })
@@ -112333,35 +112414,35 @@
                         }),
                         n = o.map(function(t) {
                             return t.value
                         }),
                         a = e.filter(function(t) {
                             return !l[t]
                         });
-                    return i && (e = (t = Object(Go.a)(e, !0, l)).checkedKeys, n = t.halfCheckedKeys), [Array.from(new Set([].concat(Object(Ut.a)(a), Object(Ut.a)(e)))), n]
+                    return i && (e = (t = Object($o.a)(e, !0, l)).checkedKeys, n = t.halfCheckedKeys), [Array.from(new Set([].concat(Object(Ut.a)(a), Object(Ut.a)(e)))), n]
                 }, [r, o, i, l])),
                 x = Object(Gt.a)(W, 2),
                 T = x[0],
                 z = x[1],
                 b = Wt.useMemo(function() {
-                    var t = ri(T, G, C, M).map(function(t) {
+                    var t = li(T, G, C, M).map(function(t) {
                             var e;
                             return null != (e = null == (e = C[t]) || null == (e = e.node) ? void 0 : e[M.value]) ? e : t
                         }).map(function(e) {
                             var t = D.find(function(t) {
                                 return t.value === e
                             });
                             return {
                                 value: e,
                                 label: null == t ? void 0 : t.label
                             }
                         }),
                         t = P(t),
                         e = t[0];
-                    return !k && e && ti(e.value) && ti(e.label) ? [] : t.map(function(t) {
+                    return !k && e && ai(e.value) && ai(e.label) ? [] : t.map(function(t) {
                         var e;
                         return Object(Ct.a)(Object(Ct.a)({}, t), {}, {
                             label: null != (e = t.label) ? e : t.value
                         })
                     })
                 }, [M, k, T, D, P, G, C]),
                 Z = (e = b, n = Wt.useRef({
@@ -112375,27 +112456,27 @@
                             return r.set(e, n), Object(Ct.a)(Object(Ct.a)({}, t), {}, {
                                 label: n
                             })
                         });
                     return n.current.valueLabels = r, [t]
                 }, [e])),
                 J = Object(Gt.a)(Z, 1)[0],
-                A = ci(function(t, e, n) {
+                A = di(function(t, e, n) {
                     var a, r, o, i, c, s, l, u, d, p, f, h = P(t);
 
                     function m() {
                         f || (f = [], function o(t) {
                             var i = 1 < arguments.length && void 0 !== arguments[1] ? arguments[1] : "0",
                                 l = 2 < arguments.length && void 0 !== arguments[2] && arguments[2];
                             return t.map(function(t, e) {
                                 var e = "".concat(i, "-").concat(e),
                                     n = t[d.value],
                                     a = s.includes(n),
                                     r = o(t[d.children] || [], e, a),
-                                    t = Wt.createElement(ei, t, r.map(function(t) {
+                                    t = Wt.createElement(ri, t, r.map(function(t) {
                                         return t.node
                                     }));
                                 return c === n && (p = t), a ? (n = {
                                     pos: e,
                                     node: t,
                                     children: r
                                 }, l || f.push(n), n) : null
@@ -112403,32 +112484,32 @@
                                 return t
                             })
                         }(l), f.sort(function(t, e) {
                             t = t.node.props.value, e = e.node.props.value;
                             return s.indexOf(t) - s.indexOf(e)
                         }))
                     }
-                    vt(h), K && yt(""), B && (a = t, O && (a = ri(t, G, C, M).map(function(t) {
+                    vt(h), K && yt(""), B && (a = t, O && (a = li(t, G, C, M).map(function(t) {
                         var e = S.get(t);
                         return e ? e.node[M.value] : t
                     })), e = (h = e || {
                         triggerValue: void 0,
                         selected: void 0
                     }).triggerValue, h = h.selected, o = a, y && (r = kt.filter(function(t) {
                         return !a.includes(t.value)
                     }), o = [].concat(Object(Ut.a)(o), Object(Ut.a)(r))), r = P(o), i = o = {
                         preValue: D,
                         triggerValue: e
                     }, c = e, s = t, l = E, u = y || "selection" === n && !h ? !1 : !0, d = M, f = p = null, Object.defineProperty(i, "triggerNode", {
                         get: function() {
-                            return Object(de.a)(!1, "`triggerNode` is deprecated. Please consider decoupling data with node."), m(), p
+                            return Object(me.a)(!1, "`triggerNode` is deprecated. Please consider decoupling data with node."), m(), p
                         }
                     }), Object.defineProperty(i, "allCheckedNodes", {
                         get: function() {
-                            return Object(de.a)(!1, "`allCheckedNodes` is deprecated. Please consider decoupling data with node."), m(), u ? f : f.map(function(t) {
+                            return Object(me.a)(!1, "`allCheckedNodes` is deprecated. Please consider decoupling data with node."), m(), u ? f : f.map(function(t) {
                                 return t.node
                             })
                         }
                     }), w ? o.checked = h : o.selected = h, e = bt ? r : r.map(function(t) {
                         return t.value
                     }), B(k ? e : e[0], bt ? null : r.map(function(t) {
                         return t.label
@@ -112440,36 +112521,36 @@
                         o = C[t],
                         o = null == o ? void 0 : o.node,
                         i = null != (a = null == o ? void 0 : o[M.value]) ? a : t;
                     k ? (a = r ? [].concat(Object(Ut.a)(jt), [i]) : T.filter(function(t) {
                         return t !== i
                     }), O && (n = (t = xt(a)).missingRawValues, t = t.existRawValues.map(function(t) {
                         return S.get(t).key
-                    }), t = (r ? Object(Go.a)(t, !0, C) : Object(Go.a)(t, {
+                    }), t = (r ? Object($o.a)(t, !0, C) : Object($o.a)(t, {
                         checked: !1,
                         halfCheckedKeys: z
                     }, C)).checkedKeys, a = [].concat(Object(Ut.a)(n), Object(Ut.a)(t.map(function(t) {
                         return C[t].node[M.value]
                     })))), A(a, {
                         selected: r,
                         triggerValue: i
                     }, e || "option")) : A([i], {
                         selected: !0,
                         triggerValue: i
-                    }, "option"), r || !k ? null != F && F(i, ii(o)) : null != H && H(i, ii(o))
+                    }, "option"), r || !k ? null != F && F(i, si(o)) : null != H && H(i, si(o))
                 }, [xt, S, C, M, k, jt, A, O, F, H, T, z]),
                 $ = Wt.useCallback(function(t) {
                     var e;
                     ut && (e = {}, Object.defineProperty(e, "documentClickClose", {
                         get: function() {
-                            return Object(de.a)(!1, "Second param of `onDropdownVisibleChange` has been removed."), !1
+                            return Object(me.a)(!1, "Second param of `onDropdownVisibleChange` has been removed."), !1
                         }
                     }), ut(t, e))
                 }, [ut]),
-                h = ci(function(t, e) {
+                h = di(function(t, e) {
                     t = t.map(function(t) {
                         return t.value
                     });
                     "clear" !== e.type ? e.values.length && Mt(e.values[0].value, {
                         selected: !1,
                         source: "selection"
                     }) : A(t, {}, "selection")
@@ -112503,41 +112584,41 @@
                         showTreeIcon: ht,
                         switcherIcon: mt,
                         treeLine: pt,
                         treeNodeFilterProp: U,
                         keyEntities: C
                     }
                 }, [w, Q, tt, et, T, z, nt, at, rt, ot, ft, gt, ht, mt, pt, U, C]);
-            return Wt.createElement(Jo.Provider, {
+            return Wt.createElement(ei.Provider, {
                 value: g
-            }, Wt.createElement(Zo.Provider, {
+            }, Wt.createElement(ti.Provider, {
                 value: f
-            }, Wt.createElement(Uo.a, Object(Et.a)({
+            }, Wt.createElement(Xo.a, Object(Et.a)({
                 ref: R
             }, _, {
                 id: t,
                 prefixCls: N,
                 mode: k ? "multiple" : void 0,
                 displayValues: J,
                 onDisplayValuesChange: h,
                 searchValue: Y,
                 onSearch: function(t) {
                     yt(t), null != V && V(t)
                 },
-                OptionList: ai,
+                OptionList: ii,
                 emptyOptions: !E.length,
                 onDropdownVisibleChange: $,
                 dropdownMatchSelectWidth: dt
             }))))
         }),
-        di = (d.TreeNode = ei, d.SHOW_ALL = "SHOW_ALL", d.SHOW_PARENT = "SHOW_PARENT", d.SHOW_CHILD = "SHOW_CHILD", d),
-        pi = e(60),
-        fi = e(49),
-        hi = e(181),
-        mi = e(276),
+        hi = (d.TreeNode = ri, d.SHOW_ALL = "SHOW_ALL", d.SHOW_PARENT = "SHOW_PARENT", d.SHOW_CHILD = "SHOW_CHILD", d),
+        mi = e(60),
+        gi = e(49),
+        bi = e(181),
+        vi = e(276),
         c = Wt.forwardRef(function(t, e) {
             var n = t.prefixCls,
                 a = t.size,
                 r = t.disabled,
                 o = t.bordered,
                 o = void 0 === o || o,
                 i = t.className,
@@ -112572,48 +112653,48 @@
                 w = Wt.useContext(q.b),
                 I = w.getPopupContainer,
                 k = w.getPrefixCls,
                 j = w.renderEmpty,
                 M = w.direction,
                 N = w.virtual,
                 w = w.dropdownMatchSelectWidth,
-                E = Wt.useContext(fi.b),
+                E = Wt.useContext(gi.b),
                 C = k("select", n),
                 Y = k("select-tree", n),
                 S = k("tree-select", n),
-                L = Object(Ga.c)(C, M),
+                L = Object($a.c)(C, M),
                 P = L.compactSize,
                 L = L.compactItemClassnames,
                 b = Kt()(b || g, "".concat(S, "-dropdown"), Object(Vt.a)({}, "".concat(S, "-dropdown-rtl"), "rtl" === M)),
                 g = !(!l && !c),
                 D = void 0 !== O ? O : t.loading || !g,
-                T = Object(Wt.useContext)(ve.b),
+                T = Object(Wt.useContext)(Oe.b),
                 z = T.status,
                 A = T.hasFeedback,
                 B = T.isFormItemInput,
                 T = T.feedbackIcon,
-                z = Object(_e.a)(z, _),
-                _ = Object(hi.a)(Object(Et.a)(Object(Et.a)({}, t), {
+                z = Object(je.a)(z, _),
+                _ = Object(bi.a)(Object(Et.a)(Object(Et.a)({}, t), {
                     multiple: g,
                     showArrow: D,
                     hasFeedback: A,
                     feedbackIcon: T,
                     prefixCls: C
                 })),
                 g = _.suffixIcon,
                 D = _.removeIcon,
                 T = _.clearIcon,
-                _ = void 0 !== p ? p : (j || be.a)("Select"),
-                p = Object(ct.a)(t, ["suffixIcon", "itemIcon", "removeIcon", "clearIcon", "switcherIcon"]),
+                _ = void 0 !== p ? p : (j || _e.a)("Select"),
+                p = Object(pt.a)(t, ["suffixIcon", "itemIcon", "removeIcon", "clearIcon", "switcherIcon"]),
                 j = P || a || E,
-                t = Wt.useContext(pi.b),
+                t = Wt.useContext(mi.b),
                 P = null != r ? r : t,
-                E = Kt()(!n && S, (a = {}, Object(Vt.a)(a, "".concat(C, "-lg"), "large" === j), Object(Vt.a)(a, "".concat(C, "-sm"), "small" === j), Object(Vt.a)(a, "".concat(C, "-rtl"), "rtl" === M), Object(Vt.a)(a, "".concat(C, "-borderless"), !o), Object(Vt.a)(a, "".concat(C, "-in-form-item"), B), a), Object(_e.b)(C, z, A), L, i),
+                E = Kt()(!n && S, (a = {}, Object(Vt.a)(a, "".concat(C, "-lg"), "large" === j), Object(Vt.a)(a, "".concat(C, "-sm"), "small" === j), Object(Vt.a)(a, "".concat(C, "-rtl"), "rtl" === M), Object(Vt.a)(a, "".concat(C, "-borderless"), !o), Object(Vt.a)(a, "".concat(C, "-in-form-item"), B), a), Object(je.b)(C, z, A), L, i),
                 r = k();
-            return Wt.createElement(di, Object(Et.a)({
+            return Wt.createElement(hi, Object(Et.a)({
                 virtual: N,
                 dropdownMatchSelectWidth: w,
                 disabled: P
             }, p, {
                 ref: e,
                 prefixCls: C,
                 className: E,
@@ -112625,73 +112706,73 @@
                 treeLine: !!h,
                 inputIcon: g,
                 multiple: c,
                 placement: void 0 !== d ? d : "rtl" === M ? "bottomRight" : "bottomLeft",
                 removeIcon: D,
                 clearIcon: T,
                 switcherIcon: function(t) {
-                    return Object(mi.a)(Y, f, h, t)
+                    return Object(vi.a)(Y, f, h, t)
                 },
                 showTreeIcon: v,
                 notFoundContent: _,
                 getPopupContainer: m || I,
                 treeMotion: null,
                 dropdownClassName: b,
-                choiceTransitionName: Object(Va.c)(r, "", x),
-                transitionName: Object(Va.c)(r, Object(Va.b)(d), y),
+                choiceTransitionName: Object(Ga.c)(r, "", x),
+                transitionName: Object(Ga.c)(r, Object(Ga.b)(d), y),
                 showArrow: A || O,
                 treeExpandAction: R
             }))
         }),
-        gi = (c.TreeNode = ei, c.SHOW_ALL = "SHOW_ALL", c.SHOW_PARENT = "SHOW_PARENT", c.SHOW_CHILD = "SHOW_CHILD", c);
+        yi = (c.TreeNode = ri, c.SHOW_ALL = "SHOW_ALL", c.SHOW_PARENT = "SHOW_PARENT", c.SHOW_CHILD = "SHOW_CHILD", c);
 
-    function bi(t) {
-        return (bi = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
+    function xi(t) {
+        return (xi = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
             return typeof t
         } : function(t) {
             return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
         })(t)
     }
 
-    function vi(e, t) {
+    function _i(e, t) {
         var n, a = Object.keys(e);
         return Object.getOwnPropertySymbols && (n = Object.getOwnPropertySymbols(e), t && (n = n.filter(function(t) {
             return Object.getOwnPropertyDescriptor(e, t).enumerable
         })), a.push.apply(a, n)), a
     }
 
-    function yi(a) {
+    function Oi(a) {
         for (var t = 1; t < arguments.length; t++) {
             var r = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? vi(Object(r), !0).forEach(function(t) {
+            t % 2 ? _i(Object(r), !0).forEach(function(t) {
                 var e, n;
                 e = a, t = r[n = t], (n = function() {
                     var t = function(t) {
-                        if ("object" !== bi(t) || null === t) return t;
+                        if ("object" !== xi(t) || null === t) return t;
                         var e = t[Symbol.toPrimitive];
                         if (void 0 === e) return String(t);
                         e = e.call(t, "string");
-                        if ("object" !== bi(e)) return e;
+                        if ("object" !== xi(e)) return e;
                         throw new TypeError("@@toPrimitive must return a primitive value.")
                     }(n);
-                    return "symbol" === bi(t) ? t : String(t)
+                    return "symbol" === xi(t) ? t : String(t)
                 }()) in e ? Object.defineProperty(e, n, {
                     value: t,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : e[n] = t
-            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(r)) : vi(Object(r)).forEach(function(t) {
+            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(r)) : _i(Object(r)).forEach(function(t) {
                 Object.defineProperty(a, t, Object.getOwnPropertyDescriptor(r, t))
             })
         }
         return a
     }
 
-    function xi(t) {
+    function wi(t) {
         var e = t.id,
             n = t.style,
             a = t.className,
             r = t.key,
             o = t.locale,
             i = t.treeData,
             l = t.treeDataMode,
@@ -112735,18 +112816,18 @@
                     treeExpandedKeys: _
                 })
             }, []), Object(Wt.useMemo)(function() {
                 return B(i)
             }, [i]));
         return React.createElement(W.a, {
             locale: K.b.get(o)
-        }, React.createElement(gi, {
+        }, React.createElement(yi, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
-            style: yi({
+            style: Oi({
                 width: "100%"
             }, n),
             key: r,
             treeData: "flat" === l ? Y : i,
             allowClear: Object(V.isUndefined)(P) ? c : !P,
             bordered: s,
             treeLine: u,
@@ -112754,15 +112835,15 @@
             placeholder: p,
             value: f,
             defaultValue: h,
             maxTagCount: m,
             multiple: g,
             size: A && !Object(V.isUndefined)(A.componentSize) ? A.componentSize : b,
             treeCheckable: v,
-            showCheckedStrategy: Oi.get(D),
+            showCheckedStrategy: ji.get(D),
             treeCheckStrictly: y,
             treeDefaultExpandAll: x,
             treeDefaultExpandedKeys: _,
             treeExpandedKeys: O,
             onChange: function(t) {
                 L(y ? {
                     value: t.map(function(t) {
@@ -112794,32 +112875,32 @@
             getPopupContainer: "parent" === S ? function(t) {
                 return t.parentNode
             } : void 0,
             open: !(!Object(V.isUndefined)(P) && P) && void 0
         }))
     }
 
-    function _i(t) {
+    function ki(t) {
         var e = t.prefixCls,
             n = t.className,
             a = t.style,
             r = t.children,
             t = t.containerRef;
         return Wt.createElement(Wt.Fragment, null, Wt.createElement("div", {
             className: Kt()("".concat(e, "-content"), n),
             style: Object(Ct.a)({}, a),
             "aria-modal": "true",
             role: "dialog",
             ref: t
         }, r))
     }
-    var d = gi.SHOW_ALL,
-        c = gi.SHOW_CHILD,
-        p = gi.SHOW_PARENT,
-        Oi = new Map([
+    var d = yi.SHOW_ALL,
+        c = yi.SHOW_CHILD,
+        p = yi.SHOW_PARENT,
+        ji = new Map([
             ["show-all", d],
             ["show-child", c],
             ["show-parent", p]
         ]),
         d = {
             title: n.a.string.isRequired,
             key: n.a.string.isRequired,
@@ -112839,15 +112920,15 @@
             disabled: n.a.bool,
             checkable: n.a.bool,
             disableCheckbox: n.a.bool,
             selectable: n.a.bool,
             isLeaf: n.a.bool,
             parent: n.a.string
         },
-        wi = (xi.propTypes = {
+        Mi = (wi.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             locale: n.a.oneOf(["zh-cn", "en-us"]),
             treeDataMode: n.a.oneOf(["tree", "flat"]),
             treeData: n.a.oneOfType([p, n.a.arrayOf(d)]).isRequired,
@@ -112882,15 +112963,15 @@
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func,
             persistence: n.a.oneOfType([n.a.bool, n.a.string, n.a.number]),
             persisted_props: n.a.arrayOf(n.a.oneOf(["value"])),
             persistence_type: n.a.oneOf(["local", "session", "memory"])
-        }, xi.defaultProps = {
+        }, wi.defaultProps = {
             listHeight: 256,
             virtual: !0,
             allowClear: !0,
             disabled: !1,
             bordered: !0,
             placement: "bottomLeft",
             treeLine: !1,
@@ -112903,38 +112984,38 @@
             persisted_props: ["value"],
             persistence_type: "local",
             locale: "zh-cn",
             treeNodeFilterProp: "value",
             treeDataMode: "tree",
             popupContainer: "body",
             showCheckedStrategy: "show-all"
-        }, xi),
-        ki = e(188),
-        ji = e(41),
-        Mi = Wt.createContext(null);
+        }, wi),
+        Ei = e(188),
+        Ci = e(41),
+        Si = Wt.createContext(null);
 
-    function Ei(t) {
-        return "string" == typeof t && String(Number(t)) === t ? (Object(de.a)(!1, "Invalid value type of `width` or `height` which should be number type instead."), Number(t)) : t
+    function Li(t) {
+        return "string" == typeof t && String(Number(t)) === t ? (Object(me.a)(!1, "Invalid value type of `width` or `height` which should be number type instead."), Number(t)) : t
     }
-    var Ci = {
+    var Pi = {
         width: 0,
         height: 0,
         overflow: "hidden",
         outline: "none",
         position: "absolute"
     };
 
-    function Si(t) {
+    function Di(t) {
         var e = t.width,
             n = t.height,
             a = void 0 === (r = t.size) ? "default" : r,
             r = void 0 === (r = t.closable) || r,
             o = void 0 === (o = t.mask) || o,
-            i = void 0 === (i = t.push) ? Ti : i,
-            l = void 0 === (l = t.closeIcon) ? Wt.createElement(Ze.a, null) : l,
+            i = void 0 === (i = t.push) ? Ri : i,
+            l = void 0 === (l = t.closeIcon) ? Wt.createElement(tn.a, null) : l,
             c = t.bodyStyle,
             s = t.drawerStyle,
             u = t.className,
             d = t.visible,
             p = t.open,
             f = t.children,
             h = t.style,
@@ -112944,15 +113025,15 @@
             v = t.footer,
             y = t.footerStyle,
             x = t.prefixCls,
             _ = t.getContainer,
             O = t.extra,
             w = t.afterVisibleChange,
             k = t.afterOpenChange,
-            t = Di(t, ["width", "height", "size", "closable", "mask", "push", "closeIcon", "bodyStyle", "drawerStyle", "className", "visible", "open", "children", "style", "title", "headerStyle", "onClose", "footer", "footerStyle", "prefixCls", "getContainer", "extra", "afterVisibleChange", "afterOpenChange"]),
+            t = Ai(t, ["width", "height", "size", "closable", "mask", "push", "closeIcon", "bodyStyle", "drawerStyle", "className", "visible", "open", "children", "style", "title", "headerStyle", "onClose", "footer", "footerStyle", "prefixCls", "getContainer", "extra", "afterVisibleChange", "afterOpenChange"]),
             j = (E = Wt.useContext(q.b)).getPopupContainer,
             M = E.getPrefixCls,
             E = E.direction,
             C = M("drawer", x),
             M = void 0 === _ && j ? function() {
                 return j(document.body)
             } : _,
@@ -112974,24 +113055,24 @@
             l = Wt.useMemo(function() {
                 return null != e ? e : "large" === a ? 736 : 378
             }, [e, a]),
             E = Wt.useMemo(function() {
                 return null != n ? n : "large" === a ? 736 : 378
             }, [n, a]),
             u = {
-                motionName: Object(Va.c)(C, "mask-motion"),
+                motionName: Object(Ga.c)(C, "mask-motion"),
                 motionAppear: !0,
                 motionEnter: !0,
                 motionLeave: !0,
                 motionDeadline: 500
             };
-        return Wt.createElement(Ga.a, null, Wt.createElement(ve.e, {
+        return Wt.createElement($a.a, null, Wt.createElement(Oe.e, {
             status: !0,
             override: !0
-        }, Wt.createElement(Pi, Object(Et.a)({
+        }, Wt.createElement(zi, Object(Et.a)({
             prefixCls: C,
             onClose: b
         }, t, {
             open: null != p ? p : d,
             mask: o,
             push: i,
             width: l,
@@ -113000,15 +113081,15 @@
             getContainer: M,
             afterOpenChange: function(t) {
                 null != k && k(t), null != w && w(t)
             },
             maskMotion: u,
             motion: function(t) {
                 return {
-                    motionName: Object(Va.c)(C, "panel-motion-".concat(t)),
+                    motionName: Object(Ga.c)(C, "panel-motion-".concat(t)),
                     motionAppear: !0,
                     motionEnter: !0,
                     motionLeave: !0,
                     motionDeadline: 500
                 }
             },
             rootStyle: h
@@ -113028,15 +113109,15 @@
             className: "".concat(C, "-body"),
             style: c
         }, f), v ? (b = "".concat(C, "-footer"), Wt.createElement("div", {
             className: b,
             style: y
         }, v)) : null))))
     }
-    var Li = Wt.forwardRef(function(t, e) {
+    var Ti = Wt.forwardRef(function(t, e) {
             var a = t.prefixCls,
                 r = t.open,
                 n = t.placement,
                 o = t.inline,
                 i = t.push,
                 l = t.forceRender,
                 c = t.autoFocus,
@@ -113067,15 +113148,15 @@
                     var t;
                     r && c && null != (t = E.current) && t.focus({
                         preventScroll: !0
                     })
                 }, [r]), Wt.useState(!1)),
                 t = (e = Object(Gt.a)(t, 2))[0],
                 L = e[1],
-                P = Wt.useContext(Mi),
+                P = Wt.useContext(Si),
                 D = null != (e = null != (i = null === (e = !1 === i ? {
                     distance: 0
                 } : !0 !== i && i || {}) ? void 0 : e.distance) ? i : null == P ? void 0 : P.pushDistance) ? e : 180,
                 i = Wt.useMemo(function() {
                     return {
                         pushDistance: D,
                         push: function() {
@@ -113090,15 +113171,15 @@
                     var t;
                     r ? null != P && null != (t = P.push) && t.call(P) : null != P && null != (t = P.pull) && t.call(P)
                 }, [r]), Wt.useEffect(function() {
                     return function() {
                         var t;
                         null != P && null != (t = P.pull) && t.call(P)
                     }
-                }, []), x && Wt.createElement(Er.b, Object(Et.a)({
+                }, []), x && Wt.createElement(Lr.b, Object(Et.a)({
                     key: "mask"
                 }, O, {
                     visible: r
                 }), function(t, e) {
                     var n = t.className,
                         t = t.style;
                     return Wt.createElement("div", {
@@ -113119,15 +113200,15 @@
                     break;
                 case "left":
                     T.transform = "translateX(".concat(D, "px)");
                     break;
                 default:
                     T.transform = "translateX(".concat(-D, "px)")
             }
-            return "left" === n || "right" === n ? T.width = Ei(g) : T.height = Ei(b), O = Wt.createElement(Er.b, Object(Et.a)({
+            return "left" === n || "right" === n ? T.width = Li(g) : T.height = Li(b), O = Wt.createElement(Lr.b, Object(Et.a)({
                 key: "panel"
             }, x, {
                 visible: r,
                 forceRender: l,
                 onVisibleChanged: function(t) {
                     null != j && j(t)
                 },
@@ -113135,21 +113216,21 @@
                 leavedClassName: "".concat(a, "-content-wrapper-hidden")
             }), function(t, e) {
                 var n = t.className,
                     t = t.style;
                 return Wt.createElement("div", {
                     className: Kt()("".concat(a, "-content-wrapper"), n),
                     style: Object(Ct.a)(Object(Ct.a)(Object(Ct.a)({}, T), t), y)
-                }, Wt.createElement(_i, {
+                }, Wt.createElement(ki, {
                     containerRef: e,
                     prefixCls: a,
                     className: f,
                     style: h
                 }, v))
-            }), m = Object(Ct.a)({}, d), p && (m.zIndex = p), Wt.createElement(Mi.Provider, {
+            }), m = Object(Ct.a)({}, d), p && (m.zIndex = p), Wt.createElement(Si.Provider, {
                 value: i
             }, Wt.createElement("div", {
                 className: Kt()(a, "".concat(a, "-").concat(n), u, (t = {}, Object(Vt.a)(t, "".concat(a, "-open"), r), Object(Vt.a)(t, "".concat(a, "-inline"), o), t)),
                 style: m,
                 tabIndex: -1,
                 ref: E,
                 onKeyDown: function(t) {
@@ -113166,26 +113247,26 @@
                         case X.a.ESC:
                             M && s && (t.stopPropagation(), M(t))
                     }
                 }
             }, e, Wt.createElement("div", {
                 tabIndex: 0,
                 ref: C,
-                style: Ci,
+                style: Pi,
                 "aria-hidden": "true",
                 "data-sentinel": "start"
             }), O, Wt.createElement("div", {
                 tabIndex: 0,
                 ref: S,
-                style: Ci,
+                style: Pi,
                 "aria-hidden": "true",
                 "data-sentinel": "end"
             })))
         }),
-        Pi = function(t) {
+        zi = function(t) {
             var e = t.open,
                 e = void 0 !== e && e,
                 n = t.prefixCls,
                 n = void 0 === n ? "rc-drawer" : n,
                 a = t.placement,
                 a = void 0 === a ? "right" : a,
                 r = t.autoFocus,
@@ -113206,20 +113287,20 @@
                 f = Object(Gt.a)(f, 2),
                 h = f[0],
                 m = f[1],
                 f = Wt.useState(!1),
                 f = Object(Gt.a)(f, 2),
                 g = f[0],
                 b = f[1],
-                v = (Object(ji.a)(function() {
+                v = (Object(Ci.a)(function() {
                     b(!0)
                 }, []), !!g && e),
                 y = Wt.useRef(),
                 x = Wt.useRef();
-            return Object(ji.a)(function() {
+            return Object(Ci.a)(function() {
                 v && (x.current = document.activeElement)
             }, [v]), u || h || v || !p ? (f = Object(Ct.a)(Object(Ct.a)({}, t), {}, {
                 open: v,
                 prefixCls: n,
                 placement: a,
                 autoFocus: r,
                 keyboard: o,
@@ -113227,76 +113308,76 @@
                 mask: l,
                 maskClosable: c,
                 inline: !1 === s,
                 afterOpenChange: function(t) {
                     m(t), null != d && d(t), t || !x.current || null != (t = y.current) && t.contains(x.current) || null == (t = x.current) || t.focus()
                 },
                 ref: y
-            }), Wt.createElement(ki.a, {
+            }), Wt.createElement(Ei.a, {
                 open: v || u || h,
                 autoDestroy: !1,
                 getContainer: s,
                 autoLock: l && (v || h)
-            }, Wt.createElement(Li, f))) : null
+            }, Wt.createElement(Ti, f))) : null
         },
-        Di = function(t, e) {
+        Ai = function(t, e) {
             var n = {};
             for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
             if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                 for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
             return n
         },
-        Ti = (Object(l.a)("default", "large"), {
+        Ri = (Object(l.a)("default", "large"), {
             distance: 180
         });
 
-    function zi(t) {
-        return (zi = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
+    function Ii(t) {
+        return (Ii = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
             return typeof t
         } : function(t) {
             return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
         })(t)
     }
 
-    function Ai(e, t) {
+    function Ni(e, t) {
         var n, a = Object.keys(e);
         return Object.getOwnPropertySymbols && (n = Object.getOwnPropertySymbols(e), t && (n = n.filter(function(t) {
             return Object.getOwnPropertyDescriptor(e, t).enumerable
         })), a.push.apply(a, n)), a
     }
 
-    function Ri(a) {
+    function Yi(a) {
         for (var t = 1; t < arguments.length; t++) {
             var r = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? Ai(Object(r), !0).forEach(function(t) {
+            t % 2 ? Ni(Object(r), !0).forEach(function(t) {
                 var e, n;
                 e = a, t = r[n = t], (n = function() {
                     var t = function(t) {
-                        if ("object" !== zi(t) || null === t) return t;
+                        if ("object" !== Ii(t) || null === t) return t;
                         var e = t[Symbol.toPrimitive];
                         if (void 0 === e) return String(t);
                         e = e.call(t, "string");
-                        if ("object" !== zi(e)) return e;
+                        if ("object" !== Ii(e)) return e;
                         throw new TypeError("@@toPrimitive must return a primitive value.")
                     }(n);
-                    return "symbol" === zi(t) ? t : String(t)
+                    return "symbol" === Ii(t) ? t : String(t)
                 }()) in e ? Object.defineProperty(e, n, {
                     value: t,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : e[n] = t
-            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(r)) : Ai(Object(r)).forEach(function(t) {
+            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(r)) : Ni(Object(r)).forEach(function(t) {
                 Object.defineProperty(a, t, Object.getOwnPropertyDescriptor(r, t))
             })
         }
         return a
     }
 
-    function Ii(t) {
+    function Bi(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.visible,
             l = t.title,
@@ -113309,18 +113390,18 @@
             h = t.mask,
             m = t.maskClosable,
             g = t.width,
             b = t.zIndex,
             v = t.extra,
             y = t.setProps,
             t = t.loading_state;
-        return H.a.createElement(Si, {
+        return H.a.createElement(Di, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
-            style: p ? Ri(Ri({}, r), {
+            style: p ? Yi(Yi({}, r), {
                 position: "absolute"
             }) : r,
             key: o,
             open: i,
             title: l,
             placement: c,
             closable: s,
@@ -113340,15 +113421,15 @@
                     visible: !1
                 })
             },
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
 
-    function Ni(t) {
+    function Fi(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.title,
             l = t.content,
@@ -113360,15 +113441,15 @@
             f = t.overlayStyle,
             h = t.overlayInnerStyle,
             m = t.trigger,
             g = t.zIndex,
             b = t.popupContainer,
             t = t.loading_state,
             n = j(n);
-        return H.a.createElement(To.a, {
+        return H.a.createElement(Ro.a, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             title: i && i.content ? H.a.createElement("div", null, H.a.createElement(I.a, {
                 icon: i.prefixIcon
             }), H.a.createElement("span", {
@@ -113389,41 +113470,41 @@
             getPopupContainer: "parent" === b ? function(t) {
                 return t.parentNode
             } : void 0,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
 
-    function Yi(t) {
+    function Hi(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.locale,
             l = t.description,
             c = t.image,
             s = t.imageStyle,
             t = (t.setProps, t.loading_state),
             u = Object(Wt.useContext)(G.a),
             i = u && u.locale || i;
         return H.a.createElement(W.a, {
             locale: K.b.get(i)
-        }, H.a.createElement(Hi.a, {
+        }, H.a.createElement(Ki.a, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             description: l,
-            image: Wi.get(c) || c,
+            image: Ui.get(c) || c,
             imageStyle: s,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n))
     }
-    Ii.propTypes = {
+    Bi.propTypes = {
         id: n.a.string,
         children: n.a.node,
         className: n.a.oneOfType([n.a.string, n.a.object]),
         style: n.a.object,
         key: n.a.string,
         visible: n.a.bool,
         title: n.a.node,
@@ -113440,28 +113521,28 @@
         containerId: n.a.string,
         loading_state: n.a.shape({
             is_loading: n.a.bool,
             prop_name: n.a.string,
             component_name: n.a.string
         }),
         setProps: n.a.func
-    }, Ii.defaultProps = {
+    }, Bi.defaultProps = {
         visible: !1,
         placement: "right",
         closable: !0,
         forceRender: !1,
         destroyOnClose: !1,
         width: 256,
         height: 256,
         mask: !0,
         maskClosable: !0,
         zIndex: 1e3
     };
-    var Bi = Ii,
-        Fi = (Ni.propTypes = {
+    var Wi = Bi,
+        Vi = (Fi.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             title: n.a.node,
             content: n.a.node,
@@ -113478,28 +113559,28 @@
             popupContainer: n.a.oneOf(["parent", "body"]),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, Ni.defaultProps = {
+        }, Fi.defaultProps = {
             mouseEnterDelay: .1,
             mouseLeaveDelay: .1,
             placement: "top",
             trigger: "hover",
             arrowPointAtCenter: !1,
             popupContainer: "body"
-        }, Ni),
-        Hi = e(134),
-        Wi = new Map([
-            ["default", Hi.a.PRESENTED_IMAGE_DEFAULT],
-            ["simple", Hi.a.PRESENTED_IMAGE_SIMPLE]
+        }, Fi),
+        Ki = e(134),
+        Ui = new Map([
+            ["default", Ki.a.PRESENTED_IMAGE_DEFAULT],
+            ["simple", Ki.a.PRESENTED_IMAGE_SIMPLE]
         ]),
-        Vi = (Yi.propTypes = {
+        Gi = (Hi.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             locale: n.a.oneOf(["zh-cn", "en-us"]),
             description: n.a.oneOfType([n.a.node, n.a.bool]),
@@ -113507,47 +113588,47 @@
             imageStyle: n.a.object,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, Yi.defaultProps = {
+        }, Hi.defaultProps = {
             locale: "zh-cn",
             image: "default"
-        }, Yi),
-        Ki = Wt.createContext(null);
+        }, Hi),
+        qi = Wt.createContext(null);
 
-    function Ui(t) {
+    function Xi(t) {
         return t.join("__RC_CASCADER_SPLIT__")
     }
 
-    function Gi(t) {
-        return t.map(Ui)
+    function $i(t) {
+        return t.map(Xi)
     }
 
-    function qi(t, e) {
+    function Zi(t, e) {
         var n;
         return null != (n = t.isLeaf) ? n : !(null != (n = t[e.children]) && n.length)
     }
 
-    function Xi(t, e, n) {
+    function Ji(t, e, n) {
         var a = new Set(t),
             r = e();
         return t.filter(function(t) {
             var t = r[t],
                 e = t ? t.parent : null,
                 t = t ? t.children : null;
             return "SHOW_CHILD" === n ? !(t && t.some(function(t) {
                 return t.key && a.has(t.key)
             })) : !(e && !e.node.disabled && a.has(e.key))
         })
     }
 
-    function $i(r, t, o, e) {
+    function Qi(r, t, o, e) {
         for (var i = 3 < arguments.length && void 0 !== e && e, l = t, c = [], s = 0; s < r.length; s += 1) ! function() {
             var t, e = r[s],
                 n = null == (n = l) ? void 0 : n.findIndex(function(t) {
                     t = t[o.value];
                     return i ? String(t) === String(e) : t === e
                 }),
                 a = -1 !== n ? null == (a = l) ? void 0 : a[n] : null;
@@ -113556,83 +113637,83 @@
                 index: n,
                 option: a
             }), l = null == a ? void 0 : a[o.children]
         }();
         return c
     }
 
-    function Zi(t) {
+    function tl(t) {
         var e = Wt.useRef();
         return e.current = t, Wt.useCallback(function() {
             return e.current.apply(e, arguments)
         }, [])
     }
 
-    function Ji(e, t, n) {
+    function el(e, t, n) {
         var a = n.label;
         return t.some(function(t) {
             return String(t[a]).toLowerCase().includes(e.toLowerCase())
         })
     }
 
-    function Qi(t, e, n, a) {
+    function nl(t, e, n, a) {
         return e.map(function(t) {
             return t[a.label]
         }).join(" / ")
     }
-    var tl = "__rc_cascader_search_mark__";
+    var al = "__rc_cascader_search_mark__";
 
-    function el(t) {
+    function rl(t) {
         var e, n = t.prefixCls,
             a = t.checked,
             r = t.halfChecked,
             o = t.disabled,
             t = t.onClick,
-            i = Wt.useContext(Ki).checkable,
+            i = Wt.useContext(qi).checkable,
             i = "boolean" != typeof i ? i : null;
         return Wt.createElement("span", {
             className: Kt()("".concat(n), (e = {}, Object(Vt.a)(e, "".concat(n, "-checked"), a), Object(Vt.a)(e, "".concat(n, "-indeterminate"), !a && r), Object(Vt.a)(e, "".concat(n, "-disabled"), o), e)),
             onClick: t
         }, i)
     }
 
-    function nl(t) {
+    function ol(t) {
         var h = t.prefixCls,
             m = t.multiple,
             e = t.options,
             g = t.activeValue,
             l = t.prevValuePath,
             b = t.onToggleOpen,
             v = t.onSelect,
             y = t.onActive,
             c = t.checkedSet,
             s = t.halfCheckedSet,
             u = t.loadingKeys,
             x = t.isSelectable,
             t = "".concat(h, "-menu"),
             _ = "".concat(h, "-menu-item"),
-            n = Wt.useContext(Ki),
+            n = Wt.useContext(qi),
             d = n.fieldNames,
             O = n.changeOnSelect,
             a = n.expandTrigger,
             w = n.expandIcon,
             k = n.loadingIcon,
             j = n.dropdownMenuColumnStyle,
             M = "hover" === a,
             n = Wt.useMemo(function() {
                 return e.map(function(t) {
                     var e = t.disabled,
-                        n = t[tl],
+                        n = t[al],
                         a = null != (a = t.__cascader_fix_label__) ? a : t[d.label],
                         r = t[d.value],
-                        o = qi(t, d),
+                        o = Zi(t, d),
                         n = n ? n.map(function(t) {
                             return t[d.value]
                         }) : [].concat(Object(Ut.a)(l), [r]),
-                        i = Ui(n);
+                        i = Xi(n);
                     return {
                         disabled: e,
                         label: a,
                         value: r,
                         isLeaf: o,
                         isLoading: u.includes(i),
                         checked: c.has(i),
@@ -113681,15 +113762,15 @@
                 },
                 onMouseEnter: function() {
                     M && e()
                 },
                 onMouseDown: function(t) {
                     t.preventDefault()
                 }
-            }, m && Wt.createElement(el, {
+            }, m && Wt.createElement(rl, {
                 prefixCls: "".concat(h, "-checkbox"),
                 checked: u,
                 halfChecked: d,
                 disabled: o,
                 onClick: function(t) {
                     t.stopPropagation(), n()
                 }
@@ -113699,15 +113780,15 @@
                 className: "".concat(_, "-expand-icon")
             }, w), s && k && Wt.createElement("div", {
                 className: "".concat(_, "-loading-icon")
             }, k))
         }))
     }
 
-    function al(t, c, s, u, e, a) {
+    function il(t, c, s, u, e, a) {
         function o(t) {
             e(t)
         }
 
         function r() {
             var t;
             1 < m.length ? (t = m.slice(0, -1), o(t)) : d(!1)
@@ -113715,15 +113796,15 @@
 
         function i() {
             var t = ((null == (t = b[g]) ? void 0 : t[s.children]) || []).find(function(t) {
                 return !t.disabled
             });
             t && (t = [].concat(Object(Ut.a)(m), [t[s.value]]), o(t))
         }
-        var n = (h = Object(Uo.e)()).direction,
+        var n = (h = Object(Xo.e)()).direction,
             l = h.searchValue,
             d = h.toggleOpen,
             p = h.open,
             f = "rtl" === n,
             h = Wt.useMemo(function() {
                 for (var n = -1, a = c, r = [], o = [], t = u.length, e = 0; e < t && a && "break" !== function(e) {
                         var t = a.findIndex(function(t) {
@@ -113761,56 +113842,56 @@
                         case X.a.RIGHT:
                             (f ? r : i)();
                             break;
                         case X.a.BACKSPACE:
                             l || r();
                             break;
                         case X.a.ENTER:
-                            m.length && ((n = (null == (n = b[g]) ? void 0 : n[tl]) || []).length ? a(n.map(function(t) {
+                            m.length && ((n = (null == (n = b[g]) ? void 0 : n[al]) || []).length ? a(n.map(function(t) {
                                 return t[s.value]
                             }), n[n.length - 1]) : a(m, b[g]));
                             break;
                         case X.a.ESC:
                             d(!1), p && t.stopPropagation()
                     }
                 },
                 onKeyUp: function() {}
             }
         })
     }
-    var rl = Wt.forwardRef(function(t, e) {
+    var ll = Wt.forwardRef(function(t, e) {
             function n(t) {
                 var e, n, a;
-                D(t), t = t, j && !p && (n = (e = $i(t, b, x).map(function(t) {
+                D(t), t = t, j && !p && (n = (e = Qi(t, b, x).map(function(t) {
                     return t.option
-                }))[e.length - 1]) && !qi(n, x) && (a = Ui(t), S(function(t) {
+                }))[e.length - 1]) && !Zi(n, x) && (a = Xi(t), S(function(t) {
                     return [].concat(Object(Ut.a)(t), [a])
                 }), j(e))
             }
 
             function a(t) {
                 var e = t.disabled,
-                    t = qi(t, x);
+                    t = Zi(t, x);
                 return !e && (t || _ || d)
             }
 
             function r(t, e) {
                 var n = 2 < arguments.length && void 0 !== arguments[2] && arguments[2];
                 O(t), !d && (e || _ && ("hover" === M || n)) && f(!1)
             }
-            var o, i, l, c, s = Object(Uo.e)(),
+            var o, i, l, c, s = Object(Xo.e)(),
                 u = s.prefixCls,
                 d = s.multiple,
                 p = s.searchValue,
                 f = s.toggleOpen,
                 h = s.notFoundContent,
                 s = s.direction,
                 m = Wt.useRef(),
                 s = "rtl" === s,
-                g = Wt.useContext(Ki),
+                g = Wt.useContext(qi),
                 b = g.options,
                 v = g.values,
                 y = g.halfValues,
                 x = g.fieldNames,
                 _ = g.changeOnSelect,
                 O = g.onSelect,
                 w = g.searchOptions,
@@ -113820,31 +113901,31 @@
                 E = k || u,
                 g = Wt.useState([]),
                 k = Object(Gt.a)(g, 2),
                 C = k[0],
                 S = k[1],
                 u = (Wt.useEffect(function() {
                     C.length && C.forEach(function(e) {
-                        var t = $i(e.split("__RC_CASCADER_SPLIT__"), b, x, !0).map(function(t) {
+                        var t = Qi(e.split("__RC_CASCADER_SPLIT__"), b, x, !0).map(function(t) {
                                 return t.option
                             }),
                             t = t[t.length - 1];
-                        t && !t[x.children] && !qi(t, x) || S(function(t) {
+                        t && !t[x.children] && !Zi(t, x) || S(function(t) {
                             return t.filter(function(t) {
                                 return t !== e
                             })
                         })
                     })
                 }, [b, C, x]), Wt.useMemo(function() {
-                    return new Set(Gi(v))
+                    return new Set($i(v))
                 }, [v])),
                 g = Wt.useMemo(function() {
-                    return new Set(Gi(y))
+                    return new Set($i(y))
                 }, [y]),
-                k = (k = Object(Uo.e)(), o = k.multiple, i = k.open, l = Wt.useContext(Ki).values, k = Wt.useState([]), k = Object(Gt.a)(k, 2), L = k[0], c = k[1], Wt.useEffect(function() {
+                k = (k = Object(Xo.e)(), o = k.multiple, i = k.open, l = Wt.useContext(qi).values, k = Wt.useState([]), k = Object(Gt.a)(k, 2), L = k[0], c = k[1], Wt.useEffect(function() {
                     var t;
                     i && !o && (t = l[0], c(t || []))
                 }, [i]), [L, c]),
                 L = Object(Gt.a)(k, 2),
                 P = L[0],
                 D = L[1],
                 T = Wt.useMemo(function() {
@@ -113862,19 +113943,19 @@
                             if (null == t || !t.length) return "break";
                             a = t, n.push({
                                 options: t
                             })
                         }(); r += 1);
                     return n
                 }, [T, P, x]),
-                L = (al(e, T, x, P, n, function(t, e) {
-                    a(e) && r(t, qi(e, x), !0)
+                L = (il(e, T, x, P, n, function(t, e) {
+                    a(e) && r(t, Zi(e, x), !0)
                 }), Wt.useEffect(function() {
                     for (var t, e = 0; e < P.length; e += 1) {
-                        var n = Ui(P.slice(0, e + 1)),
+                        var n = Xi(P.slice(0, e + 1)),
                             a = null == (a = m.current) ? void 0 : a.querySelector('li[data-path-key="'.concat(n.replace(/\\{0,2}"/g, '\\"'), '"]'));
                         a && (t = n = void 0, t = (a = a).parentElement) && ((n = a.offsetTop - t.offsetTop) - t.scrollTop < 0 ? t.scrollTo({
                             top: n
                         }) : n + a.offsetHeight - t.scrollTop > t.offsetHeight && t.scrollTo({
                             top: n + a.offsetHeight - t.offsetHeight
                         }))
                     }
@@ -113891,38 +113972,38 @@
                     isSelectable: a
                 }),
                 e = (L ? [{
                     options: h
                 }] : k).map(function(t, e) {
                     var n = P.slice(0, e),
                         a = P[e];
-                    return Wt.createElement(nl, Object(Et.a)({
+                    return Wt.createElement(ol, Object(Et.a)({
                         key: e
                     }, z, {
                         prefixCls: E,
                         options: t.options,
                         prevValuePath: n,
                         activeValue: a
                     }))
                 });
             return Wt.createElement("div", {
                 className: Kt()("".concat(E, "-menus"), (t = {}, Object(Vt.a)(t, "".concat(E, "-menu-empty"), L), Object(Vt.a)(t, "".concat(E, "-rtl"), s), t)),
                 ref: m
             }, e)
         }),
-        ol = ["id", "prefixCls", "fieldNames", "defaultValue", "value", "changeOnSelect", "onChange", "displayRender", "checkable", "searchValue", "onSearch", "showSearch", "expandTrigger", "options", "dropdownPrefixCls", "loadData", "popupVisible", "open", "popupClassName", "dropdownClassName", "dropdownMenuColumnStyle", "popupPlacement", "placement", "onDropdownVisibleChange", "onPopupVisibleChange", "expandIcon", "loadingIcon", "children", "dropdownMatchSelectWidth", "showCheckedStrategy"];
+        cl = ["id", "prefixCls", "fieldNames", "defaultValue", "value", "changeOnSelect", "onChange", "displayRender", "checkable", "searchValue", "onSearch", "showSearch", "expandTrigger", "options", "dropdownPrefixCls", "loadData", "popupVisible", "open", "popupClassName", "dropdownClassName", "dropdownMenuColumnStyle", "popupPlacement", "placement", "onDropdownVisibleChange", "onPopupVisibleChange", "expandIcon", "loadingIcon", "children", "dropdownMatchSelectWidth", "showCheckedStrategy"];
 
-    function il(t) {
+    function sl(t) {
         return t ? (e = t, Array.isArray(e) && Array.isArray(e[0]) ? t : (0 === t.length ? [] : [t]).map(function(t) {
             return Array.isArray(t) ? t : [t]
         })) : [];
         var e
     }
 
-    function ll(t, e, n, c) {
+    function ul(t, e, n, c) {
         var s = [],
             u = t.toLowerCase();
         return e.forEach(function(t, e) {
             0 !== e && s.push(" / ");
             var a, r, o, i, l, e = t[c.label],
                 t = Object(qt.a)(e);
             "string" !== t && "number" !== t || (a = String(e), r = u, o = n, t = a.toLowerCase().split(r).reduce(function(t, e, n) {
@@ -113934,15 +114015,15 @@
                     className: "".concat(o, "-menu-item-keyword"),
                     key: "seperator-".concat(e)
                 }, n)), i.push(n)
             }), e = i), s.push(e)
         }), s
     }
 
-    function cl(t) {
+    function dl(t) {
         var e = t.id,
             n = t.style,
             a = t.className,
             r = t.key,
             o = t.locale,
             i = t.options,
             l = t.optionsMode,
@@ -113974,15 +114055,15 @@
                     value: f
                 })
             }, []), Object(Wt.useMemo)(function() {
                 return B(i)
             }, [i]));
         return "flat" === l && (i = S), React.createElement(W.a, {
             locale: K.b.get(o)
-        }, React.createElement(vl, {
+        }, React.createElement(_l, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: n,
             key: r,
             options: i,
             changeOnSelect: c,
             size: C && !Object(V.isUndefined)(C.componentSize) ? C.componentSize : s,
@@ -113996,15 +114077,15 @@
             multiple: b,
             persistence: j,
             persisted_props: M,
             persistence_type: E,
             expandTrigger: v,
             status: y,
             allowClear: Object(V.isUndefined)(w) ? x : !w,
-            showCheckedStrategy: yl.get(_),
+            showCheckedStrategy: Ol.get(_),
             showSearch: function(e, t) {
                 return t.some(function(t) {
                     return -1 < t.label.toLowerCase().indexOf(e.toLowerCase())
                 })
             },
             onChange: function(t) {
                 k({
@@ -114015,15 +114096,15 @@
             getPopupContainer: "parent" === O ? function(t) {
                 return t.parentNode
             } : void 0,
             open: !(!Object(V.isUndefined)(w) && w) && void 0
         }))
     }
 
-    function sl(t) {
+    function pl(t) {
         function e(t) {
             h({
                 value: t.target.value
             })
         }
         var n = t.id,
             a = t.style,
@@ -114043,40 +114124,40 @@
             b = t.persistence_type,
             t = t.loading_state,
             v = Object(Wt.useContext)(G.a);
         return Object(Wt.useEffect)(function() {
             l && !c && h({
                 value: l
             })
-        }, []), "vertical" === s ? H.a.createElement(_l.a.Group, {
+        }, []), "vertical" === s ? H.a.createElement(kl.a.Group, {
             id: n,
             className: Object(V.isString)(r) ? r : r ? Object(U.a)(r) : void 0,
             style: a,
             key: o,
             defaultValue: l,
             value: c,
             buttonStyle: d,
             disabled: v && !Object(V.isUndefined)(v.componentDisabled) ? v.componentDisabled : p,
             size: v && !Object(V.isUndefined)(v.componentSize) ? v.componentSize : f,
             persistence: m,
             persisted_props: g,
             persistence_type: b,
             onChange: e,
             "data-dash-is-loading": t && t.is_loading || void 0
-        }, H.a.createElement(za.b, {
+        }, H.a.createElement(Ia.b, {
             direction: "vertical"
         }, i.map(function(t) {
-            return "button" !== u ? H.a.createElement(_l.a, {
+            return "button" !== u ? H.a.createElement(kl.a, {
                 value: t.value,
                 disabled: t.disabled
-            }, t.label) : H.a.createElement(_l.a.Button, {
+            }, t.label) : H.a.createElement(kl.a.Button, {
                 value: t.value,
                 disabled: t.disabled
             }, t.label)
-        }))) : H.a.createElement(_l.a.Group, {
+        }))) : H.a.createElement(kl.a.Group, {
             id: n,
             className: Object(V.isString)(r) ? r : r ? Object(U.a)(r) : void 0,
             style: a,
             key: o,
             options: i,
             defaultValue: l,
             value: c,
@@ -114088,15 +114169,15 @@
             persisted_props: g,
             persistence_type: b,
             onChange: e,
             "data-dash-is-loading": t && t.is_loading || void 0
         })
     }
 
-    function ul(t) {
+    function fl(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.locale,
             l = t.title,
@@ -114118,15 +114199,15 @@
             w = t.setProps,
             t = t.loading_state,
             k = Object(Wt.useContext)(G.a),
             i = k && k.locale || i,
             n = j(n);
         return H.a.createElement(W.a, {
             locale: K.b.get(i)
-        }, H.a.createElement(wl.a, {
+        }, H.a.createElement(Ml.a, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             title: l,
             disabled: k && !Object(V.isUndefined)(k.componentDisabled) ? k.componentDisabled : c,
             placement: s,
@@ -114153,55 +114234,55 @@
                     confirmCounts: y + 1
                 })
             },
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n))
     }
 
-    function dl(t, e) {
-        return Wt.createElement(to.a, Object(Ct.a)(Object(Ct.a)({}, t), {}, {
+    function hl(t, e) {
+        return Wt.createElement(ao.a, Object(Ct.a)(Object(Ct.a)({}, t), {}, {
             ref: e,
-            icon: jl
+            icon: Cl
         }))
     }
 
-    function pl(t) {
+    function ml(t) {
         var e = t.prefixCls,
             n = t.rootPrefixCls,
             a = t.children,
             t = t.visible,
             r = Wt.createElement("div", {
                 className: "".concat(e, "-content")
             }, Wt.createElement("div", {
                 className: "".concat(e, "-icon")
-            }, Wt.createElement(Ml, null)));
-        return Wt.createElement(Er.b, {
+            }, Wt.createElement(Sl, null)));
+        return Wt.createElement(Lr.b, {
             visible: t,
             motionName: "".concat(n, "-fade")
         }, function(t) {
             var e = t.className;
-            return Object(je.a)(a || r, function(t) {
+            return Object(Ce.a)(a || r, function(t) {
                 t = t.className;
                 return {
                     className: Kt()(e, t)
                 }
             })
         })
     }
 
-    function fl(t) {
+    function gl(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.duration,
             i = t.visibilityHeight,
             l = t.containerId,
             t = (t.setProps, t.loading_state);
-        return H.a.createElement(El, {
+        return H.a.createElement(Ll, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             target: l ? function() {
                 return document.getElementById(l)
             } : function() {
@@ -114209,15 +114290,15 @@
             },
             duration: 1e3 * o,
             visibilityHeight: i,
             "data-dash-is-loading": t && t.is_loading || void 0
         })
     }
 
-    function hl(t) {
+    function bl(t) {
         var e = t.prefixCls,
             n = t.className,
             a = t.style,
             r = t.size,
             t = t.shape,
             o = Kt()((o = {}, Object(Vt.a)(o, "".concat(e, "-lg"), "large" === r), Object(Vt.a)(o, "".concat(e, "-sm"), "small" === r), o)),
             t = Kt()((i = {}, Object(Vt.a)(i, "".concat(e, "-circle"), "circle" === t), Object(Vt.a)(i, "".concat(e, "-square"), "square" === t), Object(Vt.a)(i, "".concat(e, "-round"), "round" === t), i)),
@@ -114230,15 +114311,15 @@
             }, [r]);
         return Wt.createElement("span", {
             className: Kt()(e, o, t, n),
             style: Object(Et.a)(Object(Et.a)({}, i), a)
         })
     }
 
-    function ml(r) {
+    function vl(r) {
         var t = r.prefixCls,
             e = r.className,
             n = r.style,
             a = r.rows,
             a = Object(Ut.a)(Array(a)).map(function(t, e) {
                 return Wt.createElement("li", {
                     key: e,
@@ -114250,15 +114331,15 @@
             });
         return Wt.createElement("ul", {
             className: Kt()(t, e),
             style: n
         }, a)
     }
 
-    function gl(t) {
+    function yl(t) {
         var e = t.prefixCls,
             n = t.className,
             a = t.width,
             t = t.style;
         return Wt.createElement("h3", {
             className: Kt()(e, n),
             style: Object(Et.a)({
@@ -114297,20 +114378,20 @@
                 et = void 0 === C ? ">" : C,
                 nt = t.loadingIcon,
                 at = t.children,
                 C = t.dropdownMatchSelectWidth,
                 C = void 0 !== C && C,
                 rt = t.showCheckedStrategy,
                 ot = void 0 === rt ? "SHOW_PARENT" : rt,
-                rt = Object(Bt.a)(t, ol),
-                t = Object(qo.a)(_),
+                rt = Object(Jt.a)(t, cl),
+                t = Object(Zo.a)(_),
                 S = !!B,
-                _ = Object($t.a)(w, {
+                _ = Object(Zt.a)(w, {
                     value: k,
-                    postState: il
+                    postState: sl
                 }),
                 w = Object(Gt.a)(_, 2),
                 it = w[0],
                 lt = w[1],
                 L = Wt.useMemo(function() {
                     return e = (t = I || {}).label, n = t.value || "value", {
                         label: e || "label",
@@ -114323,15 +114404,15 @@
                 P = Wt.useMemo(function() {
                     return W || []
                 }, [W]),
                 D = (v = P, y = L, x = Wt.useRef({
                     options: null,
                     info: null
                 }), Wt.useCallback(function() {
-                    return x.current.options !== v && (x.current.options = v, x.current.info = Object(si.a)(v, {
+                    return x.current.options !== v && (x.current.options = v, x.current.info = Object(pi.a)(v, {
                         fieldNames: y,
                         initWrapper: function(t) {
                             return Object(Ct.a)(Object(Ct.a)({}, t), {}, {
                                 pathKeyEntities: {}
                             })
                         },
                         processEntity: function(t, e) {
@@ -114346,15 +114427,15 @@
                     var e = D();
                     return t.map(function(t) {
                         return e[t].nodes.map(function(t) {
                             return t[L.value]
                         })
                     })
                 }, [D, L]),
-                k = Object($t.a)("", {
+                k = Object(Zt.a)("", {
                     value: M,
                     postState: function(t) {
                         return t || ""
                     }
                 }),
                 _ = Object(Gt.a)(k, 2),
                 w = _[0],
@@ -114365,101 +114446,101 @@
                         matchInputWidth: !0,
                         limit: 50
                     }, (t = b && "object" === Object(qt.a)(b) ? Object(Ct.a)(Object(Ct.a)({}, t), b) : t).limit <= 0 && delete t.limit, [!0, t]) : [!1, {}]
                 }, [b])),
                 k = Object(Gt.a)(M, 2),
                 _ = k[0],
                 E = k[1],
-                st = (c = w, s = P, u = L, d = V || O, p = j, M = E.filter, f = void 0 === M ? Ji : M, M = E.render, h = void 0 === M ? Qi : M, M = E.limit, m = void 0 === M ? 50 : M, g = E.sort, Wt.useMemo(function() {
+                st = (c = w, s = P, u = L, d = V || O, p = j, M = E.filter, f = void 0 === M ? el : M, M = E.render, h = void 0 === M ? nl : M, M = E.limit, m = void 0 === M ? 50 : M, g = E.sort, Wt.useMemo(function() {
                     var i = [];
                     return c ? (function r(t, o) {
                         t.forEach(function(t) {
                             var e, n, a;
                             !g && 0 < m && m <= i.length || (n = [].concat(Object(Ut.a)(o), [t]), (a = t[u.children]) && 0 !== a.length && !p || f(c, n, {
                                 label: u.label
-                            }) && i.push(Object(Ct.a)(Object(Ct.a)({}, t), {}, (e = {}, Object(Vt.a)(e, u.label, h(c, n, d, u)), Object(Vt.a)(e, tl, n), Object(Vt.a)(e, u.children, void 0), e))), a && r(t[u.children], n))
+                            }) && i.push(Object(Ct.a)(Object(Ct.a)({}, t), {}, (e = {}, Object(Vt.a)(e, u.label, h(c, n, d, u)), Object(Vt.a)(e, al, n), Object(Vt.a)(e, u.children, void 0), e))), a && r(t[u.children], n))
                         })
                     }(s, []), g && i.sort(function(t, e) {
-                        return g(t[tl], e[tl], c, u)
+                        return g(t[al], e[al], c, u)
                     }), 0 < m ? i.slice(0, m) : i) : []
                 }, [c, s, u, d, h, p, f, g, m])),
                 ut = (r = P, l = L, Wt.useCallback(function(t) {
                     var e = [],
                         n = [];
                     return t.forEach(function(t) {
-                        ($i(t, r, l).every(function(t) {
+                        (Qi(t, r, l).every(function(t) {
                             return t.option
                         }) ? n : e).push(t)
                     }), [n, e]
                 }, [r, l])),
                 k = Wt.useMemo(function() {
                     var t, e, n = ut(it),
                         n = Object(Gt.a)(n, 2),
                         a = n[0],
                         n = n[1];
-                    return S && it.length ? (e = Gi(a), t = D(), t = (e = Object(Go.a)(e, !0, t)).checkedKeys, e = e.halfCheckedKeys, [T(t), T(e), n]) : [a, [], n]
+                    return S && it.length ? (e = $i(a), t = D(), t = (e = Object($o.a)(e, !0, t)).checkedKeys, e = e.halfCheckedKeys, [T(t), T(e), n]) : [a, [], n]
                 }, [S, it, D, T, ut]),
                 M = Object(Gt.a)(k, 3),
                 z = M[0],
                 dt = M[1],
                 A = M[2],
                 k = (e = Wt.useMemo(function() {
-                    var t = Xi(Gi(z), D, ot);
+                    var t = Ji($i(z), D, ot);
                     return [].concat(Object(Ut.a)(A), Object(Ut.a)(T(t)))
                 }, [z, D, T, A, ot]), o = P, i = L, n = S, a = Y, Wt.useMemo(function() {
                     var r = a || function(t) {
                         t = n ? t.slice(-1) : t;
                         return t.every(function(t) {
                             return ["string", "number"].includes(Object(qt.a)(t))
                         }) ? t.join(" / ") : t.reduce(function(t, e, n) {
                             e = Wt.isValidElement(e) ? Wt.cloneElement(e, {
                                 key: n
                             }) : e;
                             return 0 === n ? [e] : [].concat(Object(Ut.a)(t), [" / ", e])
                         }, [])
                     };
                     return e.map(function(t) {
-                        var e = $i(t, o, i),
+                        var e = Qi(t, o, i),
                             n = r(e.map(function(t) {
                                 var e = t.option,
                                     t = t.value;
                                 return null != (e = null == e ? void 0 : e[i.label]) ? e : t
                             }), e.map(function(t) {
                                 return t.option
                             })),
-                            a = Ui(t);
+                            a = Xi(t);
                         return {
                             label: n,
                             value: a,
                             key: a,
                             valueCells: t,
                             disabled: null == (n = e[e.length - 1]) || null == (a = n.option) ? void 0 : a.disabled
                         }
                     })
                 }, [e, o, i, a, n])),
-                pt = Zi(function(t) {
+                pt = tl(function(t) {
                     var e;
-                    lt(t), N && (e = (t = il(t)).map(function(t) {
-                        return $i(t, P, L).map(function(t) {
+                    lt(t), N && (e = (t = sl(t)).map(function(t) {
+                        return Qi(t, P, L).map(function(t) {
                             return t.option
                         })
                     }), t = S ? t : t[0], e = S ? e : e[0], N(t, e))
                 }),
-                ft = Zi(function(t) {
+                ft = tl(function(t) {
                     var e, n, a, r, o, i, l;
-                    ct(""), S ? (e = Ui(t), o = Gi(z), n = Gi(dt), i = o.includes(e), r = A.some(function(t) {
-                        return Ui(t) === e
+                    ct(""), S ? (e = Xi(t), o = $i(z), n = $i(dt), i = o.includes(e), r = A.some(function(t) {
+                        return Xi(t) === e
                     }), l = z, a = A, r && !i ? a = A.filter(function(t) {
-                        return Ui(t) !== e
+                        return Xi(t) !== e
                     }) : (r = i ? o.filter(function(t) {
                         return t !== e
-                    }) : [].concat(Object(Ut.a)(o), [e]), o = D(), i = Xi((i ? Object(Go.a)(r, {
+                    }) : [].concat(Object(Ut.a)(o), [e]), o = D(), i = Ji((i ? Object($o.a)(r, {
                         checked: !1,
                         halfCheckedKeys: n
-                    }, o) : Object(Go.a)(r, !0, o)).checkedKeys, D, ot), l = T(i)), pt([].concat(Object(Ut.a)(a), Object(Ut.a)(l)))) : pt(t)
+                    }, o) : Object($o.a)(r, !0, o)).checkedKeys, D, ot), l = T(i)), pt([].concat(Object(Ut.a)(a), Object(Ut.a)(l)))) : pt(t)
                 }),
                 M = void 0 !== G ? G : U,
                 Y = X || q,
                 G = J || Z,
                 U = Wt.useMemo(function() {
                     return {
                         options: P,
@@ -114478,17 +114559,17 @@
                         dropdownMenuColumnStyle: $
                     }
                 }, [P, L, z, dt, j, ft, B, st, V, K, H, et, nt, $]),
                 X = !(w ? st : P).length,
                 q = w && E.matchInputWidth || X ? {} : {
                     minWidth: "auto"
                 };
-            return Wt.createElement(Ki.Provider, {
+            return Wt.createElement(qi.Provider, {
                 value: U
-            }, Wt.createElement(Uo.a, Object(Et.a)({}, rt, {
+            }, Wt.createElement(Xo.a, Object(Et.a)({}, rt, {
                 ref: R,
                 id: t,
                 prefixCls: O,
                 dropdownMatchSelectWidth: C,
                 dropdownStyle: q,
                 displayValues: k,
                 onDisplayValuesChange: function(t, e) {
@@ -114496,30 +114577,30 @@
                 },
                 mode: S ? "multiple" : void 0,
                 searchValue: w,
                 onSearch: function(t, e) {
                     ct(t), "blur" !== e.source && F && F(t)
                 },
                 showSearch: _,
-                OptionList: rl,
+                OptionList: ll,
                 emptyOptions: X,
                 open: M,
                 dropdownClassName: Y,
                 placement: G,
                 onDropdownVisibleChange: function(t) {
                     null != Q && Q(t), null != tt && tt(t)
                 },
                 getRawInputElement: function() {
                     return at
                 }
             })))
         }),
-        bl = (c.SHOW_PARENT = "SHOW_PARENT", c.SHOW_CHILD = "SHOW_CHILD", c),
-        p = bl.SHOW_CHILD,
-        d = bl.SHOW_PARENT,
+        xl = (c.SHOW_PARENT = "SHOW_PARENT", c.SHOW_CHILD = "SHOW_CHILD", c),
+        p = xl.SHOW_CHILD,
+        d = xl.SHOW_PARENT,
         l = Wt.forwardRef(function(t, e) {
             var n, a = t.prefixCls,
                 r = t.size,
                 o = t.disabled,
                 i = t.className,
                 l = t.multiple,
                 c = t.bordered,
@@ -114542,71 +114623,71 @@
                 O = function(t, e) {
                     var n = {};
                     for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
                     if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                         for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
                     return n
                 }(t, ["prefixCls", "size", "disabled", "className", "multiple", "bordered", "transitionName", "choiceTransitionName", "popupClassName", "dropdownClassName", "expandIcon", "placement", "showSearch", "allowClear", "notFoundContent", "direction", "getPopupContainer", "status", "showArrow"]),
-                O = Object(ct.a)(O, ["suffixIcon"]),
+                O = Object(pt.a)(O, ["suffixIcon"]),
                 w = Object(Wt.useContext)(q.b),
                 k = w.getPopupContainer,
                 j = w.getPrefixCls,
                 M = w.renderEmpty,
                 w = w.direction,
                 w = v || w,
                 E = "rtl" === w,
-                C = Object(Wt.useContext)(ve.b),
+                C = Object(Wt.useContext)(Oe.b),
                 S = C.status,
                 L = C.hasFeedback,
                 P = C.isFormItemInput,
                 C = C.feedbackIcon,
-                S = Object(_e.a)(S, x),
-                x = b || (M || be.a)("Cascader"),
+                S = Object(je.a)(S, x),
+                x = b || (M || _e.a)("Cascader"),
                 b = j(),
                 M = j("select", a),
                 D = j("cascader", a),
-                j = Object(Ga.c)(M, v),
+                j = Object($a.c)(M, v),
                 T = j.compactSize,
                 j = j.compactItemClassnames,
                 d = Kt()(d || p, "".concat(D, "-dropdown"), Object(Vt.a)({}, "".concat(D, "-dropdown-rtl"), "rtl" === w)),
                 p = Wt.useMemo(function() {
                     var t;
                     return m && (t = {
-                        render: ll
+                        render: ul
                     }, "object" === Object(qt.a)(m) ? Object(Et.a)(Object(Et.a)({}, t), m) : t)
                 }, [m]),
-                z = Wt.useContext(fi.b),
+                z = Wt.useContext(gi.b),
                 T = T || r || z,
-                r = Wt.useContext(pi.b),
+                r = Wt.useContext(mi.b),
                 z = null != o ? o : r,
                 o = f,
-                r = (f || (o = E ? Wt.createElement(We.a, null) : Wt.createElement(Ve.a, null)), Wt.createElement("span", {
+                r = (f || (o = E ? Wt.createElement(Ue.a, null) : Wt.createElement(Ge.a, null)), Wt.createElement("span", {
                     className: "".concat(M, "-menu-item-loading-icon")
-                }, Wt.createElement(oo.a, {
+                }, Wt.createElement(co.a, {
                     spin: !0
                 }))),
                 f = Wt.useMemo(function() {
                     return !!l && Wt.createElement("span", {
                         className: "".concat(D, "-checkbox-inner")
                     })
                 }, [l]),
                 A = void 0 !== _ ? _ : t.loading || !l,
-                t = Object(hi.a)(Object(Et.a)(Object(Et.a)({}, t), {
+                t = Object(bi.a)(Object(Et.a)(Object(Et.a)({}, t), {
                     hasFeedback: L,
                     feedbackIcon: C,
                     showArrow: A,
                     multiple: l,
                     prefixCls: M
                 })),
                 C = t.suffixIcon,
                 A = t.removeIcon,
                 t = t.clearIcon;
-            return Wt.createElement(bl, Object(Et.a)({
+            return Wt.createElement(xl, Object(Et.a)({
                 prefixCls: M,
-                className: Kt()(!a && D, (n = {}, Object(Vt.a)(n, "".concat(M, "-lg"), "large" === T), Object(Vt.a)(n, "".concat(M, "-sm"), "small" === T), Object(Vt.a)(n, "".concat(M, "-rtl"), E), Object(Vt.a)(n, "".concat(M, "-borderless"), !c), Object(Vt.a)(n, "".concat(M, "-in-form-item"), P), n), Object(_e.b)(M, S, L), j, i),
+                className: Kt()(!a && D, (n = {}, Object(Vt.a)(n, "".concat(M, "-lg"), "large" === T), Object(Vt.a)(n, "".concat(M, "-sm"), "small" === T), Object(Vt.a)(n, "".concat(M, "-rtl"), E), Object(Vt.a)(n, "".concat(M, "-borderless"), !c), Object(Vt.a)(n, "".concat(M, "-in-form-item"), P), n), Object(je.b)(M, S, L), j, i),
                 disabled: z
             }, O, {
                 direction: w,
                 placement: void 0 !== h ? h : "rtl" === v ? "bottomRight" : "bottomLeft",
                 notFoundContent: x,
                 allowClear: g,
                 showSearch: p,
@@ -114614,25 +114695,25 @@
                 inputIcon: C,
                 removeIcon: A,
                 clearIcon: t,
                 loadingIcon: r,
                 checkable: f,
                 dropdownClassName: d,
                 dropdownPrefixCls: a || D,
-                choiceTransitionName: Object(Va.c)(b, "", u),
-                transitionName: Object(Va.c)(b, Object(Va.b)(h), s),
+                choiceTransitionName: Object(Ga.c)(b, "", u),
+                transitionName: Object(Ga.c)(b, Object(Ga.b)(h), s),
                 getPopupContainer: y || k,
                 ref: e,
                 showArrow: L || _
             }))
         }),
-        vl = (l.SHOW_PARENT = d, l.SHOW_CHILD = p, l),
-        c = vl.SHOW_CHILD,
-        d = vl.SHOW_PARENT,
-        yl = new Map([
+        _l = (l.SHOW_PARENT = d, l.SHOW_CHILD = p, l),
+        c = _l.SHOW_CHILD,
+        d = _l.SHOW_PARENT,
+        Ol = new Map([
             ["show-child", c],
             ["show-parent", d]
         ]),
         p = {
             value: n.a.oneOfType([n.a.string, n.a.number]).isRequired,
             label: n.a.string.isRequired,
             disabled: n.a.bool
@@ -114642,15 +114723,15 @@
         d = {
             value: n.a.oneOfType([n.a.string, n.a.number]).isRequired,
             label: n.a.string.isRequired,
             disabled: n.a.bool,
             key: n.a.string,
             parent: n.a.string
         },
-        xl = (cl.propTypes = {
+        wl = (dl.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             locale: n.a.oneOf(["zh-cn", "en-us"]),
             optionsMode: n.a.oneOf(["tree", "flat"]),
             options: n.a.oneOfType([c, n.a.arrayOf(d)]).isRequired,
@@ -114675,31 +114756,31 @@
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func,
             persistence: n.a.oneOfType([n.a.bool, n.a.string, n.a.number]),
             persisted_props: n.a.arrayOf(n.a.oneOf(["value"])),
             persistence_type: n.a.oneOf(["local", "session", "memory"])
-        }, cl.defaultProps = {
+        }, dl.defaultProps = {
             changeOnSelect: !1,
             placement: "bottomLeft",
             multiple: !1,
             expandTrigger: "click",
             allowClear: !0,
             locale: "zh-cn",
             optionsMode: "tree",
             showCheckedStrategy: "show-parent",
             popupContainer: "body",
             bordered: !0,
             disabled: !1,
             persisted_props: ["value"],
             persistence_type: "local"
-        }, cl),
-        _l = e(209),
-        Ol = (sl.propTypes = {
+        }, dl),
+        kl = e(209),
+        jl = (pl.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             direction: n.a.oneOf(["horizontal", "vertical"]),
             options: n.a.arrayOf(n.a.exact({
                 label: n.a.node,
@@ -114717,25 +114798,25 @@
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func,
             persistence: n.a.oneOfType([n.a.bool, n.a.string, n.a.number]),
             persisted_props: n.a.arrayOf(n.a.oneOf(["value"])),
             persistence_type: n.a.oneOf(["local", "session", "memory"])
-        }, sl.defaultProps = {
+        }, pl.defaultProps = {
             direction: "horizontal",
             optionType: "default",
             buttonStyle: "outline",
             disabled: !1,
             size: "middle",
             persisted_props: ["value"],
             persistence_type: "local"
-        }, sl),
-        wl = e(543),
-        kl = (ul.propTypes = {
+        }, pl),
+        Ml = e(543),
+        El = (fl.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             locale: n.a.oneOf(["zh-cn", "en-us"]),
             title: n.a.node,
@@ -114768,26 +114849,26 @@
             popupContainer: n.a.oneOf(["parent", "body"]),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, ul.defaultProps = {
+        }, fl.defaultProps = {
             disabled: !1,
             placement: "top",
             mouseEnterDelay: .1,
             mouseLeaveDelay: .1,
             confirmCounts: 0,
             cancelCounts: 0,
             trigger: "hover",
             locale: "zh-cn",
             popupContainer: "body"
-        }, ul),
-        jl = {
+        }, fl),
+        Cl = {
             icon: {
                 tag: "svg",
                 attrs: {
                     viewBox: "64 64 896 896",
                     focusable: "false"
                 },
                 children: [{
@@ -114796,36 +114877,36 @@
                         d: "M859.9 168H164.1c-4.5 0-8.1 3.6-8.1 8v60c0 4.4 3.6 8 8.1 8h695.8c4.5 0 8.1-3.6 8.1-8v-60c0-4.4-3.6-8-8.1-8zM518.3 355a8 8 0 00-12.6 0l-112 141.7a7.98 7.98 0 006.3 12.9h73.9V848c0 4.4 3.6 8 8 8h60c4.4 0 8-3.6 8-8V509.7H624c6.7 0 10.4-7.7 6.3-12.9L518.3 355z"
                     }
                 }]
             },
             name: "vertical-align-top",
             theme: "outlined"
         },
-        Ml = (dl.displayName = "VerticalAlignTopOutlined", Wt.forwardRef(dl)),
-        El = Wt.memo(function(r) {
-            var t = Object($t.a)(!1, {
+        Sl = (hl.displayName = "VerticalAlignTopOutlined", Wt.forwardRef(hl)),
+        Ll = Wt.memo(function(r) {
+            var t = Object(Zt.a)(!1, {
                     value: r.visible
                 }),
                 t = Object(Gt.a)(t, 2),
                 e = t[0],
                 n = t[1],
                 a = Wt.createRef(),
                 o = Wt.useRef(null),
                 i = function() {
                     return a.current && a.current.ownerDocument ? a.current.ownerDocument : window
                 },
-                l = ut(function(t) {
+                l = ht(function(t) {
                     var e = r.visibilityHeight,
                         e = void 0 === e ? 400 : e,
-                        t = Object(Mt.a)(t.target, !0);
+                        t = Object(Dt.a)(t.target, !0);
                     n(e < t)
                 }),
                 t = (Wt.useEffect(function() {
                     var t = (r.target || i)();
-                    return o.current = Object(it.a)(t, "scroll", function(t) {
+                    return o.current = Object(ut.a)(t, "scroll", function(t) {
                             l(t)
                         }), l({
                             target: t
                         }),
                         function() {
                             o.current && o.current.remove(), l.cancel()
                         }
@@ -114834,59 +114915,59 @@
                 t = t.direction,
                 s = r.prefixCls,
                 u = r.className,
                 u = void 0 === u ? "" : u,
                 s = c("back-top", s),
                 c = c(),
                 t = Kt()(s, Object(Vt.a)({}, "".concat(s, "-rtl"), "rtl" === t), u),
-                u = Object(ct.a)(r, ["prefixCls", "className", "children", "visibilityHeight", "target", "visible"]);
+                u = Object(pt.a)(r, ["prefixCls", "className", "children", "visibilityHeight", "target", "visible"]);
             return Wt.createElement("div", Object(Et.a)({}, u, {
                 className: t,
                 onClick: function(t) {
                     var e = r.onClick,
                         n = r.target,
                         a = r.duration,
                         a = void 0 === a ? 450 : a;
-                    Object(St.a)(0, {
+                    Object(Tt.a)(0, {
                         getContainer: n || i,
                         duration: a
                     }), "function" == typeof e && e(t)
                 },
                 ref: a
-            }), Wt.createElement(pl, {
+            }), Wt.createElement(ml, {
                 prefixCls: s,
                 rootPrefixCls: c,
                 visible: e
             }, r.children))
         }),
-        Cl = (fl.propTypes = {
+        Pl = (gl.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             duration: n.a.number,
             visibilityHeight: n.a.number,
             containerId: n.a.string,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, fl.defaultProps = {
+        }, gl.defaultProps = {
             duration: .45,
             visibilityHeight: 400
-        }, fl),
-        Sl = e(526);
+        }, gl),
+        Dl = e(526);
 
-    function Ll(t) {
+    function Tl(t) {
         return t && "object" === Object(qt.a)(t) ? t : {}
     }
 
-    function Pl(t) {
+    function zl(t) {
         var e, n, a, r = t.prefixCls,
             o = t.loading,
             i = t.className,
             l = t.style,
             c = t.children,
             s = void 0 !== (s = t.avatar) && s,
             u = void 0 === (u = t.title) || u,
@@ -114900,83 +114981,83 @@
             prefixCls: "".concat(h, "-avatar")
         }, r && !o ? {
             size: "large",
             shape: "square"
         } : {
             size: "large",
             shape: "circle"
-        }), Ll(s)), e = Wt.createElement("div", {
+        }), Tl(s)), e = Wt.createElement("div", {
             className: "".concat(h, "-header")
-        }, Wt.createElement(hl, Object(Et.a)({}, c)))), (r || o) && (r && (s = Object(Et.a)(Object(Et.a)({
+        }, Wt.createElement(bl, Object(Et.a)({}, c)))), (r || o) && (r && (s = Object(Et.a)(Object(Et.a)({
             prefixCls: "".concat(h, "-title")
         }, !t && o ? {
             width: "38%"
         } : t && o ? {
             width: "50%"
-        } : {}), Ll(u)), n = Wt.createElement(gl, Object(Et.a)({}, s))), o && (o = Object(Et.a)(Object(Et.a)({
+        } : {}), Tl(u)), n = Wt.createElement(yl, Object(Et.a)({}, s))), o && (o = Object(Et.a)(Object(Et.a)({
             prefixCls: "".concat(h, "-paragraph")
-        }, (c = r, u = {}, (s = t) && c || (u.width = "61%"), u.rows = !s && c ? 3 : 2, u)), Ll(d)), a = Wt.createElement(ml, Object(Et.a)({}, o))), n = Wt.createElement("div", {
+        }, (c = r, u = {}, (s = t) && c || (u.width = "61%"), u.rows = !s && c ? 3 : 2, u)), Tl(d)), a = Wt.createElement(vl, Object(Et.a)({}, o))), n = Wt.createElement("div", {
             className: "".concat(h, "-content")
         }, n, a)), s = Kt()(h, (r = {}, Object(Vt.a)(r, "".concat(h, "-with-avatar"), t), Object(Vt.a)(r, "".concat(h, "-active"), p), Object(Vt.a)(r, "".concat(h, "-rtl"), "rtl" === m), Object(Vt.a)(r, "".concat(h, "-round"), f), r), i), Wt.createElement("div", {
             className: s,
             style: l
         }, e, n))
     }
-    Pl.Button = function(t) {
+    zl.Button = function(t) {
         var e, n = t.prefixCls,
             a = t.className,
             r = t.active,
             o = t.block,
             o = void 0 !== o && o,
             i = t.size,
             i = void 0 === i ? "default" : i,
             n = (0, Wt.useContext(q.b).getPrefixCls)("skeleton", n),
-            t = Object(ct.a)(t, ["prefixCls"]),
+            t = Object(pt.a)(t, ["prefixCls"]),
             r = Kt()(n, "".concat(n, "-element"), (e = {}, Object(Vt.a)(e, "".concat(n, "-active"), r), Object(Vt.a)(e, "".concat(n, "-block"), o), e), a);
         return Wt.createElement("div", {
             className: r
-        }, Wt.createElement(hl, Object(Et.a)({
+        }, Wt.createElement(bl, Object(Et.a)({
             prefixCls: "".concat(n, "-button"),
             size: i
         }, t)))
-    }, Pl.Avatar = function(t) {
+    }, zl.Avatar = function(t) {
         var e = t.prefixCls,
             n = t.className,
             a = t.active,
             r = t.shape,
             r = void 0 === r ? "circle" : r,
             o = t.size,
             o = void 0 === o ? "default" : o,
             e = (0, Wt.useContext(q.b).getPrefixCls)("skeleton", e),
-            t = Object(ct.a)(t, ["prefixCls", "className"]),
+            t = Object(pt.a)(t, ["prefixCls", "className"]),
             a = Kt()(e, "".concat(e, "-element"), Object(Vt.a)({}, "".concat(e, "-active"), a), n);
         return Wt.createElement("div", {
             className: a
-        }, Wt.createElement(hl, Object(Et.a)({
+        }, Wt.createElement(bl, Object(Et.a)({
             prefixCls: "".concat(e, "-avatar"),
             shape: r,
             size: o
         }, t)))
-    }, Pl.Input = function(t) {
+    }, zl.Input = function(t) {
         var e, n = t.prefixCls,
             a = t.className,
             r = t.active,
             o = t.block,
             i = t.size,
             i = void 0 === i ? "default" : i,
             n = (0, Wt.useContext(q.b).getPrefixCls)("skeleton", n),
-            t = Object(ct.a)(t, ["prefixCls"]),
+            t = Object(pt.a)(t, ["prefixCls"]),
             r = Kt()(n, "".concat(n, "-element"), (e = {}, Object(Vt.a)(e, "".concat(n, "-active"), r), Object(Vt.a)(e, "".concat(n, "-block"), o), e), a);
         return Wt.createElement("div", {
             className: r
-        }, Wt.createElement(hl, Object(Et.a)({
+        }, Wt.createElement(bl, Object(Et.a)({
             prefixCls: "".concat(n, "-input"),
             size: i
         }, t)))
-    }, Pl.Image = function(t) {
+    }, zl.Image = function(t) {
         var e = t.prefixCls,
             n = t.className,
             a = t.style,
             t = t.active,
             e = (0, Wt.useContext(q.b).getPrefixCls)("skeleton", e),
             t = Kt()(e, "".concat(e, "-element"), Object(Vt.a)({}, "".concat(e, "-active"), t), n);
         return Wt.createElement("div", {
@@ -114988,39 +115069,39 @@
             viewBox: "0 0 1098 1024",
             xmlns: "http://www.w3.org/2000/svg",
             className: "".concat(e, "-image-svg")
         }, Wt.createElement("path", {
             d: "M365.714286 329.142857q0 45.714286-32.036571 77.677714t-77.677714 32.036571-77.677714-32.036571-32.036571-77.677714 32.036571-77.677714 77.677714-32.036571 77.677714 32.036571 32.036571 77.677714zM950.857143 548.571429l0 256-804.571429 0 0-109.714286 182.857143-182.857143 91.428571 91.428571 292.571429-292.571429zM1005.714286 146.285714l-914.285714 0q-7.460571 0-12.873143 5.412571t-5.412571 12.873143l0 694.857143q0 7.460571 5.412571 12.873143t12.873143 5.412571l914.285714 0q7.460571 0 12.873143-5.412571t5.412571-12.873143l0-694.857143q0-7.460571-5.412571-12.873143t-12.873143-5.412571zM1097.142857 164.571429l0 694.857143q0 37.741714-26.843429 64.585143t-64.585143 26.843429l-914.285714 0q-37.741714 0-64.585143-26.843429t-26.843429-64.585143l0-694.857143q0-37.741714 26.843429-64.585143t64.585143-26.843429l914.285714 0q37.741714 0 64.585143 26.843429t26.843429 64.585143z",
             className: "".concat(e, "-image-path")
         }))))
-    }, Pl.Node = function(t) {
+    }, zl.Node = function(t) {
         var e = t.prefixCls,
             n = t.className,
             a = t.style,
             r = t.active,
             t = t.children,
             e = (0, Wt.useContext(q.b).getPrefixCls)("skeleton", e),
             r = Kt()(e, "".concat(e, "-element"), Object(Vt.a)({}, "".concat(e, "-active"), r), n),
-            t = null != t ? t : Wt.createElement(Sl.a, null);
+            t = null != t ? t : Wt.createElement(Dl.a, null);
         return Wt.createElement("div", {
             className: r
         }, Wt.createElement("div", {
             className: Kt()("".concat(e, "-image"), n),
             style: a
         }, t))
     };
-    var Dl = Pl;
+    var Al = zl;
 
-    function Tl(t, e) {
+    function Rl(t, e) {
         (null == e || e > t.length) && (e = t.length);
         for (var n = 0, a = new Array(e); n < e; n++) a[n] = t[n];
         return a
     }
 
-    function zl(t) {
+    function Il(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.children,
             i = t.loading,
             l = t.active,
@@ -115057,65 +115138,65 @@
                             if (s) throw r
                         }
                     }
                     return l
                 }
             }(t, i) || function(t, e) {
                 var n;
-                if (t) return "string" == typeof t ? Tl(t, e) : "Map" === (n = "Object" === (n = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : n) || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? Tl(t, e) : void 0
+                if (t) return "string" == typeof t ? Rl(t, e) : "Map" === (n = "Object" === (n = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : n) || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? Rl(t, e) : void 0
             }(t, i) || function() {
                 throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
             }())[0],
             v = t[1],
             y = Object(Wt.useRef)();
         return Object(Wt.useEffect)(function() {
             g && (y.current && clearTimeout(y.current), g.is_loading && !b ? "default" === p ? (m && console.log(g.component_name + "." + g.prop_name), v(!0)) : "exclude" === p ? -1 === f.indexOf(g.component_name + "." + g.prop_name) && (m && console.log(g.component_name + "." + g.prop_name), v(!0)) : "include" === p && -1 !== h.indexOf(g.component_name + "." + g.prop_name) && (m && console.log(g.component_name + "." + g.prop_name), v(!0)) : !g.is_loading && b && (y.current = setTimeout(function() {
                 return v(!1)
             })))
-        }, [g]), H.a.createElement(Dl, {
+        }, [g]), H.a.createElement(Al, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             loading: b,
             active: l,
             avatar: c,
             paragraph: s,
             round: u,
             title: d,
             "data-dash-is-loading": g && g.is_loading || void 0
         }, o)
     }
 
-    function Al(t) {
+    function Nl(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.children,
             i = t.offsetBottom,
             l = t.offsetTop,
             c = t.target,
             t = (t.setProps, t.loading_state),
             o = j(o);
-        return H.a.createElement(jt, {
+        return H.a.createElement(Pt, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             offsetBottom: i,
             offsetTop: l,
             target: function() {
                 return c ? document.getElementById(c) : window
             },
             "data-dash-is-loading": t && t.is_loading || void 0
         }, o)
     }
 
-    function Rl(t) {
+    function Yl(t) {
         var e = t.prefixCls,
             n = void 0 === (n = t.separator) ? "/" : n,
             a = t.children,
             r = t.menu,
             o = t.overlay,
             i = t.dropdownProps,
             t = function(t, e) {
@@ -115127,33 +115208,33 @@
             }(t, ["prefixCls", "separator", "children", "menu", "overlay", "dropdownProps"]),
             e = (0, Wt.useContext(q.b).getPrefixCls)("breadcrumb", e),
             l = t = "href" in t ? Wt.createElement("a", Object(Et.a)({
                 className: "".concat(e, "-link")
             }, t), a) : Wt.createElement("span", Object(Et.a)({
                 className: "".concat(e, "-link")
             }, t), a);
-        return t = r || o ? Wt.createElement(Bl.a, Object(Et.a)({
+        return t = r || o ? Wt.createElement(Wl.a, Object(Et.a)({
             menu: r,
             overlay: o,
             placement: "bottom"
         }, i), Wt.createElement("span", {
             className: "".concat(e, "-overlay-link")
-        }, l, Wt.createElement(Oe.a, null))) : l, null != a ? Wt.createElement("li", null, t, n && Wt.createElement("span", {
+        }, l, Wt.createElement(Me.a, null))) : l, null != a ? Wt.createElement("li", null, t, n && Wt.createElement("span", {
             className: "".concat(e, "-separator")
         }, n)) : null
     }
 
-    function Il(t) {
+    function Bl(t) {
         var t = t.children,
             e = (0, Wt.useContext(q.b).getPrefixCls)("breadcrumb");
         return Wt.createElement("span", {
             className: "".concat(e, "-separator")
         }, t || "/")
     }
-    zl._dashprivate_isLoadingComponent = !0, zl.propTypes = {
+    Il._dashprivate_isLoadingComponent = !0, Il.propTypes = {
         id: n.a.string,
         children: n.a.node,
         className: n.a.oneOfType([n.a.string, n.a.object]),
         style: n.a.object,
         key: n.a.string,
         loading: n.a.bool,
         active: n.a.bool,
@@ -115176,127 +115257,127 @@
         includeProps: n.a.arrayOf(n.a.string),
         loading_state: n.a.shape({
             is_loading: n.a.bool,
             prop_name: n.a.string,
             component_name: n.a.string
         }),
         setProps: n.a.func
-    }, zl.defaultProps = {
+    }, Il.defaultProps = {
         loading: !1,
         active: !1,
         avatar: !1,
         paragraph: !0,
         title: !0,
         round: !1,
         debug: !1,
         listenPropsMode: "default",
         excludeProps: [],
         includeProps: []
     };
-    var Nl = zl,
-        Yl = (Al.propTypes = {
+    var Fl = Il,
+        Hl = (Nl.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             offsetBottom: n.a.number,
             offsetTop: n.a.number,
             target: n.a.string,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, Al.defaultProps = {
+        }, Nl.defaultProps = {
             offsetTop: 0
-        }, Al),
-        Bl = e(275),
-        Fl = (Rl.__ANT_BREADCRUMB_ITEM = !0, Rl),
-        p = (Il.__ANT_BREADCRUMB_SEPARATOR = !0, Il);
+        }, Nl),
+        Wl = e(275),
+        Vl = (Yl.__ANT_BREADCRUMB_ITEM = !0, Yl),
+        p = (Bl.__ANT_BREADCRUMB_SEPARATOR = !0, Bl);
 
-    function Hl(t, e, n, a) {
+    function Kl(t, e, n, a) {
         var r, n = n.indexOf(t) === n.length - 1,
             e = (r = e, (e = t).breadcrumbName ? (t = Object.keys(r).join("|"), e.breadcrumbName.replace(new RegExp(":(".concat(t, ")"), "g"), function(t, e) {
                 return r[e] || t
             })) : null);
         return n ? Wt.createElement("span", null, e) : Wt.createElement("a", {
             href: "#/".concat(a.join("/"))
         }, e)
     }
 
-    function Wl(t) {
+    function Ul(t) {
         var r, e, n = t.prefixCls,
             o = void 0 === (a = t.separator) ? "/" : a,
             a = t.style,
             i = t.className,
             l = t.routes,
             c = t.children,
-            s = void 0 === (d = t.itemRender) ? Hl : d,
+            s = void 0 === (d = t.itemRender) ? Kl : d,
             u = void 0 === (d = t.params) ? {} : d,
             d = function(t, e) {
                 var n = {};
                 for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
                 if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                     for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
                 return n
             }(t, ["prefixCls", "separator", "style", "className", "routes", "children", "itemRender", "params"]),
             p = (t = Wt.useContext(q.b)).getPrefixCls,
             t = t.direction,
             p = p("breadcrumb", n),
             n = (l && 0 < l.length ? (r = [], e = l.map(function(t) {
-                var e, n = Xl(t.path, u),
-                    a = (n && r.push(n), t.children && t.children.length && (e = Wt.createElement(Nn.a, {
+                var e, n = ql(t.path, u),
+                    a = (n && r.push(n), t.children && t.children.length && (e = Wt.createElement(Fn.a, {
                         items: t.children.map(function(t) {
                             return {
                                 key: t.path || t.breadcrumbName,
                                 label: s(t, u, l, function(t, e, n) {
-                                    t = Object(Ut.a)(t), e = Xl(e || "", n);
+                                    t = Object(Ut.a)(t), e = ql(e || "", n);
                                     return e && t.push(e), t
                                 }(r, t.path, u))
                             }
                         })
                     })), {
                         separator: o
                     });
-                return e && (a.overlay = e), Wt.createElement(Fl, Object(Et.a)({}, a, {
+                return e && (a.overlay = e), Wt.createElement(Vl, Object(Et.a)({}, a, {
                     key: n || t.breadcrumbName
                 }), s(t, u, l, r))
-            })) : c && (e = Object(Dn.a)(c).map(function(t, e) {
-                return t && Object(je.a)(t, {
+            })) : c && (e = Object(An.a)(c).map(function(t, e) {
+                return t && Object(Ce.a)(t, {
                     separator: o,
                     key: e
                 })
             })), Kt()(p, Object(Vt.a)({}, "".concat(p, "-rtl"), "rtl" === t), i));
         return Wt.createElement("nav", Object(Et.a)({
             className: n,
             style: a
         }, d), Wt.createElement("ol", null, e))
     }
 
-    function Vl(t) {
+    function Gl(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.separator,
             i = t.items,
             t = (t.setProps, t.loading_state);
-        return H.a.createElement($l, {
+        return H.a.createElement(Xl, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             separator: o,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, i.map(function(t) {
-            return H.a.createElement($l.Item, {
-                overlay: t.menuItems ? H.a.createElement(Nn.a, null, t.menuItems.map(function(t) {
-                    return H.a.createElement(Nn.a.Item, {
+            return H.a.createElement(Xl.Item, {
+                overlay: t.menuItems ? H.a.createElement(Fn.a, null, t.menuItems.map(function(t) {
+                    return H.a.createElement(Fn.a.Item, {
                         icon: H.a.createElement(I.a, {
                             icon: t.icon,
                             style: {
                                 marginRight: 3
                             }
                         }),
                         disabled: t.disabled
@@ -115312,16 +115393,93 @@
                 }
             }), H.a.createElement("a", {
                 href: t.href,
                 target: t.target
             }, t.title))
         }))
     }
+    var ql = function(e, n) {
+            return e = (e || "").replace(/^\//, ""), Object.keys(n).forEach(function(t) {
+                e = e.replace(":".concat(t), n[t])
+            }), e
+        },
+        Xl = (Ul.Item = Vl, Ul.Separator = p, Ul),
+        $l = (Gl.propTypes = {
+            id: n.a.string,
+            className: n.a.oneOfType([n.a.string, n.a.object]),
+            style: n.a.object,
+            key: n.a.string,
+            items: n.a.arrayOf(n.a.exact({
+                title: n.a.string,
+                href: n.a.string,
+                target: n.a.string,
+                icon: n.a.string,
+                menuItems: n.a.arrayOf(n.a.exact({
+                    title: n.a.string,
+                    href: n.a.string,
+                    target: n.a.string,
+                    disabled: n.a.bool,
+                    icon: n.a.string
+                }))
+            })),
+            separator: n.a.node,
+            loading_state: n.a.shape({
+                is_loading: n.a.bool,
+                prop_name: n.a.string,
+                component_name: n.a.string
+            }),
+            setProps: n.a.func
+        }, Gl.defaultProps = {
+            separator: "/"
+        }, Gl);
+
+    function Zl(t) {
+        return (Zl = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
+            return typeof t
+        } : function(t) {
+            return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
+        })(t)
+    }
 
-    function Kl(t) {
+    function Jl(e, t) {
+        var n, a = Object.keys(e);
+        return Object.getOwnPropertySymbols && (n = Object.getOwnPropertySymbols(e), t && (n = n.filter(function(t) {
+            return Object.getOwnPropertyDescriptor(e, t).enumerable
+        })), a.push.apply(a, n)), a
+    }
+
+    function Ql(a) {
+        for (var t = 1; t < arguments.length; t++) {
+            var r = null != arguments[t] ? arguments[t] : {};
+            t % 2 ? Jl(Object(r), !0).forEach(function(t) {
+                var e, n;
+                e = a, t = r[n = t], (n = function() {
+                    var t = function(t) {
+                        if ("object" !== Zl(t) || null === t) return t;
+                        var e = t[Symbol.toPrimitive];
+                        if (void 0 === e) return String(t);
+                        e = e.call(t, "string");
+                        if ("object" !== Zl(e)) return e;
+                        throw new TypeError("@@toPrimitive must return a primitive value.")
+                    }(n);
+                    return "symbol" === Zl(t) ? t : String(t)
+                }()) in e ? Object.defineProperty(e, n, {
+                    value: t,
+                    enumerable: !0,
+                    configurable: !0,
+                    writable: !0
+                }) : e[n] = t
+            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(r)) : Jl(Object(r)).forEach(function(t) {
+                Object.defineProperty(a, t, Object.getOwnPropertyDescriptor(r, t))
+            })
+        }
+        return a
+    }
+
+    function tc(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.title,
             i = t.buttonMode,
             l = t.arrow,
@@ -115332,67 +115490,80 @@
             p = t.trigger,
             f = t.autoAdjustOverflow,
             h = t.visible,
             m = t.menuItems,
             g = t.nClicks,
             b = t.popupContainer,
             v = t.buttonProps,
-            y = t.setProps,
+            y = t.freePosition,
+            x = t.freePositionStyle,
+            _ = t.freePositionClassName,
+            O = t.setProps,
             t = t.loading_state,
-            x = Object(Wt.useContext)(G.a);
-        return H.a.createElement(ke.a, {
+            w = Object(Wt.useContext)(G.a);
+        return H.a.createElement(R.a, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
-            overlay: H.a.createElement(Nn.a, {
+            overlay: H.a.createElement(Fn.a, {
                 onClick: function(t, e, n, a) {
-                    return y({
+                    return O(Ql({
                         clickedKey: t.key,
                         nClicks: g + 1
-                    })
+                    }, y ? {
+                        visible: !1
+                    } : {}))
                 }
             }, m.map(function(t) {
-                return t.isDivider ? H.a.createElement(Nn.a.Divider, null) : H.a.createElement(Nn.a.Item, {
+                return t.isDivider ? H.a.createElement(Fn.a.Divider, null) : H.a.createElement(Fn.a.Item, {
                     icon: H.a.createElement(I.a, {
                         icon: t.icon
                     }),
                     disabled: t.disabled,
                     key: t.key || t.title
                 }, H.a.createElement("a", {
                     href: t.href,
                     target: t.target
                 }, t.title))
             })),
             arrow: l,
-            disabled: x && !Object(V.isUndefined)(x.componentDisabled) ? x.componentDisabled : c,
+            disabled: w && !Object(V.isUndefined)(w.componentDisabled) ? w.componentDisabled : c,
             overlayClassName: Object(V.isString)(s) ? s : s ? Object(U.a)(s) : void 0,
             overlayStyle: u,
             placement: d,
             trigger: [p],
             autoAdjustOverflow: f,
-            visible: h,
-            onVisibleChange: function(t) {
-                return y({
+            open: h,
+            onOpenChange: function(t) {
+                return O({
                     visible: t
                 })
             },
             getPopupContainer: "parent" === b ? function(t) {
                 return t.parentNode
             } : void 0,
             "data-dash-is-loading": t && t.is_loading || void 0
-        }, i ? H.a.createElement(z.a, v, o, " ", H.a.createElement(Oe.a, null)) : H.a.createElement("a", {
+        }, y ? H.a.createElement("div", {
+            style: Ql({
+                width: 1,
+                height: 1,
+                position: "fixed",
+                background: "transparent"
+            }, x),
+            className: _
+        }) : i ? H.a.createElement(z.a, v, o, " ", H.a.createElement(Me.a, null)) : H.a.createElement("a", {
             className: "ant-dropdown-link",
             onClick: function(t) {
                 return t.preventDefault()
             }
-        }, o, " ", H.a.createElement(Oe.a, null)))
+        }, o, " ", H.a.createElement(Me.a, null)))
     }
 
-    function Ul(t) {
+    function ec(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.size,
             i = t.addonBefore,
             l = t.addonAfter,
@@ -115428,15 +115599,15 @@
                 j({
                     debounceValue: t
                 })
             }, {
                 debounceWait: Math.max(k, 200),
                 manual: !0
             }).run);
-        return H.a.createElement(Ql.a, {
+        return H.a.createElement(oc.a, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             size: S && !Object(V.isUndefined)(S.componentSize) ? S.componentSize : o,
             addonBefore: i,
             addonAfter: l,
@@ -115468,104 +115639,75 @@
             persistence: M,
             persisted_props: E,
             persistence_type: C,
             "data-dash-is-loading": t && t.is_loading || void 0
         })
     }
 
-    function Gl(t, e) {
-        return Wt.createElement(to.a, Object(Ct.a)(Object(Ct.a)({}, t), {}, {
+    function nc(t, e) {
+        return Wt.createElement(ao.a, Object(Ct.a)(Object(Ct.a)({}, t), {}, {
             ref: e,
-            icon: ec
+            icon: lc
         }))
     }
-    var ql, Xl = function(e, n) {
-            return e = (e || "").replace(/^\//, ""), Object.keys(n).forEach(function(t) {
-                e = e.replace(":".concat(t), n[t])
-            }), e
-        },
-        $l = (Wl.Item = Fl, Wl.Separator = p, Wl),
-        Zl = (Vl.propTypes = {
-            id: n.a.string,
-            className: n.a.oneOfType([n.a.string, n.a.object]),
-            style: n.a.object,
-            key: n.a.string,
-            items: n.a.arrayOf(n.a.exact({
-                title: n.a.string,
-                href: n.a.string,
-                target: n.a.string,
-                icon: n.a.string,
-                menuItems: n.a.arrayOf(n.a.exact({
-                    title: n.a.string,
-                    href: n.a.string,
-                    target: n.a.string,
-                    disabled: n.a.bool,
-                    icon: n.a.string
-                }))
-            })),
-            separator: n.a.node,
-            loading_state: n.a.shape({
-                is_loading: n.a.bool,
-                prop_name: n.a.string,
-                component_name: n.a.string
-            }),
-            setProps: n.a.func
-        }, Vl.defaultProps = {
-            separator: "/"
-        }, Vl),
-        Jl = (Kl.propTypes = {
-            id: n.a.string,
-            className: n.a.oneOfType([n.a.string, n.a.object]),
-            style: n.a.object,
-            key: n.a.string,
+    tc.propTypes = {
+        id: n.a.string,
+        className: n.a.oneOfType([n.a.string, n.a.object]),
+        style: n.a.object,
+        key: n.a.string,
+        title: n.a.string,
+        buttonMode: n.a.bool,
+        buttonProps: n.a.exact({
+            size: n.a.oneOf(["default", "small", "large"]),
+            type: n.a.oneOf(["primary", "ghost", "dashed", "link", "text", "default"]),
+            danger: n.a.bool
+        }),
+        freePosition: n.a.bool,
+        freePositionStyle: n.a.object,
+        freePositionClassName: n.a.string,
+        clickedKey: n.a.string,
+        nClicks: n.a.number,
+        menuItems: n.a.arrayOf(n.a.exact({
             title: n.a.string,
-            buttonMode: n.a.bool,
-            buttonProps: n.a.exact({
-                size: n.a.oneOf(["default", "small", "large"]),
-                type: n.a.oneOf(["primary", "ghost", "dashed", "link", "text", "default"]),
-                danger: n.a.bool
-            }),
-            clickedKey: n.a.string,
-            nClicks: n.a.number,
-            menuItems: n.a.arrayOf(n.a.exact({
-                title: n.a.string,
-                href: n.a.string,
-                target: n.a.string,
-                disabled: n.a.bool,
-                icon: n.a.string,
-                key: n.a.string,
-                isDivider: n.a.bool
-            })),
-            arrow: n.a.bool,
+            href: n.a.string,
+            target: n.a.string,
             disabled: n.a.bool,
-            overlayClassName: n.a.oneOfType([n.a.string, n.a.object]),
-            overlayStyle: n.a.object,
-            placement: n.a.oneOf(["bottomLeft", "bottomCenter", "bottomRight", "topLeft", "topCenter", "topRight"]),
-            trigger: n.a.oneOf(["click", "hover"]),
-            autoAdjustOverflow: n.a.bool,
-            visible: n.a.bool,
-            popupContainer: n.a.oneOf(["parent", "body"]),
-            loading_state: n.a.shape({
-                is_loading: n.a.bool,
-                prop_name: n.a.string,
-                component_name: n.a.string
-            }),
-            setProps: n.a.func
-        }, Kl.defaultProps = {
-            arrow: !1,
-            disabled: !1,
-            visible: !1,
-            buttonMode: !1,
-            trigger: "hover",
-            nClicks: 0,
-            popupContainer: "body",
-            autoAdjustOverflow: !0
-        }, Kl),
-        Ql = e(708),
-        tc = (Ul.propTypes = {
+            icon: n.a.string,
+            key: n.a.string,
+            isDivider: n.a.bool
+        })),
+        arrow: n.a.bool,
+        disabled: n.a.bool,
+        overlayClassName: n.a.oneOfType([n.a.string, n.a.object]),
+        overlayStyle: n.a.object,
+        placement: n.a.oneOf(["bottomLeft", "bottomCenter", "bottomRight", "topLeft", "topCenter", "topRight"]),
+        trigger: n.a.oneOf(["click", "hover"]),
+        autoAdjustOverflow: n.a.bool,
+        visible: n.a.bool,
+        popupContainer: n.a.oneOf(["parent", "body"]),
+        loading_state: n.a.shape({
+            is_loading: n.a.bool,
+            prop_name: n.a.string,
+            component_name: n.a.string
+        }),
+        setProps: n.a.func
+    }, tc.defaultProps = {
+        arrow: !1,
+        disabled: !1,
+        visible: !1,
+        buttonMode: !1,
+        trigger: "hover",
+        nClicks: 0,
+        popupContainer: "body",
+        autoAdjustOverflow: !0,
+        freePosition: !1
+    };
+    var ac, rc = tc,
+        oc = e(708),
+        ic = (ec.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             addonBefore: n.a.node,
             addonAfter: n.a.node,
             prefix: n.a.node,
@@ -115592,27 +115734,27 @@
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func,
             persistence: n.a.oneOfType([n.a.bool, n.a.string, n.a.number]),
             persisted_props: n.a.arrayOf(n.a.oneOf(["value"])),
             persistence_type: n.a.oneOf(["local", "session", "memory"])
-        }, Ul.defaultProps = {
+        }, ec.defaultProps = {
             controls: !0,
             keyboard: !0,
             stringMode: !1,
             disabled: !1,
             size: "middle",
             bordered: !0,
             nSubmit: 0,
             debounceWait: 200,
             persisted_props: ["value"],
             persistence_type: "local"
-        }, Ul),
-        ec = {
+        }, ec),
+        lc = {
             icon: {
                 tag: "svg",
                 attrs: {
                     viewBox: "64 64 896 896",
                     focusable: "false"
                 },
                 children: [{
@@ -115621,17 +115763,17 @@
                         d: "M908.1 353.1l-253.9-36.9L540.7 86.1c-3.1-6.3-8.2-11.4-14.5-14.5-15.8-7.8-35-1.3-42.9 14.5L369.8 316.2l-253.9 36.9c-7 1-13.4 4.3-18.3 9.3a32.05 32.05 0 00.6 45.3l183.7 179.1-43.4 252.9a31.95 31.95 0 0046.4 33.7L512 754l227.1 119.4c6.2 3.3 13.4 4.4 20.3 3.2 17.4-3 29.1-19.5 26.1-36.9l-43.4-252.9 183.7-179.1c5-4.9 8.3-11.3 9.3-18.3 2.7-17.5-9.5-33.7-27-36.3z"
                     }
                 }]
             },
             name: "star",
             theme: "filled"
         },
-        nc = (Gl.displayName = "StarFilled", Wt.forwardRef(Gl)),
-        ac = e(107),
-        rc = (l = H.a.Component, Object(r.a)(oc, l), ql = Object(o.a)(oc), Object(a.a)(oc, [{
+        cc = (nc.displayName = "StarFilled", Wt.forwardRef(nc)),
+        sc = e(107),
+        uc = (l = H.a.Component, Object(r.a)(dc, l), ac = Object(o.a)(dc), Object(a.a)(dc, [{
             key: "getClassName",
             value: function() {
                 var t = this.props,
                     e = t.prefixCls,
                     n = t.index,
                     a = t.value,
                     r = t.allowHalf,
@@ -115669,47 +115811,47 @@
                     }, H.a.createElement("div", {
                         className: "".concat(o, "-first")
                     }, i), H.a.createElement("div", {
                         className: "".concat(o, "-second")
                     }, i)));
                 return e = l ? l(e, this.props) : e
             }
-        }]), oc);
+        }]), dc);
 
-    function oc() {
+    function dc() {
         var a;
-        Object(i.a)(this, oc);
+        Object(i.a)(this, dc);
         for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
-        return (a = ql.call.apply(ql, [this].concat(e))).onHover = function(t) {
+        return (a = ac.call.apply(ac, [this].concat(e))).onHover = function(t) {
             var e = a.props;
             (0, e.onHover)(t, e.index)
         }, a.onClick = function(t) {
             var e = a.props;
             (0, e.onClick)(t, e.index)
         }, a.onKeyDown = function(t) {
             var e = a.props,
                 n = e.onClick,
                 e = e.index;
             13 === t.keyCode && n(t, e)
         }, a
     }
 
-    function ic() {}
-    c = H.a.Component, Object(r.a)(cc, c), lc = Object(o.a)(cc), Object(a.a)(cc, [{
+    function pc() {}
+    c = H.a.Component, Object(r.a)(hc, c), fc = Object(o.a)(hc), Object(a.a)(hc, [{
         key: "componentDidMount",
         value: function() {
             var t = this.props,
                 e = t.autoFocus,
                 t = t.disabled;
             e && !t && this.focus()
         }
     }, {
         key: "getStarDOM",
         value: function(t) {
-            return Object(ac.a)(this.stars[t])
+            return Object(sc.a)(this.stars[t])
         }
     }, {
         key: "getStarValue",
         value: function(t, e) {
             var n, a, r, o, i = this.props,
                 l = i.allowHalf,
                 i = "rtl" === i.direction,
@@ -115736,15 +115878,15 @@
             "value" in this.props || this.setState({
                 value: t
             }), e(t)
         }
     }, {
         key: "render",
         value: function() {
-            for (var t = this.props, e = t.count, n = t.allowHalf, a = t.style, r = t.prefixCls, o = t.disabled, i = t.className, l = t.character, c = t.characterRender, s = t.tabIndex, t = t.direction, u = this.state, d = u.value, p = u.hoverValue, f = u.focused, h = [], u = o ? "".concat(r, "-disabled") : "", m = 0; m < e; m += 1) h.push(H.a.createElement(rc, {
+            for (var t = this.props, e = t.count, n = t.allowHalf, a = t.style, r = t.prefixCls, o = t.disabled, i = t.className, l = t.character, c = t.characterRender, s = t.tabIndex, t = t.direction, u = this.state, d = u.value, p = u.hoverValue, f = u.focused, h = [], u = o ? "".concat(r, "-disabled") : "", m = 0; m < e; m += 1) h.push(H.a.createElement(uc, {
                 ref: this.saveRef(m),
                 index: m,
                 count: e,
                 disabled: o,
                 prefixCls: "".concat(r, "-star"),
                 allowHalf: n,
                 value: void 0 === p ? d : p,
@@ -115772,18 +115914,18 @@
         key: "getDerivedStateFromProps",
         value: function(t, e) {
             return "value" in t && void 0 !== t.value ? Object(Ct.a)(Object(Ct.a)({}, e), {}, {
                 value: t.value
             }) : e
         }
     }]);
-    var lc, d = cc;
+    var fc, d = hc;
 
-    function cc(t) {
-        Object(i.a)(this, cc), (l = lc.call(this, t)).stars = void 0, l.rate = void 0, l.onHover = function(t, e) {
+    function hc(t) {
+        Object(i.a)(this, hc), (l = fc.call(this, t)).stars = void 0, l.rate = void 0, l.onHover = function(t, e) {
             var n = l.props.onHoverChange,
                 e = l.getStarValue(e, t.pageX);
             e !== l.state.cleanedValue && l.setState({
                 hoverValue: e,
                 cleanedValue: null
             }), n(e)
         }, l.onMouseLeave = function() {
@@ -115836,22 +115978,22 @@
     d.defaultProps = {
         defaultValue: 0,
         count: 5,
         allowHalf: !1,
         allowClear: !0,
         style: {},
         prefixCls: "rc-rate",
-        onChange: ic,
+        onChange: pc,
         character: "★",
-        onHoverChange: ic,
+        onHoverChange: pc,
         tabIndex: 0,
         direction: "ltr"
     };
 
-    function sc(t) {
+    function mc(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.allowClear,
             i = t.allowHalf,
             l = t.count,
@@ -115865,15 +116007,15 @@
             m = t.persisted_props,
             t = t.persistence_type,
             g = Object(Wt.useContext)(G.a);
         return Object(Wt.useEffect)(function() {
             u && !d && p({
                 value: u
             })
-        }, []), H.a.createElement(pc, {
+        }, []), H.a.createElement(vc, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             allowClear: o,
             allowHalf: i,
             count: l,
@@ -115888,63 +116030,63 @@
             persistence: h,
             persisted_props: m,
             persistence_type: t,
             "data-dash-is-loading": f && f.is_loading || void 0
         })
     }
 
-    function uc(t) {
+    function gc(t) {
         var e, n, a = t.value,
             r = t.formatter,
             o = t.precision,
             i = t.decimalSeparator,
             l = void 0 === (l = t.groupSeparator) ? "" : l,
             t = t.prefixCls;
-        return l = "function" == typeof r ? r(a) : (a = (r = String(a)).match(/^(-?)(\d*)(\.(\d+))?$/)) && "-" !== r ? (e = a[1], n = a[2] || "0", a = a[4] || "", n = n.replace(/\B(?=(\d{3})+(?!\d))/g, l), a = (a = "number" == typeof o ? mc()(a, o, "0").slice(0, 0 < o ? o : 0) : a) && "".concat(i).concat(a), [Wt.createElement("span", {
+        return l = "function" == typeof r ? r(a) : (a = (r = String(a)).match(/^(-?)(\d*)(\.(\d+))?$/)) && "-" !== r ? (e = a[1], n = a[2] || "0", a = a[4] || "", n = n.replace(/\B(?=(\d{3})+(?!\d))/g, l), a = (a = "number" == typeof o ? _c()(a, o, "0").slice(0, 0 < o ? o : 0) : a) && "".concat(i).concat(a), [Wt.createElement("span", {
             key: "int",
             className: "".concat(t, "-content-value-int")
         }, e, n), a && Wt.createElement("span", {
             key: "decimal",
             className: "".concat(t, "-content-value-decimal")
         }, a)]) : r, Wt.createElement("span", {
             className: "".concat(t, "-content-value")
         }, l)
     }
-    var dc = d,
-        pc = Wt.forwardRef(function(t, e) {
+    var bc = d,
+        vc = Wt.forwardRef(function(t, e) {
             var n = t.prefixCls,
                 a = t.tooltips,
                 r = t.character,
-                r = void 0 === r ? Wt.createElement(nc, null) : r,
+                r = void 0 === r ? Wt.createElement(cc, null) : r,
                 t = function(t, e) {
                     var n = {};
                     for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
                     if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                         for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
                     return n
                 }(t, ["prefixCls", "tooltips", "character"]),
                 o = Wt.useContext(q.b),
                 i = o.getPrefixCls,
                 o = o.direction,
                 i = i("rate", n);
-            return Wt.createElement(dc, Object(Et.a)({
+            return Wt.createElement(bc, Object(Et.a)({
                 ref: e,
                 character: r,
                 characterRender: function(t, e) {
                     e = e.index;
                     return a ? Wt.createElement(D.a, {
                         title: a[e]
                     }, t) : t
                 }
             }, t, {
                 prefixCls: i,
                 direction: o
             }))
         }),
-        fc = (sc.propTypes = {
+        yc = (mc.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             allowClear: n.a.bool,
             allowHalf: n.a.bool,
             count: n.a.number,
@@ -115957,27 +116099,27 @@
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func,
             persistence: n.a.oneOfType([n.a.bool, n.a.string, n.a.number]),
             persisted_props: n.a.arrayOf(n.a.oneOf(["value"])),
             persistence_type: n.a.oneOf(["local", "session", "memory"])
-        }, sc.defaultProps = {
+        }, mc.defaultProps = {
             allowClear: !0,
             allowHalf: !1,
             count: 5,
             defaultValue: 0,
             disabled: !1,
             persisted_props: ["value"],
             persistence_type: "local"
-        }, sc),
-        hc = e(143),
+        }, mc),
+        xc = e(143),
         p = e(519),
-        mc = e.n(p),
-        gc = Object(q.c)({
+        _c = e.n(p),
+        Oc = Object(q.c)({
             prefixCls: "statistic"
         })(function(t) {
             var e = t.prefixCls,
                 n = t.className,
                 a = t.style,
                 r = t.valueStyle,
                 o = t.value,
@@ -115991,105 +116133,105 @@
                 d = t.direction,
                 p = t.onMouseEnter,
                 f = t.onMouseLeave,
                 h = t.decimalSeparator,
                 h = void 0 === h ? "." : h,
                 m = t.groupSeparator,
                 m = void 0 === m ? "," : m,
-                h = Wt.createElement(uc, Object(Et.a)({
+                h = Wt.createElement(gc, Object(Et.a)({
                     decimalSeparator: h,
                     groupSeparator: m
                 }, t, {
                     value: o
                 })),
                 m = Kt()(e, Object(Vt.a)({}, "".concat(e, "-rtl"), "rtl" === d), n);
             return Wt.createElement("div", {
                 className: m,
                 style: a,
                 onMouseEnter: p,
                 onMouseLeave: f
             }, i && Wt.createElement("div", {
                 className: "".concat(e, "-title")
-            }, i), Wt.createElement(Dl, {
+            }, i), Wt.createElement(Al, {
                 paragraph: !1,
                 loading: u,
                 className: "".concat(e, "-skeleton")
             }, Wt.createElement("div", {
                 style: r,
                 className: "".concat(e, "-content")
             }, c && Wt.createElement("span", {
                 className: "".concat(e, "-content-prefix")
             }, c), l ? l(h) : h, s && Wt.createElement("span", {
                 className: "".concat(e, "-content-suffix")
             }, s))))
         }),
         l = e(270),
-        bc = e.n(l),
-        vc = [
+        wc = e.n(l),
+        kc = [
             ["Y", 31536e6],
             ["M", 2592e6],
             ["D", 864e5],
             ["H", 36e5],
             ["m", 6e4],
             ["s", 1e3],
             ["S", 1]
         ];
 
-    function yc(t) {
+    function jc(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.value,
             i = t.showGroupSeparator,
             l = t.precision,
             c = t.prefix,
             s = t.suffix,
             u = t.title,
             d = t.titleTooltip,
             p = t.valueStyle,
             t = (t.setProps, t.loading_state);
-        return H.a.createElement(Pc, {
+        return H.a.createElement(Ic, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             value: Object(V.isString)(o) || Object(V.isNumber)(o) ? o : void 0,
             formatter: Object(V.isString)(o) || Object(V.isNumber)(o) ? void 0 : function() {
                 return o
             },
             groupSeparator: i ? "," : "",
             precision: l,
             prefix: c,
             suffix: s,
-            title: d ? H.a.createElement(za.b, {
+            title: d ? H.a.createElement(Ia.b, {
                 size: 5
-            }, u, H.a.createElement(po, {
+            }, u, H.a.createElement(mo, {
                 title: d
-            }, H.a.createElement(Dc.a, null))) : u,
+            }, H.a.createElement(Nc.a, null))) : u,
             valueStyle: p,
             "data-dash-is-loading": t && t.is_loading || void 0
         })
     }
 
-    function xc(t) {
+    function Mc(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.value,
             i = t.valueFormat,
             l = t.format,
             c = t.prefix,
             s = t.suffix,
             u = t.title,
             d = t.titleTooltip,
             p = t.valueStyle,
             t = (t.setProps, t.loading_state);
-        return H.a.createElement(zc, {
+        return H.a.createElement(Bc, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             value: C()(o, i),
             format: l,
             prefix: c,
@@ -116100,23 +116242,23 @@
                 title: d
             }, H.a.createElement(QuestionCircleOutlined, null))) : u,
             valueStyle: p,
             "data-dash-is-loading": t && t.is_loading || void 0
         })
     }
 
-    function _c(t) {
+    function Ec(t) {
         var e = t.prefixCls,
             n = t.className,
             a = void 0 === (a = t.color) ? "blue" : a,
             r = t.dot,
             o = void 0 !== (o = t.pending) && o,
             i = (t.position, t.label),
             l = t.children,
-            t = Rc(t, ["prefixCls", "className", "color", "dot", "pending", "position", "label", "children"]),
+            t = Hc(t, ["prefixCls", "className", "color", "dot", "pending", "position", "label", "children"]),
             e = (0, Wt.useContext(q.b).getPrefixCls)("timeline", e),
             o = Kt()((c = {}, Object(Vt.a)(c, "".concat(e, "-item"), !0), Object(Vt.a)(c, "".concat(e, "-item-pending"), o), c), n),
             n = Kt()((c = {}, Object(Vt.a)(c, "".concat(e, "-item-head"), !0), Object(Vt.a)(c, "".concat(e, "-item-head-custom"), !!r), Object(Vt.a)(c, "".concat(e, "-item-head-").concat(a), !0), c)),
             c = /blue|red|green|gray/.test(a || "") ? void 0 : a;
         return Wt.createElement("li", Object(Et.a)({}, t, {
             className: o
         }), i && Wt.createElement("div", {
@@ -116130,15 +116272,15 @@
                 color: c
             }
         }, r), Wt.createElement("div", {
             className: "".concat(e, "-item-content")
         }, l))
     }
 
-    function Oc(t) {
+    function Cc(t) {
         var e = (n = Wt.useContext(q.b)).getPrefixCls,
             n = n.direction,
             a = t.prefixCls,
             r = void 0 === (o = t.pending) ? null : o,
             o = t.pendingDot,
             i = t.children,
             l = t.className,
@@ -116149,70 +116291,70 @@
                 for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
                 if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                     for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
                 return n
             }(t, ["prefixCls", "pending", "pendingDot", "children", "className", "reverse", "mode"]),
             d = e("timeline", a),
             t = "boolean" == typeof r ? null : r,
-            e = r ? Wt.createElement(_c, {
+            e = r ? Wt.createElement(Ec, {
                 pending: !!r,
-                dot: o || Wt.createElement(oo.a, null)
+                dot: o || Wt.createElement(co.a, null)
             }, t) : null,
             o = ((a = Wt.Children.toArray(i)).push(e), c && a.reverse(), a.filter(function(t) {
                 return !!t
             })),
             p = Wt.Children.count(o),
             f = "".concat(d, "-item-last"),
             t = Wt.Children.map(o, function(t, e) {
                 var n = e === p - 2 ? f : "",
                     a = e === p - 1 ? f : "";
-                return Object(je.a)(t, {
+                return Object(Ce.a)(t, {
                     className: Kt()([t.props.className, !c && r ? n : a, (n = t, a = e, "alternate" === s ? "right" === n.props.position ? "".concat(d, "-item-right") : "left" === n.props.position ? "".concat(d, "-item-left") : "".concat(d, a % 2 == 0 ? "-item-left" : "-item-right") : "left" === s ? "".concat(d, "-item-left") : "right" === s || "right" === n.props.position ? "".concat(d, "-item-right") : "")])
                 })
             }),
             i = a.some(function(t) {
                 return !(null == (t = null == t ? void 0 : t.props) || !t.label)
             }),
             o = Kt()(d, (e = {}, Object(Vt.a)(e, "".concat(d, "-pending"), !!r), Object(Vt.a)(e, "".concat(d, "-reverse"), !!c), Object(Vt.a)(e, "".concat(d, "-").concat(s), !!s && !i), Object(Vt.a)(e, "".concat(d, "-label"), i), Object(Vt.a)(e, "".concat(d, "-rtl"), "rtl" === n), e), l);
         return Wt.createElement("ul", Object(Et.a)({}, u, {
             className: o
         }), t)
     }
 
-    function wc(t) {
+    function Sc(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.items,
             i = t.mode,
             l = t.pending,
             c = t.pendingDot,
             s = t.reverse,
             t = (t.setProps, t.loading_state);
-        return H.a.createElement(Ic, {
+        return H.a.createElement(Wc, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             mode: i,
             pending: l,
             pendingDot: c,
             reverse: s,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, o.map(function(t) {
-            return H.a.createElement(Ic.Item, {
+            return H.a.createElement(Wc.Item, {
                 color: t.color,
                 dot: t.icon,
                 label: t.label
             }, t.content)
         }))
     }
 
-    function kc(t) {
+    function Lc(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.type,
             i = t.size,
             l = t.percent,
@@ -116224,15 +116366,15 @@
             f = t.strokeWidth,
             h = t.trailColor,
             m = t.width,
             g = t.gapDegree,
             b = t.gapPosition,
             v = t.steps,
             y = t.loading_state;
-        return t.setProps, H.a.createElement(kn, {
+        return t.setProps, H.a.createElement(En, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             type: o,
             size: i,
             percent: l,
@@ -116252,50 +116394,50 @@
             gapDegree: g,
             gapPosition: b,
             steps: v,
             "data-dash-is-loading": y && y.is_loading || void 0
         })
     }
 
-    function jc(t) {
+    function Pc(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.mode,
             i = t.text,
             l = t.src,
             c = t.srcSet,
             s = t.icon,
             u = t.alt,
             d = t.gap,
             p = t.size,
             f = t.shape,
             h = t.loading_state;
-        return t.setProps, "image" === o ? H.a.createElement(Bc.a, {
+        return t.setProps, "image" === o ? H.a.createElement(Uc.a, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             src: l,
             srcSet: c,
             alt: u,
             size: p,
             shape: f,
             "data-dash-is-loading": h && h.is_loading || void 0
-        }) : "text" === o ? H.a.createElement(Bc.a, {
+        }) : "text" === o ? H.a.createElement(Uc.a, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             gap: d,
             size: p,
             shape: f,
             "data-dash-is-loading": h && h.is_loading || void 0
-        }, i) : H.a.createElement(Bc.a, {
+        }, i) : H.a.createElement(Uc.a, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             icon: s ? H.a.createElement(I.a, {
                 icon: s
             }) : H.a.createElement(I.a, {
@@ -116303,41 +116445,41 @@
             }),
             size: p,
             shape: f,
             "data-dash-is-loading": h && h.is_loading || void 0
         })
     }
 
-    function Mc(t) {
+    function Dc(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.maxCount,
             l = t.maxPopoverPlacement,
             c = t.maxPopoverTrigger,
             s = t.maxStyle,
             u = t.size,
             d = t.loading_state;
-        return t.setProps, H.a.createElement(Bc.a.Group, {
+        return t.setProps, H.a.createElement(Uc.a.Group, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             maxCount: i,
             maxPopoverPlacement: l,
             maxPopoverTrigger: c,
             maxStyle: s,
             size: u,
             "data-dash-is-loading": d && d.is_loading || void 0
         }, n)
     }
 
-    function Ec(t) {
+    function Tc(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.color,
             l = t.count,
@@ -116348,15 +116490,15 @@
             p = t.status,
             f = t.text,
             h = t.title,
             m = t.size,
             g = t.nClicks,
             b = t.loading_state,
             v = t.setProps;
-        return H.a.createElement(Wc.a, {
+        return H.a.createElement(Xc.a, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             color: i,
             count: l,
             dot: c,
@@ -116372,37 +116514,37 @@
                     nClicks: ++g
                 })
             },
             "data-dash-is-loading": b && b.is_loading || void 0
         }, n)
     }
 
-    function Cc(t) {
+    function zc(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.color,
             l = t.placement,
             c = t.text,
             s = t.loading_state;
-        return t.setProps, H.a.createElement(Wc.a.Ribbon, {
+        return t.setProps, H.a.createElement(Xc.a.Ribbon, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             color: i,
             placement: l,
             text: c,
             "data-dash-is-loading": s && s.is_loading || void 0
         }, n)
     }
 
-    function Sc(t) {
+    function Ac(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.locale,
             i = t.setProps,
             l = t.disabled,
@@ -116429,15 +116571,15 @@
             o = M && M.locale || o;
         return Object(Wt.useEffect)(function() {
             f && !p && i({
                 value: f
             })
         }, []), H.a.createElement("div", null, H.a.createElement(W.a, {
             locale: K.b.get(o)
-        }, H.a.createElement(qc, {
+        }, H.a.createElement(ts, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             onChange: function(t, e) {
                 Object(V.isString)(e) && i({
                     value: e
@@ -116465,15 +116607,15 @@
                 return t.parentNode
             } : void 0,
             open: !(!Object(V.isUndefined)(O) && O) && void 0,
             inputReadOnly: O
         })))
     }
 
-    function Lc(t) {
+    function Rc(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.locale,
             i = t.setProps,
             l = t.value,
@@ -116500,15 +116642,15 @@
             o = M && M.locale || o;
         return Object(Wt.useEffect)(function() {
             c && !l && i({
                 value: c
             })
         }, []), H.a.createElement("div", null, H.a.createElement(W.a, {
             locale: K.b.get(o)
-        }, H.a.createElement($c, {
+        }, H.a.createElement(ns, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             onChange: function(t, e) {
                 Array.isArray(e) ? i({
                     value: [e[0], e[1]]
@@ -116544,54 +116686,54 @@
     }
     var c = Wt.memo(function(t) {
             var e = t.value,
                 n = t.format,
                 i = void 0 === n ? "HH:mm:ss" : n,
                 a = t.onChange,
                 r = t.onFinish,
-                o = Object(hc.a)(),
+                o = Object(xc.a)(),
                 l = Wt.useRef(null);
             return Wt.useEffect(function() {
                 return (t = new Date(e).getTime()) >= Date.now() && (l.current = setInterval(function() {
                         o(), null != a && a(t - Date.now()), t < Date.now() && (null != r && r(), l.current) && (clearInterval(l.current), l.current = null)
                     }, 1e3 / 30)),
                     function() {
                         l.current && (clearInterval(l.current), l.current = null)
                     };
                 var t
-            }, [e]), Wt.createElement(gc, Object(Et.a)({}, t, {
+            }, [e]), Wt.createElement(Oc, Object(Et.a)({}, t, {
                 valueRender: function(t) {
-                    return Object(je.a)(t, {
+                    return Object(Ce.a)(t, {
                         title: void 0
                     })
                 },
                 formatter: function(t, e) {
                     return t = t, e = void 0 === (e = (e = Object(Et.a)(Object(Et.a)({}, e), {
                         format: i
                     })).format) ? "" : e, t = new Date(t).getTime(), o = Date.now(), t = Math.max(t - o, 0), r = t, t = /\[[^\]]*]/g, n = ((o = e).match(t) || []).map(function(t) {
                         return t.slice(1, -1)
-                    }), o = o.replace(t, "[]"), o = vc.reduce(function(t, e) {
+                    }), o = o.replace(t, "[]"), o = kc.reduce(function(t, e) {
                         var n, e = Object(Gt.a)(e, 2),
                             a = e[0],
                             e = e[1];
                         return t.includes(a) ? (n = Math.floor(r / e), r -= n * e, t.replace(new RegExp("".concat(a, "+"), "g"), function(t) {
                             t = t.length;
-                            return bc()(n.toString(), t, "0")
+                            return wc()(n.toString(), t, "0")
                         })) : t
                     }, o), a = 0, o.replace(t, function() {
                         var t = n[a];
                         return a += 1, t
                     });
                     var r, n, a, o
                 }
             }))
         }),
-        Pc = (gc.Countdown = c, gc),
-        Dc = e(310),
-        Tc = (yc.propTypes = {
+        Ic = (Oc.Countdown = c, Oc),
+        Nc = e(310),
+        Yc = (jc.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             value: n.a.oneOfType([n.a.number, n.a.string, n.a.node]),
             showGroupSeparator: n.a.bool,
             precision: n.a.number,
@@ -116602,19 +116744,19 @@
             valueStyle: n.a.object,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, yc.defaultProps = {
+        }, jc.defaultProps = {
             showGroupSeparator: !0
-        }, yc),
-        zc = Pc.Countdown,
-        Ac = (xc.propTypes = {
+        }, jc),
+        Bc = Ic.Countdown,
+        Fc = (Mc.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             format: n.a.string,
             value: n.a.string,
             valueFormat: n.a.string,
@@ -116625,26 +116767,26 @@
             valueStyle: n.a.object,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, xc.defaultProps = {
+        }, Mc.defaultProps = {
             valueFormat: "YYYY-MM-DD hh:mm:ss"
-        }, xc),
-        Rc = function(t, e) {
+        }, Mc),
+        Hc = function(t, e) {
             var n = {};
             for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
             if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                 for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
             return n
         },
-        Ic = (Oc.Item = _c, Oc),
-        Nc = (wc.propTypes = {
+        Wc = (Cc.Item = Ec, Cc),
+        Vc = (Sc.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             items: n.a.arrayOf(n.a.exact({
                 content: n.a.node,
                 color: n.a.string,
@@ -116657,19 +116799,19 @@
             reverse: n.a.bool,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, wc.defaultProps = {
+        }, Sc.defaultProps = {
             mode: "left",
             reverse: !1
-        }, wc),
-        Yc = (kc.propTypes = {
+        }, Sc),
+        Kc = (Lc.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             type: n.a.oneOf(["line", "circle", "dashboard"]),
             size: n.a.oneOf(["default", "small"]),
             percent: n.a.number,
@@ -116693,24 +116835,24 @@
             steps: n.a.number,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, kc.defaultProps = {
+        }, Lc.defaultProps = {
             type: "line",
             size: "default",
             percent: 0,
             showInfo: !0,
             width: 132,
             gapPosition: "bottom"
-        }, kc),
-        Bc = e(220),
-        Fc = (jc.propTypes = {
+        }, Lc),
+        Uc = e(220),
+        Gc = (Pc.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             mode: n.a.oneOf(["text", "icon", "image"]),
             gap: n.a.number,
             text: n.a.string,
@@ -116729,21 +116871,21 @@
             shape: n.a.oneOf(["circle", "square"]),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, jc.defaultProps = {
+        }, Pc.defaultProps = {
             mode: "icon",
             gap: 4,
             size: "default",
             shape: "circle"
-        }, jc),
-        Hc = (Mc.propTypes = {
+        }, Pc),
+        qc = (Dc.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             maxCount: n.a.number,
             maxPopoverPlacement: n.a.oneOf(["top", "bottom"]),
@@ -116759,21 +116901,21 @@
             })]),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, Mc.defaultProps = {
+        }, Dc.defaultProps = {
             maxPopoverPlacement: "top",
             maxPopoverTrigger: "hover",
             size: "default"
-        }, Mc),
-        Wc = e(697),
-        Vc = (Ec.propTypes = {
+        }, Dc),
+        Xc = e(697),
+        $c = (Tc.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             color: n.a.string,
             count: n.a.number,
@@ -116788,45 +116930,45 @@
             nClicks: n.a.number,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, Ec.defaultProps = {
+        }, Tc.defaultProps = {
             nClicks: 0,
             dot: !1,
             showZero: !1,
             overflowCount: 99,
             size: "default"
-        }, Ec),
-        Kc = (Cc.propTypes = {
+        }, Tc),
+        Zc = (zc.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             color: n.a.string,
             placement: n.a.oneOf(["start", "end"]),
             text: n.a.node,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, Cc.defaultProps = {
+        }, zc.defaultProps = {
             placement: "end"
-        }, Cc),
-        Uc = S.a.TimePicker,
-        Gc = S.a.RangePicker,
+        }, zc),
+        Jc = S.a.TimePicker,
+        Qc = S.a.RangePicker,
         d = Wt.forwardRef(function(t, e) {
             var n = t.dropdownClassName,
                 a = t.popupClassName;
-            return Wt.createElement(Gc, Object(Et.a)({}, t, {
+            return Wt.createElement(Qc, Object(Et.a)({}, t, {
                 dropdownClassName: n,
                 popupClassName: a,
                 picker: "time",
                 mode: void 0,
                 ref: e
             }))
         }),
@@ -116841,25 +116983,25 @@
                     if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                         for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
                     return n
                 }(t, ["addon", "renderExtraFooter", "popupClassName", "dropdownClassName"]),
                 i = Wt.useMemo(function() {
                     return a || n || void 0
                 }, [n, a]);
-            return Wt.createElement(Uc, Object(Et.a)({
+            return Wt.createElement(Jc, Object(Et.a)({
                 dropdownClassName: o,
                 popupClassName: r
             }, t, {
                 mode: void 0,
                 ref: e,
                 renderExtraFooter: i
             }))
         }),
-        qc = (p.RangePicker = d, p),
-        Xc = (Sc.propTypes = {
+        ts = (p.RangePicker = d, p),
+        es = (Ac.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             locale: n.a.oneOf(["zh-cn", "en-us"]),
             format: n.a.string,
             disabled: n.a.bool,
@@ -116882,32 +117024,32 @@
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func,
             persistence: n.a.oneOfType([n.a.bool, n.a.string, n.a.number]),
             persisted_props: n.a.arrayOf(n.a.oneOf(["value"])),
             persistence_type: n.a.oneOf(["local", "session", "memory"])
-        }, Sc.defaultProps = {
+        }, Ac.defaultProps = {
             hourStep: 1,
             minuteStep: 1,
             secondStep: 1,
             use12Hours: !1,
             disabled: !1,
             placement: "bottomLeft",
             format: "HH:mm:ss",
             allowClear: !0,
             bordered: !0,
             size: "middle",
             persisted_props: ["value"],
             persistence_type: "local",
             locale: "zh-cn",
             popupContainer: "body"
-        }, Sc),
-        $c = qc.RangePicker,
-        Zc = (Lc.propTypes = {
+        }, Ac),
+        ns = ts.RangePicker,
+        as = (Rc.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             locale: n.a.oneOf(["zh-cn", "en-us"]),
             hourStep: n.a.number,
             minuteStep: n.a.number,
@@ -116930,31 +117072,31 @@
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func,
             persistence: n.a.oneOfType([n.a.bool, n.a.string, n.a.number]),
             persisted_props: n.a.arrayOf(n.a.oneOf(["value"])),
             persistence_type: n.a.oneOf(["local", "session", "memory"])
-        }, Lc.defaultProps = {
+        }, Rc.defaultProps = {
             disabled: [!1, !1],
             hourStep: 1,
             minuteStep: 1,
             secondStep: 1,
             use12Hours: !1,
             allowClear: !0,
             bordered: !0,
             size: "middle",
             format: "HH:mm:ss",
             persisted_props: ["value"],
             persistence_type: "local",
             locale: "zh-cn",
             placement: "bottomLeft",
             popupContainer: "body"
-        }, Lc),
-        Jc = {
+        }, Rc),
+        rs = {
             animating: !1,
             autoplaying: null,
             currentDirection: 0,
             currentLeft: null,
             currentSlide: 0,
             direction: 1,
             dragging: !1,
@@ -116977,40 +117119,40 @@
                 curY: 0
             },
             trackStyle: {},
             trackWidth: 0,
             targetSlide: 0
         },
         l = e(152),
-        Qc = e.n(l);
+        os = e.n(l);
 
-    function ts(t, e, n) {
+    function is(t, e, n) {
         return Math.max(e, Math.min(t, n))
     }
 
-    function es(t) {
+    function ls(t) {
         ["onTouchStart", "onTouchMove", "onWheel"].includes(t._reactName) || t.preventDefault()
     }
 
-    function ns(t) {
+    function cs(t) {
         var e = 1 < arguments.length && void 0 !== arguments[1] && arguments[1],
             n = t.startX - t.curX,
             t = t.startY - t.curY,
             t = Math.atan2(t, n);
         return (n = (n = Math.round(180 * t / Math.PI)) < 0 ? 360 - Math.abs(n) : n) <= 45 && 0 <= n || n <= 360 && 315 <= n ? "left" : 135 <= n && n <= 225 ? "right" : !0 === e ? 35 <= n && n <= 135 ? "up" : "down" : "vertical"
     }
 
-    function as(e, t) {
+    function ss(e, t) {
         var n = {};
         return t.forEach(function(t) {
             return n[t] = e[t]
         }), n
     }
 
-    function rs(t, e) {
+    function us(t, e) {
         var n = function(t) {
                 for (var e = t.infinite ? 2 * t.slideCount : t.slideCount, n = t.infinite ? -1 * t.slidesToShow : 0, a = t.infinite ? -1 * t.slidesToShow : 0, r = []; n < e;) r.push(n), n = a + t.slidesToScroll, a += Math.min(t.slidesToScroll, t.slidesToShow);
                 return r
             }(t),
             a = 0;
         if (e > n[n.length - 1]) e = n[n.length - 1];
         else
@@ -117020,193 +117162,193 @@
                     break
                 }
                 a = n[r]
             }
         return e
     }
 
-    function os(e) {
+    function ds(e) {
         var n, t, a = e.centerMode ? e.slideWidth * Math.floor(e.slidesToShow / 2) : 0;
         return e.swipeToSlide ? (t = (t = e.listRef).querySelectorAll && t.querySelectorAll(".slick-slide") || [], Array.from(t).every(function(t) {
             if (e.vertical) {
-                if (t.offsetTop + ks(t) / 2 > -1 * e.swipeLeft) return n = t, !1
-            } else if (t.offsetLeft - a + ws(t) / 2 > -1 * e.swipeLeft) return n = t, !1;
+                if (t.offsetTop + Ls(t) / 2 > -1 * e.swipeLeft) return n = t, !1
+            } else if (t.offsetLeft - a + Ss(t) / 2 > -1 * e.swipeLeft) return n = t, !1;
             return !0
         }), n ? (t = !0 === e.rtl ? e.slideCount - e.currentSlide : e.currentSlide, Math.abs(n.dataset.index - t) || 1) : 0) : e.slidesToScroll
     }
 
-    function is(t) {
+    function ps(t) {
         return t.unslick || !t.infinite ? 0 : t.slideCount
     }
 
-    function ls() {
+    function fs() {
         return !("undefined" == typeof window || !window.document || !window.document.createElement)
     }
 
-    function cs(t) {
+    function hs(t) {
         var e, n, a, r, o = (r = t.rtl ? t.slideCount - 1 - t.index : t.index) < 0 || r >= t.slideCount;
         return t.centerMode ? (a = Math.floor(t.slidesToShow / 2), n = (r - t.currentSlide) % t.slideCount == 0, r > t.currentSlide - a - 1 && r <= t.currentSlide + a && (e = !0)) : e = t.currentSlide <= r && r < t.currentSlide + t.slidesToShow, {
             "slick-slide": !0,
             "slick-active": e,
             "slick-center": n,
             "slick-cloned": o,
             "slick-current": r === (t.targetSlide < 0 ? t.targetSlide + t.slideCount : t.targetSlide >= t.slideCount ? t.targetSlide - t.slideCount : t.targetSlide)
         }
     }
 
-    function ss(t, e) {
+    function ms(t, e) {
         return t.key + "-" + e
     }
 
-    function us(c) {
+    function gs(c) {
         var s, u = [],
             d = [],
             p = [],
             f = H.a.Children.count(c.children),
-            h = ys(c),
-            m = xs(c);
+            h = js(c),
+            m = Ms(c);
         return H.a.Children.forEach(c.children, function(t, e) {
             var n, a = {
                     message: "children",
                     index: e,
                     slidesToScroll: c.slidesToScroll,
                     currentSlide: c.currentSlide
                 },
                 r = !c.lazyLoad || c.lazyLoad && 0 <= c.lazyLoadedList.indexOf(e) ? t : H.a.createElement("div", null),
                 o = (o = Object(Ct.a)(Object(Ct.a)({}, c), {}, {
                     index: e
                 }), i = {}, void 0 !== o.variableWidth && !1 !== o.variableWidth || (i.width = o.slideWidth), o.fade && (i.position = "relative", o.vertical ? i.top = -o.index * parseInt(o.slideHeight) : i.left = -o.index * parseInt(o.slideWidth), i.opacity = o.currentSlide === o.index ? 1 : 0, o.useCSS) && (i.transition = "opacity " + o.speed + "ms " + o.cssEase + ", visibility " + o.speed + "ms " + o.cssEase), i),
                 i = r.props.className || "",
-                l = cs(Object(Ct.a)(Object(Ct.a)({}, c), {}, {
+                l = hs(Object(Ct.a)(Object(Ct.a)({}, c), {}, {
                     index: e
                 }));
             u.push(H.a.cloneElement(r, {
-                key: "original" + ss(r, e),
+                key: "original" + ms(r, e),
                 "data-index": e,
                 className: Kt()(l, i),
                 tabIndex: "-1",
                 "aria-hidden": !l["slick-active"],
                 style: Object(Ct.a)(Object(Ct.a)({
                     outline: "none"
                 }, r.props.style || {}), o),
                 onClick: function(t) {
                     r.props && r.props.onClick && r.props.onClick(t), c.focusOnSelect && c.focusOnSelect(a)
                 }
-            })), c.infinite && !1 === c.fade && ((n = f - e) <= Ls(c) && f !== c.slidesToShow && ((s = -n) >= h && (r = t), l = cs(Object(Ct.a)(Object(Ct.a)({}, c), {}, {
+            })), c.infinite && !1 === c.fade && ((n = f - e) <= Rs(c) && f !== c.slidesToShow && ((s = -n) >= h && (r = t), l = hs(Object(Ct.a)(Object(Ct.a)({}, c), {}, {
                 index: s
             })), d.push(H.a.cloneElement(r, {
-                key: "precloned" + ss(r, s),
+                key: "precloned" + ms(r, s),
                 "data-index": s,
                 tabIndex: "-1",
                 className: Kt()(l, i),
                 "aria-hidden": !l["slick-active"],
                 style: Object(Ct.a)(Object(Ct.a)({}, r.props.style || {}), o),
                 onClick: function(t) {
                     r.props && r.props.onClick && r.props.onClick(t), c.focusOnSelect && c.focusOnSelect(a)
                 }
-            }))), f !== c.slidesToShow) && ((s = f + e) < m && (r = t), l = cs(Object(Ct.a)(Object(Ct.a)({}, c), {}, {
+            }))), f !== c.slidesToShow) && ((s = f + e) < m && (r = t), l = hs(Object(Ct.a)(Object(Ct.a)({}, c), {}, {
                 index: s
             })), p.push(H.a.cloneElement(r, {
-                key: "postcloned" + ss(r, s),
+                key: "postcloned" + ms(r, s),
                 "data-index": s,
                 tabIndex: "-1",
                 className: Kt()(l, i),
                 "aria-hidden": !l["slick-active"],
                 style: Object(Ct.a)(Object(Ct.a)({}, r.props.style || {}), o),
                 onClick: function(t) {
                     r.props && r.props.onClick && r.props.onClick(t), c.focusOnSelect && c.focusOnSelect(a)
                 }
             })))
         }), c.rtl ? d.concat(u, p).reverse() : d.concat(u, p)
     }
 
-    function ds(t) {
+    function bs(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.autoplay,
             l = t.dotPosition,
             c = t.easing,
             s = t.effect,
             u = t.autoplaySpeed,
             d = t.speed,
             p = t.pauseOnHover,
             f = t.loading_state;
-        return t.setProps, H.a.createElement(Ws, {
+        return t.setProps, H.a.createElement(Xs, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             autoplay: i,
             dotPosition: l,
             easing: c,
             effect: s,
             autoplaySpeed: u,
             speed: d,
             pauseOnHover: p,
             "data-dash-is-loading": f && f.is_loading || void 0
         }, n)
     }
-    var ps, fs, hs, ms, gs, bs, vs = function(t) {
-            for (var e = [], n = ys(t), a = xs(t), r = n; r < a; r++) t.lazyLoadedList.indexOf(r) < 0 && e.push(r);
+    var vs, ys, xs, _s, Os, ws, ks = function(t) {
+            for (var e = [], n = js(t), a = Ms(t), r = n; r < a; r++) t.lazyLoadedList.indexOf(r) < 0 && e.push(r);
             return e
         },
-        ys = function(t) {
-            return t.currentSlide - _s(t)
+        js = function(t) {
+            return t.currentSlide - Es(t)
         },
-        xs = function(t) {
-            return t.currentSlide + Os(t)
+        Ms = function(t) {
+            return t.currentSlide + Cs(t)
         },
-        _s = function(t) {
+        Es = function(t) {
             return t.centerMode ? Math.floor(t.slidesToShow / 2) + (0 < parseInt(t.centerPadding) ? 1 : 0) : 0
         },
-        Os = function(t) {
+        Cs = function(t) {
             return t.centerMode ? Math.floor((t.slidesToShow - 1) / 2) + 1 + (0 < parseInt(t.centerPadding) ? 1 : 0) : t.slidesToShow
         },
-        ws = function(t) {
+        Ss = function(t) {
             return t && t.offsetWidth || 0
         },
-        ks = function(t) {
+        Ls = function(t) {
             return t && t.offsetHeight || 0
         },
-        js = function(t) {
+        Ps = function(t) {
             var e = !0;
             return t.infinite || (t.centerMode && t.currentSlide >= t.slideCount - 1 || t.slideCount <= t.slidesToShow || t.currentSlide >= t.slideCount - t.slidesToShow) && (e = !1), e
         },
-        Ms = function(n, t) {
+        Ds = function(n, t) {
             return t.reduce(function(t, e) {
                 return t && n.hasOwnProperty(e)
             }, !0) ? null : console.error("Keys Missing:", n)
         },
-        Es = function(t) {
-            Ms(t, ["left", "variableWidth", "slideCount", "slidesToShow", "slideWidth"]);
+        Ts = function(t) {
+            Ds(t, ["left", "variableWidth", "slideCount", "slidesToShow", "slideWidth"]);
             var e, n, a, r, o, i = t.slideCount + 2 * t.slidesToShow,
-                i = (t.vertical ? n = i * t.slideHeight : e = Ps(t) * t.slideWidth, {
+                i = (t.vertical ? n = i * t.slideHeight : e = Is(t) * t.slideWidth, {
                     opacity: 1,
                     transition: "",
                     WebkitTransition: ""
                 });
             return t.useTransform ? (a = t.vertical ? "translate3d(0px, " + t.left + "px, 0px)" : "translate3d(" + t.left + "px, 0px, 0px)", r = t.vertical ? "translate3d(0px, " + t.left + "px, 0px)" : "translate3d(" + t.left + "px, 0px, 0px)", o = t.vertical ? "translateY(" + t.left + "px)" : "translateX(" + t.left + "px)", i = Object(Ct.a)(Object(Ct.a)({}, i), {}, {
                 WebkitTransform: a,
                 transform: r,
                 msTransform: o
             })) : t.vertical ? i.top = t.left : i.left = t.left, t.fade && (i = {
                 opacity: 1
             }), e && (i.width = e), n && (i.height = n), window && !window.addEventListener && window.attachEvent && (t.vertical ? i.marginTop = t.left + "px" : i.marginLeft = t.left + "px"), i
         },
-        Cs = function(t) {
-            Ms(t, ["left", "variableWidth", "slideCount", "slidesToShow", "slideWidth", "speed", "cssEase"]);
-            var e = Es(t);
+        zs = function(t) {
+            Ds(t, ["left", "variableWidth", "slideCount", "slidesToShow", "slideWidth", "speed", "cssEase"]);
+            var e = Ts(t);
             return t.useTransform ? (e.WebkitTransition = "-webkit-transform " + t.speed + "ms " + t.cssEase, e.transition = "transform " + t.speed + "ms " + t.cssEase) : t.vertical ? e.transition = "top " + t.speed + "ms " + t.cssEase : e.transition = "left " + t.speed + "ms " + t.cssEase, e
         },
-        Ss = function(t) {
+        As = function(t) {
             if (t.unslick) return 0;
-            Ms(t, ["slideIndex", "trackRef", "infinite", "centerMode", "slideCount", "slidesToShow", "slidesToScroll", "slideWidth", "listWidth", "variableWidth", "slideHeight"]);
+            Ds(t, ["slideIndex", "trackRef", "infinite", "centerMode", "slideCount", "slidesToShow", "slidesToScroll", "slideWidth", "listWidth", "variableWidth", "slideHeight"]);
             var e = t.slideIndex,
                 n = t.trackRef,
                 a = t.infinite,
                 r = t.centerMode,
                 o = t.slideCount,
                 i = t.slidesToShow,
                 l = t.slidesToScroll,
@@ -117214,30 +117356,30 @@
                 s = t.listWidth,
                 u = t.variableWidth,
                 d = t.slideHeight,
                 p = t.fade,
                 f = t.vertical;
             if (p || 1 === t.slideCount) return 0;
             p = 0;
-            if (a ? (p = -Ls(t), o % l != 0 && o < e + l && (p = -(o < e ? i - (e - o) : o % l)), r && (p += parseInt(i / 2))) : (o % l != 0 && o < e + l && (p = i - o % l), r && (p = parseInt(i / 2))), g = f ? e * d * -1 + p * d : e * c * -1 + p * c, !0 === u) {
+            if (a ? (p = -Rs(t), o % l != 0 && o < e + l && (p = -(o < e ? i - (e - o) : o % l)), r && (p += parseInt(i / 2))) : (o % l != 0 && o < e + l && (p = i - o % l), r && (p = parseInt(i / 2))), g = f ? e * d * -1 + p * d : e * c * -1 + p * c, !0 === u) {
                 var h = n && n.node;
-                if (m = e + Ls(t), g = (o = h && h.childNodes[m]) ? -1 * o.offsetLeft : 0, !0 === r) {
-                    for (var m = a ? e + Ls(t) : e, o = h && h.children[m], g = 0, b = 0; b < m; b++) g -= h && h.children[b] && h.children[b].offsetWidth;
+                if (m = e + Rs(t), g = (o = h && h.childNodes[m]) ? -1 * o.offsetLeft : 0, !0 === r) {
+                    for (var m = a ? e + Rs(t) : e, o = h && h.children[m], g = 0, b = 0; b < m; b++) g -= h && h.children[b] && h.children[b].offsetWidth;
                     g = (g -= parseInt(t.centerPadding)) + (o && (s - o.offsetWidth) / 2)
                 }
             }
             return g
         },
-        Ls = function(t) {
+        Rs = function(t) {
             return t.unslick || !t.infinite ? 0 : t.variableWidth ? t.slideCount : t.slidesToShow + (t.centerMode ? 1 : 0)
         },
-        Ps = function(t) {
-            return 1 === t.slideCount ? 1 : Ls(t) + t.slideCount + is(t)
+        Is = function(t) {
+            return 1 === t.slideCount ? 1 : Rs(t) + t.slideCount + ps(t)
         },
-        Ds = function(t) {
+        Ns = function(t) {
             return t.targetSlide > t.currentSlide ? t.targetSlide > t.currentSlide + function(t) {
                 var e = t.slidesToShow,
                     n = t.centerMode,
                     a = t.rtl,
                     r = t.centerPadding;
                 if (n) {
                     var o = (e - 1) / 2 + 1;
@@ -117252,32 +117394,32 @@
                 if (n) {
                     var o = (e - 1) / 2 + 1;
                     return parseInt(r) > 0 && (o += 1), a || e % 2 != 0 || (o += 1), o
                 }
                 return a ? e - 1 : 0
             }(t) ? "right" : "left"
         },
-        Ts = (c = H.a.PureComponent, Object(r.a)(Xs, c), bs = Object(o.a)(Xs), Object(a.a)(Xs, [{
+        Ys = (c = H.a.PureComponent, Object(r.a)(eu, c), ws = Object(o.a)(eu), Object(a.a)(eu, [{
             key: "render",
             value: function() {
-                var t = us(this.props),
+                var t = gs(this.props),
                     e = this.props,
                     e = {
                         onMouseEnter: e.onMouseEnter,
                         onMouseOver: e.onMouseOver,
                         onMouseLeave: e.onMouseLeave
                     };
                 return H.a.createElement("div", Object(Et.a)({
                     ref: this.handleRef,
                     className: "slick-track",
                     style: this.props.trackStyle
                 }, e), t)
             }
-        }]), Xs),
-        zs = (d = H.a.PureComponent, Object(r.a)(qs, d), gs = Object(o.a)(qs), Object(a.a)(qs, [{
+        }]), eu),
+        Bs = (d = H.a.PureComponent, Object(r.a)(tu, d), Os = Object(o.a)(tu), Object(a.a)(tu, [{
             key: "clickHandler",
             value: function(t, e) {
                 e.preventDefault(), this.props.clickHandler(t)
             }
         }, {
             key: "render",
             value: function() {
@@ -117287,17 +117429,17 @@
                         slidesToShow: i,
                         infinite: r
                     }).infinite ? Math.ceil(t.slideCount / t.slidesToScroll) : Math.ceil((t.slideCount - t.slidesToShow) / t.slidesToScroll) + 1, i = {
                         onMouseEnter: e,
                         onMouseOver: n,
                         onMouseLeave: a
                     }, u = [], d = 0; d < s; d++) var p = (d + 1) * o - 1,
-                    p = r ? p : ts(p, 0, l - 1),
+                    p = r ? p : is(p, 0, l - 1),
                     f = p - (o - 1),
-                    f = r ? f : ts(f, 0, l - 1),
+                    f = r ? f : is(f, 0, l - 1),
                     p = Kt()({
                         "slick-active": r ? f <= c && c <= p : c === f
                     }),
                     f = this.clickHandler.bind(this, {
                         message: "dots",
                         index: d,
                         slidesToScroll: o,
@@ -117309,16 +117451,16 @@
                     }, H.a.cloneElement(this.props.customPaging(d), {
                         onClick: f
                     })));
                 return H.a.cloneElement(this.props.appendDots(u), Object(Ct.a)({
                     className: this.props.dotsClass
                 }, i))
             }
-        }]), qs),
-        As = (p = H.a.PureComponent, Object(r.a)(Gs, p), ms = Object(o.a)(Gs), Object(a.a)(Gs, [{
+        }]), tu),
+        Fs = (p = H.a.PureComponent, Object(r.a)(Qs, p), _s = Object(o.a)(Qs), Object(a.a)(Qs, [{
             key: "clickHandler",
             value: function(t, e) {
                 e && e.preventDefault(), this.props.clickHandler(t, e)
             }
         }, {
             key: "render",
             value: function() {
@@ -117343,31 +117485,31 @@
                         slideCount: this.props.slideCount
                     };
                 return this.props.prevArrow ? H.a.cloneElement(this.props.prevArrow, Object(Ct.a)(Object(Ct.a)({}, t), e)) : H.a.createElement("button", Object(Et.a)({
                     key: "0",
                     type: "button"
                 }, t), " ", "Previous")
             }
-        }]), Gs),
-        Rs = (l = H.a.PureComponent, Object(r.a)(Us, l), hs = Object(o.a)(Us), Object(a.a)(Us, [{
+        }]), Qs),
+        Hs = (l = H.a.PureComponent, Object(r.a)(Js, l), xs = Object(o.a)(Js), Object(a.a)(Js, [{
             key: "clickHandler",
             value: function(t, e) {
                 e && e.preventDefault(), this.props.clickHandler(t, e)
             }
         }, {
             key: "render",
             value: function() {
                 var t = {
                         "slick-arrow": !0,
                         "slick-next": !0
                     },
                     e = this.clickHandler.bind(this, {
                         message: "next"
                     }),
-                    t = (js(this.props) || (t["slick-disabled"] = !0, e = null), {
+                    t = (Ps(this.props) || (t["slick-disabled"] = !0, e = null), {
                         key: "1",
                         "data-role": "none",
                         className: Kt()(t),
                         style: {
                             display: "block"
                         },
                         onClick: e
@@ -117377,18 +117519,18 @@
                         slideCount: this.props.slideCount
                     };
                 return this.props.nextArrow ? H.a.cloneElement(this.props.nextArrow, Object(Ct.a)(Object(Ct.a)({}, t), e)) : H.a.createElement("button", Object(Et.a)({
                     key: "1",
                     type: "button"
                 }, t), " ", "Next")
             }
-        }]), Us),
-        Is = e(140),
-        Ns = ["animating"],
-        Ys = (c = H.a.Component, Object(r.a)(Ks, c), fs = Object(o.a)(Ks), Object(a.a)(Ks, [{
+        }]), Js),
+        Ws = e(140),
+        Vs = ["animating"],
+        Ks = (c = H.a.Component, Object(r.a)(Zs, c), ys = Object(o.a)(Zs), Object(a.a)(Zs, [{
             key: "didPropsChange",
             value: function(t) {
                 for (var e = !1, n = 0, a = Object.keys(this.props); n < a.length; n++) {
                     var r = a[n];
                     if (!t.hasOwnProperty(r)) {
                         e = !0;
                         break
@@ -117396,18 +117538,18 @@
                     if ("object" !== Object(qt.a)(t[r]) && "function" != typeof t[r] && t[r] !== this.props[r]) {
                         e = !0;
                         break
                     }
                 }
                 return e || H.a.Children.count(this.props.children) !== H.a.Children.count(t.children)
             }
-        }]), Ks),
+        }]), Zs),
         d = e(288),
-        Bs = e.n(d),
-        Fs = {
+        Us = e.n(d),
+        Gs = {
             accessibility: !0,
             adaptiveHeight: !1,
             afterChange: null,
             appendDots: function(t) {
                 return H.a.createElement("ul", {
                     style: {
                         display: "block"
@@ -117459,15 +117601,15 @@
             touchThreshold: 5,
             useCSS: !0,
             useTransform: !0,
             variableWidth: !1,
             vertical: !1,
             waitForAnimate: !0
         },
-        Hs = (p = H.a.Component, Object(r.a)(Vs, p), ps = Object(o.a)(Vs), Object(a.a)(Vs, [{
+        qs = (p = H.a.Component, Object(r.a)($s, p), vs = Object(o.a)($s), Object(a.a)($s, [{
             key: "media",
             value: function(t, e) {
                 function n(t) {
                     t.matches && e()
                 }
                 var a = window.matchMedia(t);
                 a.addListener(n), n(a), this._responsiveMediaHandlers.push({
@@ -117481,29 +117623,29 @@
             value: function() {
                 var n, t, a = this;
                 this.props.responsive && ((n = this.props.responsive.map(function(t) {
                     return t.breakpoint
                 })).sort(function(t, e) {
                     return t - e
                 }), n.forEach(function(t, e) {
-                    e = 0 === e ? Bs()({
+                    e = 0 === e ? Us()({
                         minWidth: 0,
                         maxWidth: t
-                    }) : Bs()({
+                    }) : Us()({
                         minWidth: n[e - 1] + 1,
                         maxWidth: t
                     });
-                    ls() && a.media(e, function() {
+                    fs() && a.media(e, function() {
                         a.setState({
                             breakpoint: t
                         })
                     })
-                }), t = Bs()({
+                }), t = Us()({
                     minWidth: n.slice(-1)[0]
-                }), ls()) && this.media(t, function() {
+                }), fs()) && this.media(t, function() {
                     a.setState({
                         breakpoint: null
                     })
                 })
             }
         }, {
             key: "componentWillUnmount",
@@ -117514,15 +117656,15 @@
             }
         }, {
             key: "render",
             value: function() {
                 var t, e = this;
                 (t = this.state.breakpoint ? "unslick" === (a = this.props.responsive.filter(function(t) {
                     return t.breakpoint === e.state.breakpoint
-                }))[0].settings ? "unslick" : Object(Ct.a)(Object(Ct.a)(Object(Ct.a)({}, Fs), this.props), a[0].settings) : Object(Ct.a)(Object(Ct.a)({}, Fs), this.props)).centerMode && (t.slidesToScroll, t.slidesToScroll = 1), t.fade && (t.slidesToShow, t.slidesToScroll, t.slidesToShow = 1, t.slidesToScroll = 1);
+                }))[0].settings ? "unslick" : Object(Ct.a)(Object(Ct.a)(Object(Ct.a)({}, Gs), this.props), a[0].settings) : Object(Ct.a)(Object(Ct.a)({}, Gs), this.props)).centerMode && (t.slidesToScroll, t.slidesToScroll = 1), t.fade && (t.slidesToShow, t.slidesToScroll, t.slidesToShow = 1, t.slidesToScroll = 1);
                 var n = (n = H.a.Children.toArray(this.props.children)).filter(function(t) {
                     return "string" == typeof t ? !!t.trim() : !!t
                 });
                 t.variableWidth && (1 < t.rows || 1 < t.slidesPerRow) && (console.warn("variableWidth is not supported in case of rows > 1 or slidesPerRow > 1"), t.variableWidth = !1);
                 for (var a, r = [], o = null, i = 0; i < n.length; i += t.rows * t.slidesPerRow) {
                     for (var l = [], c = i; c < i + t.rows * t.slidesPerRow; c += t.slidesPerRow) {
                         for (var s = [], u = c; u < c + t.slidesPerRow && (t.variableWidth && n[u].props.style && (o = n[u].props.style.width), !(u >= n.length)); u += 1) s.push(H.a.cloneElement(n[u], {
@@ -117544,21 +117686,21 @@
                         }
                     }, l)) : r.push(H.a.createElement("div", {
                         key: i
                     }, l))
                 }
                 return "unslick" === t ? (a = "regular slider " + (this.props.className || ""), H.a.createElement("div", {
                     className: a
-                }, n)) : (r.length <= t.slidesToShow && (t.unslick = !0), H.a.createElement(Ys, Object(Et.a)({
+                }, n)) : (r.length <= t.slidesToShow && (t.unslick = !0), H.a.createElement(Ks, Object(Et.a)({
                     style: this.props.style,
                     ref: this.innerSliderRefHandler
                 }, t), r))
             }
-        }]), Vs),
-        Ws = Wt.forwardRef(function(t, e) {
+        }]), $s),
+        Xs = Wt.forwardRef(function(t, e) {
             function n(t) {
                 d.current.slickGoTo(t, 1 < arguments.length && void 0 !== arguments[1] && arguments[1])
             }
             var a, r = t.dots,
                 r = void 0 === r || r,
                 o = t.arrows,
                 o = void 0 !== o && o,
@@ -117595,27 +117737,27 @@
                 }, s)),
                 c = ("fade" === e.effect && (e.fade = !0), u("carousel", e.prefixCls)),
                 u = !!r,
                 r = Kt()("slick-dots", "".concat("slick-dots", "-").concat(l), "boolean" != typeof r && (null == r ? void 0 : r.className)),
                 t = Kt()(c, (a = {}, Object(Vt.a)(a, "".concat(c, "-rtl"), "rtl" === t), Object(Vt.a)(a, "".concat(c, "-vertical"), "left" === l || "right" === l), a));
             return Wt.createElement("div", {
                 className: t
-            }, Wt.createElement(Hs, Object(Et.a)({
+            }, Wt.createElement(qs, Object(Et.a)({
                 ref: d
             }, e, {
                 dots: u,
                 dotsClass: r,
                 arrows: o,
                 draggable: i
             })))
         });
 
-    function Vs(t) {
+    function $s(t) {
         var e;
-        return Object(i.a)(this, Vs), e = ps.call(this, t), Object(Vt.a)(Object(s.a)(e), "innerSliderRefHandler", function(t) {
+        return Object(i.a)(this, $s), e = vs.call(this, t), Object(Vt.a)(Object(s.a)(e), "innerSliderRefHandler", function(t) {
             return e.innerSlider = t
         }), Object(Vt.a)(Object(s.a)(e), "slickPrev", function() {
             return e.innerSlider.slickPrev()
         }), Object(Vt.a)(Object(s.a)(e), "slickNext", function() {
             return e.innerSlider.slickNext()
         }), Object(Vt.a)(Object(s.a)(e), "slickGoTo", function(t) {
             return e.innerSlider.slickGoTo(t, 1 < arguments.length && void 0 !== arguments[1] && arguments[1])
@@ -117624,47 +117766,47 @@
         }), Object(Vt.a)(Object(s.a)(e), "slickPlay", function() {
             return e.innerSlider.autoPlay("play")
         }), e.state = {
             breakpoint: null
         }, e._responsiveMediaHandlers = [], e
     }
 
-    function Ks(t) {
-        Object(i.a)(this, Ks), f = fs.call(this, t), Object(Vt.a)(Object(s.a)(f), "listRefHandler", function(t) {
+    function Zs(t) {
+        Object(i.a)(this, Zs), f = ys.call(this, t), Object(Vt.a)(Object(s.a)(f), "listRefHandler", function(t) {
             return f.list = t
         }), Object(Vt.a)(Object(s.a)(f), "trackRefHandler", function(t) {
             return f.track = t
         }), Object(Vt.a)(Object(s.a)(f), "adaptHeight", function() {
             var t;
-            f.props.adaptiveHeight && f.list && (t = f.list.querySelector('[data-index="'.concat(f.state.currentSlide, '"]')), f.list.style.height = ks(t) + "px")
+            f.props.adaptiveHeight && f.list && (t = f.list.querySelector('[data-index="'.concat(f.state.currentSlide, '"]')), f.list.style.height = Ls(t) + "px")
         }), Object(Vt.a)(Object(s.a)(f), "componentDidMount", function() {
-            f.props.onInit && f.props.onInit(), f.props.lazyLoad && 0 < (e = vs(Object(Ct.a)(Object(Ct.a)({}, f.props), f.state))).length && (f.setState(function(t) {
+            f.props.onInit && f.props.onInit(), f.props.lazyLoad && 0 < (e = ks(Object(Ct.a)(Object(Ct.a)({}, f.props), f.state))).length && (f.setState(function(t) {
                 return {
                     lazyLoadedList: t.lazyLoadedList.concat(e)
                 }
             }), f.props.onLazyLoad) && f.props.onLazyLoad(e);
             var e, t = Object(Ct.a)({
                 listRef: f.list,
                 trackRef: f.track
             }, f.props);
             f.updateState(t, !0, function() {
                 f.adaptHeight(), f.props.autoplay && f.autoPlay("playing")
-            }), "progressive" === f.props.lazyLoad && (f.lazyLoadTimer = setInterval(f.progressiveLazyLoad, 1e3)), f.ro = new Is.a(function() {
+            }), "progressive" === f.props.lazyLoad && (f.lazyLoadTimer = setInterval(f.progressiveLazyLoad, 1e3)), f.ro = new Ws.a(function() {
                 f.state.animating ? (f.onWindowResized(!1), f.callbackTimers.push(setTimeout(function() {
                     return f.onWindowResized()
                 }, f.props.speed))) : f.onWindowResized()
             }), f.ro.observe(f.list), document.querySelectorAll && Array.prototype.forEach.call(document.querySelectorAll(".slick-slide"), function(t) {
                 t.onfocus = f.props.pauseOnFocus ? f.onSlideFocus : null, t.onblur = f.props.pauseOnFocus ? f.onSlideBlur : null
             }), window.addEventListener ? window.addEventListener("resize", f.onWindowResized) : window.attachEvent("onresize", f.onWindowResized)
         }), Object(Vt.a)(Object(s.a)(f), "componentWillUnmount", function() {
             f.animationEndCallback && clearTimeout(f.animationEndCallback), f.lazyLoadTimer && clearInterval(f.lazyLoadTimer), f.callbackTimers.length && (f.callbackTimers.forEach(function(t) {
                 return clearTimeout(t)
             }), f.callbackTimers = []), window.addEventListener ? window.removeEventListener("resize", f.onWindowResized) : window.detachEvent("onresize", f.onWindowResized), f.autoplayTimer && clearInterval(f.autoplayTimer), f.ro.disconnect()
         }), Object(Vt.a)(Object(s.a)(f), "componentDidUpdate", function(t) {
-            f.checkImagesLoad(), f.props.onReInit && f.props.onReInit(), f.props.lazyLoad && 0 < (e = vs(Object(Ct.a)(Object(Ct.a)({}, f.props), f.state))).length && (f.setState(function(t) {
+            f.checkImagesLoad(), f.props.onReInit && f.props.onReInit(), f.props.lazyLoad && 0 < (e = ks(Object(Ct.a)(Object(Ct.a)({}, f.props), f.state))).length && (f.setState(function(t) {
                 return {
                     lazyLoadedList: t.lazyLoadedList.concat(e)
                 }
             }), f.props.onLazyLoad) && f.props.onLazyLoad(e), f.adaptHeight();
             var e, n = Object(Ct.a)(Object(Ct.a)({
                     listRef: f.list,
                     trackRef: f.track
@@ -117674,29 +117816,29 @@
                 f.state.currentSlide >= H.a.Children.count(f.props.children) && f.changeSlide({
                     message: "index",
                     index: H.a.Children.count(f.props.children) - f.props.slidesToShow,
                     currentSlide: f.state.currentSlide
                 }), t.autoplay === f.props.autoplay && t.autoplaySpeed === f.props.autoplaySpeed || (!t.autoplay && f.props.autoplay ? f.autoPlay("playing") : f.props.autoplay ? f.autoPlay("update") : f.pause("paused"))
             })
         }), Object(Vt.a)(Object(s.a)(f), "onWindowResized", function(t) {
-            f.debouncedResize && f.debouncedResize.cancel(), f.debouncedResize = Qc()(function() {
+            f.debouncedResize && f.debouncedResize.cancel(), f.debouncedResize = os()(function() {
                 return f.resizeWindow(t)
             }, 50), f.debouncedResize()
         }), Object(Vt.a)(Object(s.a)(f), "resizeWindow", function() {
             var t, e = !(0 < arguments.length && void 0 !== arguments[0]) || arguments[0];
             Boolean(f.track && f.track.node) && (t = Object(Ct.a)(Object(Ct.a)({
                 listRef: f.list,
                 trackRef: f.track
             }, f.props), f.state), f.updateState(t, e, function() {
                 f.props.autoplay ? f.autoPlay("update") : f.pause("paused")
             }), f.setState({
                 animating: !1
             }), clearTimeout(f.animationEndCallback), delete f.animationEndCallback)
         }), Object(Vt.a)(Object(s.a)(f), "updateState", function(t, e, n) {
-            a = t, r = H.a.Children.count(a.children), o = a.listRef, d = Math.ceil(ws(o)), p = a.trackRef && a.trackRef.node, p = Math.ceil(ws(p)), u = a.vertical ? d : (u = a.centerMode && 2 * parseInt(a.centerPadding), "string" == typeof a.centerPadding && "%" === a.centerPadding.slice(-1) && (u *= d / 100), Math.ceil((d - u) / a.slidesToShow)), o = o && ks(o.querySelector('[data-index="0"]')), i = o * a.slidesToShow, l = void 0 === a.currentSlide ? a.initialSlide : a.currentSlide, a.rtl && void 0 === a.currentSlide && (l = r - 1 - a.initialSlide), c = a.lazyLoadedList || [], s = vs(Object(Ct.a)(Object(Ct.a)({}, a), {}, {
+            a = t, r = H.a.Children.count(a.children), o = a.listRef, d = Math.ceil(Ss(o)), p = a.trackRef && a.trackRef.node, p = Math.ceil(Ss(p)), u = a.vertical ? d : (u = a.centerMode && 2 * parseInt(a.centerPadding), "string" == typeof a.centerPadding && "%" === a.centerPadding.slice(-1) && (u *= d / 100), Math.ceil((d - u) / a.slidesToShow)), o = o && Ls(o.querySelector('[data-index="0"]')), i = o * a.slidesToShow, l = void 0 === a.currentSlide ? a.initialSlide : a.currentSlide, a.rtl && void 0 === a.currentSlide && (l = r - 1 - a.initialSlide), c = a.lazyLoadedList || [], s = ks(Object(Ct.a)(Object(Ct.a)({}, a), {}, {
                 currentSlide: l,
                 lazyLoadedList: c
             })), r = {
                 slideCount: r,
                 slideWidth: u,
                 listWidth: d,
                 trackWidth: p,
@@ -117704,28 +117846,28 @@
                 slideHeight: o,
                 listHeight: i,
                 lazyLoadedList: c = c.concat(s)
             }, null === a.autoplaying && a.autoplay && (r.autoplaying = "playing");
             var a, r, o, i, l, c, s, u = r,
                 d = (t = Object(Ct.a)(Object(Ct.a)(Object(Ct.a)({}, t), u), {}, {
                     slideIndex: u.currentSlide
-                }), Ss(t)),
+                }), As(t)),
                 p = (t = Object(Ct.a)(Object(Ct.a)({}, t), {}, {
                     left: d
-                }), Es(t));
+                }), Ts(t));
             !e && H.a.Children.count(f.props.children) === H.a.Children.count(t.children) || (u.trackStyle = p), f.setState(u, n)
         }), Object(Vt.a)(Object(s.a)(f), "ssrInit", function() {
             if (f.props.variableWidth) {
                 var e = 0,
                     t = 0,
                     n = [],
-                    a = Ls(Object(Ct.a)(Object(Ct.a)(Object(Ct.a)({}, f.props), f.state), {}, {
+                    a = Rs(Object(Ct.a)(Object(Ct.a)(Object(Ct.a)({}, f.props), f.state), {}, {
                         slideCount: f.props.children.length
                     })),
-                    r = is(Object(Ct.a)(Object(Ct.a)(Object(Ct.a)({}, f.props), f.state), {}, {
+                    r = ps(Object(Ct.a)(Object(Ct.a)(Object(Ct.a)({}, f.props), f.state), {}, {
                         slideCount: f.props.children.length
                     }));
                 f.props.children.forEach(function(t) {
                     n.push(t.props.style.width), e += t.props.style.width
                 });
                 for (var o = 0; o < a; o++) t += n[n.length - 1 - o], e += n[n.length - 1 - o];
                 for (var i = 0; i < r; i++) e += n[i];
@@ -117738,18 +117880,18 @@
                     trackStyle: c
                 }
             }
             var s = H.a.Children.count(f.props.children),
                 c = Object(Ct.a)(Object(Ct.a)(Object(Ct.a)({}, f.props), f.state), {}, {
                     slideCount: s
                 }),
-                s = Ls(c) + is(c) + s,
+                s = Rs(c) + ps(c) + s,
                 u = 100 / f.props.slidesToShow * s,
                 s = 100 / s,
-                c = -s * (Ls(c) + f.state.currentSlide) * u / 100;
+                c = -s * (Rs(c) + f.state.currentSlide) * u / 100;
             return f.props.centerMode && (c += (100 - s * u / 100) / 2), {
                 slideWidth: s + "%",
                 trackStyle: {
                     width: u + "%",
                     left: c + "%"
                 }
             }
@@ -117769,19 +117911,19 @@
                 }, t.onload || (f.props.lazyLoad ? t.onload = function() {
                     f.adaptHeight(), f.callbackTimers.push(setTimeout(f.onWindowResized, f.props.speed))
                 } : (t.onload = e, t.onerror = function() {
                     e(), f.props.onLazyLoadError && f.props.onLazyLoadError()
                 }))
             })
         }), Object(Vt.a)(Object(s.a)(f), "progressiveLazyLoad", function() {
-            for (var e = [], t = Object(Ct.a)(Object(Ct.a)({}, f.props), f.state), n = f.state.currentSlide; n < f.state.slideCount + is(t); n++)
+            for (var e = [], t = Object(Ct.a)(Object(Ct.a)({}, f.props), f.state), n = f.state.currentSlide; n < f.state.slideCount + ps(t); n++)
                 if (f.state.lazyLoadedList.indexOf(n) < 0) {
                     e.push(n);
                     break
-                } for (var a = f.state.currentSlide - 1; a >= -Ls(t); a--)
+                } for (var a = f.state.currentSlide - 1; a >= -Rs(t); a--)
                 if (f.state.lazyLoadedList.indexOf(a) < 0) {
                     e.push(a);
                     break
                 } 0 < e.length ? (f.setState(function(t) {
                 return {
                     lazyLoadedList: t.lazyLoadedList.concat(e)
                 }
@@ -117809,51 +117951,51 @@
                         d = t.slidesToShow,
                         p = t.useCSS,
                         f = t.lazyLoadedList;
                     if (e && n) return {};
                     var e = o,
                         n = {},
                         h = {},
-                        m = r ? o : ts(o, 0, i - 1);
+                        m = r ? o : is(o, 0, i - 1);
                     if (a) {
                         if (!r && (o < 0 || i <= o)) return {};
                         o < 0 ? e = o + i : i <= o && (e = o - i), h = {
                             animating: !(n = {
                                 animating: !0,
                                 currentSlide: e,
                                 lazyLoadedList: f = l && f.indexOf(e) < 0 ? f.concat(e) : f,
                                 targetSlide: e
                             }),
                             targetSlide: e
                         }
-                    } else(a = e) < 0 ? (a = e + i, r ? i % u != 0 && (a = i - i % u) : a = 0) : !js(t) && c < e ? e = a = c : s && i <= e ? (e = r ? i : i - 1, a = r ? 0 : i - 1) : i <= e && (a = e - i, r ? i % u != 0 && (a = 0) : a = i - d), !r && i <= e + d && (a = i - d), o = Ss(Object(Ct.a)(Object(Ct.a)({}, t), {}, {
+                    } else(a = e) < 0 ? (a = e + i, r ? i % u != 0 && (a = i - i % u) : a = 0) : !Ps(t) && c < e ? e = a = c : s && i <= e ? (e = r ? i : i - 1, a = r ? 0 : i - 1) : i <= e && (a = e - i, r ? i % u != 0 && (a = 0) : a = i - d), !r && i <= e + d && (a = i - d), o = As(Object(Ct.a)(Object(Ct.a)({}, t), {}, {
                         slideIndex: e
-                    })), c = Ss(Object(Ct.a)(Object(Ct.a)({}, t), {}, {
+                    })), c = As(Object(Ct.a)(Object(Ct.a)({}, t), {}, {
                         slideIndex: a
-                    })), r || (o === c && (e = a), o = c), l && (f = f.concat(vs(Object(Ct.a)(Object(Ct.a)({}, t), {}, {
+                    })), r || (o === c && (e = a), o = c), l && (f = f.concat(ks(Object(Ct.a)(Object(Ct.a)({}, t), {}, {
                         currentSlide: e
                     })))), p ? h = {
                         animating: !(n = {
                             animating: !0,
                             currentSlide: a,
-                            trackStyle: Cs(Object(Ct.a)(Object(Ct.a)({}, t), {}, {
+                            trackStyle: zs(Object(Ct.a)(Object(Ct.a)({}, t), {}, {
                                 left: o
                             })),
                             lazyLoadedList: f,
                             targetSlide: m
                         }),
                         currentSlide: a,
-                        trackStyle: Es(Object(Ct.a)(Object(Ct.a)({}, t), {}, {
+                        trackStyle: Ts(Object(Ct.a)(Object(Ct.a)({}, t), {}, {
                             left: c
                         })),
                         swipeLeft: null,
                         targetSlide: m
                     } : n = {
                         currentSlide: a,
-                        trackStyle: Es(Object(Ct.a)(Object(Ct.a)({}, t), {}, {
+                        trackStyle: Ts(Object(Ct.a)(Object(Ct.a)({}, t), {}, {
                             left: c
                         })),
                         lazyLoadedList: f,
                         targetSlide: m
                     };
                     return {
                         state: n,
@@ -117868,28 +118010,28 @@
                 c = e.state,
                 s = e.nextState;
             c && (r && r(n, c.currentSlide), e = c.lazyLoadedList.filter(function(t) {
                 return f.state.lazyLoadedList.indexOf(t) < 0
             }), o && 0 < e.length && o(e), !f.props.waitForAnimate && f.animationEndCallback && (clearTimeout(f.animationEndCallback), l && l(n), delete f.animationEndCallback), f.setState(c, function() {
                 a && f.asNavForIndex !== t && (f.asNavForIndex = t, a.innerSlider.slideHandler(t)), s && (f.animationEndCallback = setTimeout(function() {
                     var t = s.animating,
-                        e = Object(Bt.a)(s, Ns);
+                        e = Object(Jt.a)(s, Vs);
                     f.setState(e, function() {
                         f.callbackTimers.push(setTimeout(function() {
                             return f.setState({
                                 animating: t
                             })
                         }, 10)), l && l(c.currentSlide), delete f.animationEndCallback
                     })
                 }, i))
             }))
         }), Object(Vt.a)(Object(s.a)(f), "changeSlide", function(t) {
             var e, n, a, r, o, i, l, c, s, u = 1 < arguments.length && void 0 !== arguments[1] && arguments[1],
                 d = Object(Ct.a)(Object(Ct.a)({}, f.props), f.state),
-                p = (t = t, n = (d = d).slidesToScroll, a = d.slidesToShow, r = d.slideCount, o = d.currentSlide, i = d.targetSlide, s = d.lazyLoad, l = d.infinite, c = r % n != 0 ? 0 : (r - o) % n, "previous" === t.message ? (e = o - (p = 0 == c ? n : a - c), s && !l && (e = -1 == (a = o - p) ? r - 1 : a), l || (e = i - n)) : "next" === t.message ? (e = o + (p = 0 == c ? n : c), s && !l && (e = (o + n) % r + c), l || (e = i + n)) : "dots" === t.message ? e = t.index * t.slidesToScroll : "children" === t.message ? (e = t.index, l && (a = Ds(Object(Ct.a)(Object(Ct.a)({}, d), {}, {
+                p = (t = t, n = (d = d).slidesToScroll, a = d.slidesToShow, r = d.slideCount, o = d.currentSlide, i = d.targetSlide, s = d.lazyLoad, l = d.infinite, c = r % n != 0 ? 0 : (r - o) % n, "previous" === t.message ? (e = o - (p = 0 == c ? n : a - c), s && !l && (e = -1 == (a = o - p) ? r - 1 : a), l || (e = i - n)) : "next" === t.message ? (e = o + (p = 0 == c ? n : c), s && !l && (e = (o + n) % r + c), l || (e = i + n)) : "dots" === t.message ? e = t.index * t.slidesToScroll : "children" === t.message ? (e = t.index, l && (a = Ns(Object(Ct.a)(Object(Ct.a)({}, d), {}, {
                     targetSlide: e
                 })), e > t.currentSlide && "left" === a ? e -= r : e < t.currentSlide && "right" === a && (e += r))) : "index" === t.message && (e = Number(t.index)), e);
             (0 === p || p) && (!0 === u ? f.slideHandler(p, u) : f.slideHandler(p), f.props.autoplay && f.autoPlay("update"), f.props.focusOnSelect) && (s = f.list.querySelectorAll(".slick-current"))[0] && s[0].focus()
         }), Object(Vt.a)(Object(s.a)(f), "clickHandler", function(t) {
             !1 === f.clickable && (t.stopPropagation(), t.preventDefault()), f.clickable = !0
         }), Object(Vt.a)(Object(s.a)(f), "keyHandler", function(t) {
             t = t, n = f.props.accessibility, e = f.props.rtl;
@@ -117903,15 +118045,15 @@
             window.ontouchmove = function(t) {
                 (t = t || window.event).preventDefault && t.preventDefault(), t.returnValue = !1
             }
         }), Object(Vt.a)(Object(s.a)(f), "enableBodyScroll", function() {
             window.ontouchmove = null
         }), Object(Vt.a)(Object(s.a)(f), "swipeStart", function(t) {
             f.props.verticalSwiping && f.disableBodyScroll();
-            t = t, n = f.props.swipe, e = f.props.draggable, "IMG" === t.target.tagName && es(t);
+            t = t, n = f.props.swipe, e = f.props.draggable, "IMG" === t.target.tagName && ls(t);
             var e, n = !n || !e && -1 !== t.type.indexOf("mouse") ? "" : {
                 dragging: !0,
                 touchObject: {
                     startX: t.touches ? t.touches[0].pageX : t.clientX,
                     startY: t.touches ? t.touches[0].pageY : t.clientY,
                     curX: t.touches ? t.touches[0].pageX : t.clientX,
                     curY: t.touches ? t.touches[0].pageY : t.clientY
@@ -117936,29 +118078,29 @@
                     m = e.slidesToScroll,
                     g = e.infinite,
                     b = e.touchObject,
                     v = e.swipeEvent,
                     y = e.listHeight,
                     x = e.listWidth;
                 if (!n) {
-                    if (a) return es(t);
-                    r && o && i && es(t);
-                    n = {}, a = Ss(e), o = (b.curX = t.touches ? t.touches[0].pageX : t.clientX, b.curY = t.touches ? t.touches[0].pageY : t.clientY, b.swipeLength = Math.round(Math.sqrt(Math.pow(b.curX - b.startX, 2))), Math.round(Math.sqrt(Math.pow(b.curY - b.startY, 2))));
+                    if (a) return ls(t);
+                    r && o && i && ls(t);
+                    n = {}, a = As(e), o = (b.curX = t.touches ? t.touches[0].pageX : t.clientX, b.curY = t.touches ? t.touches[0].pageY : t.clientY, b.swipeLength = Math.round(Math.sqrt(Math.pow(b.curX - b.startX, 2))), Math.round(Math.sqrt(Math.pow(b.curY - b.startY, 2))));
                     if (!i && !f && 10 < o) return {
                         scrolling: !0
                     };
                     i && (b.swipeLength = o);
-                    f = (l ? -1 : 1) * (b.curX > b.startX ? 1 : -1), o = (i && (f = b.curY > b.startY ? 1 : -1), Math.ceil(h / m)), h = ns(e.touchObject, i), m = b.swipeLength;
-                    return g || (0 === c && ("right" === h || "down" === h) || o <= c + 1 && ("left" === h || "up" === h) || !js(e) && ("left" === h || "up" === h)) && (m = b.swipeLength * s, !1 === u) && d && (d(h), n.edgeDragged = !0), !p && v && (v(h), n.swiped = !0), g = i ? a + m * f : r ? a + m * (y / x) * f : l ? a - m * f : a + m * f, n = Object(Ct.a)(Object(Ct.a)({}, n), {}, {
+                    f = (l ? -1 : 1) * (b.curX > b.startX ? 1 : -1), o = (i && (f = b.curY > b.startY ? 1 : -1), Math.ceil(h / m)), h = cs(e.touchObject, i), m = b.swipeLength;
+                    return g || (0 === c && ("right" === h || "down" === h) || o <= c + 1 && ("left" === h || "up" === h) || !Ps(e) && ("left" === h || "up" === h)) && (m = b.swipeLength * s, !1 === u) && d && (d(h), n.edgeDragged = !0), !p && v && (v(h), n.swiped = !0), g = i ? a + m * f : r ? a + m * (y / x) * f : l ? a - m * f : a + m * f, n = Object(Ct.a)(Object(Ct.a)({}, n), {}, {
                         touchObject: b,
                         swipeLeft: g,
-                        trackStyle: Es(Object(Ct.a)(Object(Ct.a)({}, e), {}, {
+                        trackStyle: Ts(Object(Ct.a)(Object(Ct.a)({}, e), {}, {
                             left: g
                         }))
-                    }), Math.abs(b.curX - b.startX) < .8 * Math.abs(b.curY - b.startY) || 10 < b.swipeLength && (n.swiping = !0, es(t)), n
+                    }), Math.abs(b.curX - b.startX) < .8 * Math.abs(b.curY - b.startY) || 10 < b.swipeLength && (n.swiping = !0, ls(t)), n
                 }
             }(t, Object(Ct.a)(Object(Ct.a)(Object(Ct.a)({}, f.props), f.state), {}, {
                 trackRef: f.track,
                 listRef: f.list,
                 slideIndex: f.state.currentSlide
             }));
             t && (t.swiping && (f.clickable = !1), f.setState(t))
@@ -117973,46 +118115,46 @@
                     c = e.listHeight,
                     s = e.swipeToSlide,
                     u = e.scrolling,
                     d = e.onSwipe,
                     p = e.targetSlide,
                     f = e.currentSlide,
                     h = e.infinite;
-                if (!n) return a && es(t), {};
+                if (!n) return a && ls(t), {};
                 var n = l ? c / i : o / i,
-                    a = ns(r, l),
+                    a = cs(r, l),
                     m = {
                         dragging: !1,
                         edgeDragged: !1,
                         scrolling: !1,
                         swiping: !1,
                         swiped: !1,
                         swipeLeft: null,
                         touchObject: {}
                     };
                 if (!u && r.swipeLength)
                     if (r.swipeLength > n) {
-                        es(t), d && d(a);
+                        ls(t), d && d(a);
                         var g, b, v = h ? f : p;
                         switch (a) {
                             case "left":
                             case "up":
-                                b = v + os(e), g = s ? rs(e, b) : b, m.currentDirection = 0;
+                                b = v + ds(e), g = s ? us(e, b) : b, m.currentDirection = 0;
                                 break;
                             case "right":
                             case "down":
-                                b = v - os(e), g = s ? rs(e, b) : b, m.currentDirection = 1;
+                                b = v - ds(e), g = s ? us(e, b) : b, m.currentDirection = 1;
                                 break;
                             default:
                                 g = v
                         }
                         m.triggerSlideHandler = g
                     } else {
-                        c = Ss(e);
-                        m.trackStyle = Cs(Object(Ct.a)(Object(Ct.a)({}, e), {}, {
+                        c = As(e);
+                        m.trackStyle = zs(Object(Ct.a)(Object(Ct.a)({}, e), {}, {
                             left: c
                         }))
                     } return m
             }(t, Object(Ct.a)(Object(Ct.a)(Object(Ct.a)({}, f.props), f.state), {}, {
                 trackRef: f.track,
                 listRef: f.list,
                 slideIndex: f.state.currentSlide
@@ -118042,15 +118184,15 @@
                     currentSlide: f.state.currentSlide
                 }, e)
             }, 0))
         }), Object(Vt.a)(Object(s.a)(f), "play", function() {
             var t;
             if (f.props.rtl) t = f.state.currentSlide - f.props.slidesToScroll;
             else {
-                if (!js(Object(Ct.a)(Object(Ct.a)({}, f.props), f.state))) return !1;
+                if (!Ps(Object(Ct.a)(Object(Ct.a)({}, f.props), f.state))) return !1;
                 t = f.state.currentSlide + f.props.slidesToScroll
             }
             f.slideHandler(t)
         }), Object(Vt.a)(Object(s.a)(f), "autoPlay", function(t) {
             f.autoplayTimer && clearInterval(f.autoplayTimer);
             var e = f.state.autoplaying;
             if ("update" === t) {
@@ -118085,29 +118227,29 @@
             return f.props.autoplay && "focused" === f.state.autoplaying && f.autoPlay("blur")
         }), Object(Vt.a)(Object(s.a)(f), "render", function() {
             var t, e, n, a = Kt()("slick-slider", f.props.className, {
                     "slick-vertical": f.props.vertical,
                     "slick-initialized": !0
                 }),
                 r = Object(Ct.a)(Object(Ct.a)({}, f.props), f.state),
-                o = as(r, ["fade", "cssEase", "speed", "infinite", "centerMode", "focusOnSelect", "currentSlide", "lazyLoad", "lazyLoadedList", "rtl", "slideWidth", "slideHeight", "listHeight", "vertical", "slidesToShow", "slidesToScroll", "slideCount", "trackStyle", "variableWidth", "unslick", "centerPadding", "targetSlide", "useCSS"]),
+                o = ss(r, ["fade", "cssEase", "speed", "infinite", "centerMode", "focusOnSelect", "currentSlide", "lazyLoad", "lazyLoadedList", "rtl", "slideWidth", "slideHeight", "listHeight", "vertical", "slidesToShow", "slidesToScroll", "slideCount", "trackStyle", "variableWidth", "unslick", "centerPadding", "targetSlide", "useCSS"]),
                 i = f.props.pauseOnHover,
                 o = Object(Ct.a)(Object(Ct.a)({}, o), {}, {
                     onMouseEnter: i ? f.onTrackOver : null,
                     onMouseLeave: i ? f.onTrackLeave : null,
                     onMouseOver: i ? f.onTrackOver : null,
                     focusOnSelect: f.props.focusOnSelect && f.clickable ? f.selectHandler : null
                 }),
-                i = (!0 === f.props.dots && f.state.slideCount >= f.props.slidesToShow && (i = as(r, ["dotsClass", "slideCount", "slidesToShow", "currentSlide", "slidesToScroll", "clickHandler", "children", "customPaging", "infinite", "appendDots"]), n = f.props.pauseOnDotsHover, i = Object(Ct.a)(Object(Ct.a)({}, i), {}, {
+                i = (!0 === f.props.dots && f.state.slideCount >= f.props.slidesToShow && (i = ss(r, ["dotsClass", "slideCount", "slidesToShow", "currentSlide", "slidesToScroll", "clickHandler", "children", "customPaging", "infinite", "appendDots"]), n = f.props.pauseOnDotsHover, i = Object(Ct.a)(Object(Ct.a)({}, i), {}, {
                     clickHandler: f.changeSlide,
                     onMouseEnter: n ? f.onDotsLeave : null,
                     onMouseOver: n ? f.onDotsOver : null,
                     onMouseLeave: n ? f.onDotsLeave : null
-                }), n = H.a.createElement(zs, i)), as(r, ["infinite", "centerMode", "currentSlide", "slideCount", "slidesToShow", "prevArrow", "nextArrow"])),
-                r = (i.clickHandler = f.changeSlide, f.props.arrows && (t = H.a.createElement(As, i), e = H.a.createElement(Rs, i)), null),
+                }), n = H.a.createElement(Bs, i)), ss(r, ["infinite", "centerMode", "currentSlide", "slideCount", "slidesToShow", "prevArrow", "nextArrow"])),
+                r = (i.clickHandler = f.changeSlide, f.props.arrows && (t = H.a.createElement(Fs, i), e = H.a.createElement(Hs, i)), null),
                 i = (f.props.vertical && (r = {
                     height: f.state.listHeight
                 }), null),
                 r = (!1 === f.props.vertical ? !0 === f.props.centerMode && (i = {
                     padding: "0px " + f.props.centerPadding
                 }) : !0 === f.props.centerMode && (i = {
                     padding: f.props.centerPadding + " 0px"
@@ -118134,46 +118276,46 @@
                 };
             return f.props.unslick && (r = {
                 className: "slick-list"
             }, i = {
                 className: a
             }), H.a.createElement("div", i, f.props.unslick ? "" : t, H.a.createElement("div", Object(Et.a)({
                 ref: f.listRefHandler
-            }, r), H.a.createElement(Ts, Object(Et.a)({
+            }, r), H.a.createElement(Ys, Object(Et.a)({
                 ref: f.trackRefHandler
             }, o), f.props.children)), f.props.unslick ? "" : e, f.props.unslick ? "" : n)
-        }), f.list = null, f.track = null, f.state = Object(Ct.a)(Object(Ct.a)({}, Jc), {}, {
+        }), f.list = null, f.track = null, f.state = Object(Ct.a)(Object(Ct.a)({}, rs), {}, {
             currentSlide: f.props.initialSlide,
             slideCount: H.a.Children.count(f.props.children)
         }), f.callbackTimers = [], f.clickable = !0, f.debouncedResize = null;
         var f, t = f.ssrInit();
         return f.state = Object(Ct.a)(Object(Ct.a)({}, f.state), t), f
     }
 
-    function Us() {
-        return Object(i.a)(this, Us), hs.apply(this, arguments)
+    function Js() {
+        return Object(i.a)(this, Js), xs.apply(this, arguments)
     }
 
-    function Gs() {
-        return Object(i.a)(this, Gs), ms.apply(this, arguments)
+    function Qs() {
+        return Object(i.a)(this, Qs), _s.apply(this, arguments)
     }
 
-    function qs() {
-        return Object(i.a)(this, qs), gs.apply(this, arguments)
+    function tu() {
+        return Object(i.a)(this, tu), Os.apply(this, arguments)
     }
 
-    function Xs() {
+    function eu() {
         var e;
-        Object(i.a)(this, Xs);
+        Object(i.a)(this, eu);
         for (var t = arguments.length, n = new Array(t), a = 0; a < t; a++) n[a] = arguments[a];
-        return e = bs.call.apply(bs, [this].concat(n)), Object(Vt.a)(Object(s.a)(e), "node", null), Object(Vt.a)(Object(s.a)(e), "handleRef", function(t) {
+        return e = ws.call.apply(ws, [this].concat(n)), Object(Vt.a)(Object(s.a)(e), "node", null), Object(Vt.a)(Object(s.a)(e), "handleRef", function(t) {
             e.node = t
         }), e
     }
-    ds.propTypes = {
+    bs.propTypes = {
         id: n.a.string,
         children: n.a.node,
         className: n.a.oneOfType([n.a.string, n.a.object]),
         style: n.a.object,
         key: n.a.string,
         autoplay: n.a.bool,
         dotPosition: n.a.oneOf(["top", "bottom", "left", "right"]),
@@ -118184,25 +118326,25 @@
         pauseOnHover: n.a.bool,
         loading_state: n.a.shape({
             is_loading: n.a.bool,
             prop_name: n.a.string,
             component_name: n.a.string
         }),
         setProps: n.a.func
-    }, ds.defaultProps = {
+    }, bs.defaultProps = {
         autoplay: !1,
         dotPosition: "bottom",
         easing: "linear",
         effect: "scrollx",
         autoplaySpeed: 3e3,
         speed: 500,
         pauseOnHover: !1
     };
 
-    function $s(t) {
+    function nu(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.labelCol,
             l = t.colon,
@@ -118212,15 +118354,15 @@
             d = t.tooltip,
             p = t.extra,
             f = t.help,
             h = t.hidden,
             m = t.required,
             g = t.validateStatus,
             t = (t.setProps, t.loading_state);
-        return H.a.createElement(eu.a.Item, {
+        return H.a.createElement(lu.a.Item, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             labelCol: i,
             colon: l,
             wrapperCol: c,
@@ -118233,41 +118375,41 @@
             hidden: h,
             required: m,
             validateStatus: g,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
 
-    function Zs(t) {
+    function au(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.labelCol,
             l = t.wrapperCol,
             c = t.colon,
             s = t.labelAlign,
             u = t.layout,
             t = (t.setProps, t.loading_state);
-        return H.a.createElement(eu.a, {
+        return H.a.createElement(lu.a, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             labelCol: i,
             wrapperCol: l,
             colon: c,
             labelAlign: s,
             layout: u,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
 
-    function Js(t) {
+    function ru(t) {
         var e = t.prefixCls,
             n = t.className,
             a = t.hoverable,
             r = void 0 === a || a,
             o = function(t, e) {
                 var n = {};
                 for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
@@ -118279,35 +118421,35 @@
             t = (0, t.getPrefixCls)("card", e), t = Kt()("".concat(t, "-grid"), n, Object(Vt.a)({}, "".concat(t, "-grid-hoverable"), r));
             return Wt.createElement("div", Object(Et.a)({}, o, {
                 className: t
             }))
         })
     }
 
-    function Qs(t) {
+    function ou(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.hoverable,
             t = (t.setProps, t.loading_state),
             n = j(n);
-        return H.a.createElement(ru.Grid, {
+        return H.a.createElement(uu.Grid, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             hoverable: i,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
-    var tu = ds,
-        eu = e(311),
-        nu = ($s.propTypes = {
+    var iu = bs,
+        lu = e(311),
+        cu = (nu.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             required: n.a.bool,
             labelCol: n.a.exact({
@@ -118328,21 +118470,21 @@
             hidden: n.a.bool,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, $s.defaultProps = {
+        }, nu.defaultProps = {
             labelAlign: "right",
             required: !1,
             colon: !0,
             hidden: !1
-        }, $s),
-        au = (Zs.propTypes = {
+        }, nu),
+        su = (au.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             layout: n.a.oneOf(["horizontal", "vertical", "inline"]),
             labelCol: n.a.exact({
@@ -118357,24 +118499,24 @@
             labelAlign: n.a.oneOf(["left", "right"]),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, Zs.defaultProps = {
+        }, au.defaultProps = {
             layout: "horizontal",
             colon: !0,
             labelAlign: "right"
-        }, Zs),
+        }, au),
         l = Wt.forwardRef(function(n, t) {
             var e, a = Wt.useContext(q.b),
                 r = a.getPrefixCls,
                 a = a.direction,
-                o = Wt.useContext(fi.b),
+                o = Wt.useContext(gi.b),
                 i = n.prefixCls,
                 l = n.className,
                 c = n.extra,
                 s = n.headStyle,
                 s = void 0 === s ? {} : s,
                 u = n.bodyStyle,
                 u = void 0 === u ? {} : u,
@@ -118398,25 +118540,25 @@
                     var n = {};
                     for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
                     if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                         for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
                     return n
                 }(n, ["prefixCls", "className", "extra", "headStyle", "bodyStyle", "title", "loading", "bordered", "size", "type", "cover", "actions", "tabList", "children", "activeTabKey", "defaultActiveTabKey", "tabBarExtraContent", "hoverable", "tabProps"]),
                 r = r("card", i),
-                i = Wt.createElement(Dl, {
+                i = Wt.createElement(Al, {
                     loading: !0,
                     active: !0,
                     paragraph: {
                         rows: 4
                     },
                     title: !1
                 }, y),
                 M = void 0 !== x,
                 M = Object(Et.a)(Object(Et.a)({}, k), (k = {}, Object(Vt.a)(k, M ? "activeKey" : "defaultActiveKey", M ? x : _), Object(Vt.a)(k, "tabBarExtraContent", O), k)),
-                x = v && v.length ? Wt.createElement(Do.a, Object(Et.a)({
+                x = v && v.length ? Wt.createElement(Ao.a, Object(Et.a)({
                     size: "large"
                 }, M, {
                     className: "".concat(r, "-head-tabs"),
                     onChange: function(t) {
                         var e;
                         null != (e = n.onTabChange) && e.call(n, t)
                     },
@@ -118451,26 +118593,26 @@
                     return Wt.createElement("li", {
                         style: {
                             width: "".concat(100 / C.length, "%")
                         },
                         key: "action-".concat(e)
                     }, Wt.createElement("span", null, t))
                 })) : null,
-                M = Object(ct.a)(j, ["onTabChange"]),
+                M = Object(pt.a)(j, ["onTabChange"]),
                 s = h || o,
                 c = Kt()(r, (d = {}, Object(Vt.a)(d, "".concat(r, "-loading"), p), Object(Vt.a)(d, "".concat(r, "-bordered"), f), Object(Vt.a)(d, "".concat(r, "-hoverable"), w), Object(Vt.a)(d, "".concat(r, "-contain-grid"), (Wt.Children.forEach(n.children, function(t) {
-                    t && t.type && t.type === Js && (E = !0)
+                    t && t.type && t.type === ru && (E = !0)
                 }), E)), Object(Vt.a)(d, "".concat(r, "-contain-tabs"), v && v.length), Object(Vt.a)(d, "".concat(r, "-").concat(s), s), Object(Vt.a)(d, "".concat(r, "-type-").concat(m), !!m), Object(Vt.a)(d, "".concat(r, "-rtl"), "rtl" === a), d), l);
             return Wt.createElement("div", Object(Et.a)({
                 ref: t
             }, M, {
                 className: c
             }), e, _, O, k)
         }),
-        ru = (l.Grid = Js, l.Meta = function(l) {
+        uu = (l.Grid = ru, l.Meta = function(l) {
             return Wt.createElement(q.a, null, function(t) {
                 var t = t.getPrefixCls,
                     e = l.prefixCls,
                     n = l.className,
                     a = l.avatar,
                     r = l.title,
                     o = l.description,
@@ -118496,75 +118638,75 @@
                         className: "".concat(t, "-meta-detail")
                     }, a, r) : null;
                 return Wt.createElement("div", Object(Et.a)({}, i, {
                     className: e
                 }), n, o)
             })
         }, l),
-        ou = (Qs.propTypes = {
+        du = (ou.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             hoverable: n.a.bool,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, Qs.defaultProps = {
+        }, ou.defaultProps = {
             hoverable: !0
-        }, Qs);
+        }, ou);
 
-    function iu(t) {
-        return (iu = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
+    function pu(t) {
+        return (pu = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
             return typeof t
         } : function(t) {
             return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
         })(t)
     }
 
-    function lu(e, t) {
+    function fu(e, t) {
         var n, a = Object.keys(e);
         return Object.getOwnPropertySymbols && (n = Object.getOwnPropertySymbols(e), t && (n = n.filter(function(t) {
             return Object.getOwnPropertyDescriptor(e, t).enumerable
         })), a.push.apply(a, n)), a
     }
 
-    function cu(a) {
+    function hu(a) {
         for (var t = 1; t < arguments.length; t++) {
             var r = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? lu(Object(r), !0).forEach(function(t) {
+            t % 2 ? fu(Object(r), !0).forEach(function(t) {
                 var e, n;
                 e = a, t = r[n = t], (n = function() {
                     var t = function(t) {
-                        if ("object" !== iu(t) || null === t) return t;
+                        if ("object" !== pu(t) || null === t) return t;
                         var e = t[Symbol.toPrimitive];
                         if (void 0 === e) return String(t);
                         e = e.call(t, "string");
-                        if ("object" !== iu(e)) return e;
+                        if ("object" !== pu(e)) return e;
                         throw new TypeError("@@toPrimitive must return a primitive value.")
                     }(n);
-                    return "symbol" === iu(t) ? t : String(t)
+                    return "symbol" === pu(t) ? t : String(t)
                 }()) in e ? Object.defineProperty(e, n, {
                     value: t,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : e[n] = t
-            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(r)) : lu(Object(r)).forEach(function(t) {
+            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(r)) : fu(Object(r)).forEach(function(t) {
                 Object.defineProperty(a, t, Object.getOwnPropertyDescriptor(r, t))
             })
         }
         return a
     }
 
-    function su(t) {
+    function mu(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.extraLink,
             l = t.coverImg,
@@ -118572,20 +118714,20 @@
             s = t.headStyle,
             u = t.bordered,
             d = t.hoverable,
             p = t.size,
             f = t.title,
             t = (t.setProps, t.loading_state),
             n = j(n);
-        return H.a.createElement(ru, {
+        return H.a.createElement(uu, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
-            bodyStyle: cu({
+            bodyStyle: hu({
                 display: "flex",
                 flexWrap: "wrap"
             }, c),
             headStyle: s,
             extra: H.a.createElement("a", {
                 className: i && i.className,
                 style: i && i.style,
@@ -118601,15 +118743,15 @@
             bordered: u,
             hoverable: d,
             size: p,
             title: f,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
-    su.propTypes = {
+    mu.propTypes = {
         id: n.a.string,
         children: n.a.node,
         className: n.a.oneOfType([n.a.string, n.a.object]),
         style: n.a.object,
         key: n.a.string,
         title: n.a.node,
         extraLink: n.a.exact({
@@ -118632,30 +118774,30 @@
         size: n.a.oneOf(["default", "small"]),
         loading_state: n.a.shape({
             is_loading: n.a.bool,
             prop_name: n.a.string,
             component_name: n.a.string
         }),
         setProps: n.a.func
-    }, su.defaultProps = {
+    }, mu.defaultProps = {
         bordered: !0,
         hoverable: !1,
         size: "default"
     };
-    var uu = su,
-        du = e(480),
-        pu = e(695);
+    var gu = mu,
+        bu = e(480),
+        vu = e(695);
 
-    function fu(t, e) {
+    function yu(t, e) {
         (null == e || e > t.length) && (e = t.length);
         for (var n = 0, a = new Array(e); n < e; n++) a[n] = t[n];
         return a
     }
 
-    function hu(t) {
+    function xu(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.locale,
             i = t.width,
             l = t.height,
@@ -118689,22 +118831,22 @@
                             if (s) throw r
                         }
                     }
                     return l
                 }
             }(t, p) || function(t, e) {
                 var n;
-                if (t) return "string" == typeof t ? fu(t, e) : "Map" === (n = "Object" === (n = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : n) || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? fu(t, e) : void 0
+                if (t) return "string" == typeof t ? yu(t, e) : "Map" === (n = "Object" === (n = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : n) || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? yu(t, e) : void 0
             }(t, p) || function() {
                 throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
             }())[0],
             f = t[1];
         return Array.isArray(c) ? "fold" === u ? H.a.createElement(W.a, {
             locale: K.b.get(o)
-        }, H.a.createElement(pu.a, {
+        }, H.a.createElement(vu.a, {
             id: e,
             style: a,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             key: r,
             preview: {
                 visible: !1
             },
@@ -118715,60 +118857,60 @@
             onClick: function() {
                 return f(!0)
             }
         }), H.a.createElement("div", {
             style: {
                 display: "none"
             }
-        }, H.a.createElement(pu.a.PreviewGroup, {
+        }, H.a.createElement(vu.a.PreviewGroup, {
             preview: {
                 visible: p,
                 onVisibleChange: function(t) {
                     return f(t)
                 }
             }
         }, c.map(function(t) {
-            return H.a.createElement(pu.a, {
+            return H.a.createElement(vu.a, {
                 src: t,
                 fallback: s
             })
         })))) : H.a.createElement(W.a, {
             locale: K.b.get(o)
-        }, H.a.createElement(pu.a.PreviewGroup, {
+        }, H.a.createElement(vu.a.PreviewGroup, {
             id: e,
             style: a,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             key: r
         }, c.map(function(t) {
-            return H.a.createElement(pu.a, {
+            return H.a.createElement(vu.a, {
                 src: t,
                 fallback: s,
                 width: i,
                 height: l
             })
         }))) : H.a.createElement(W.a, {
             locale: K.b.get(o)
-        }, H.a.createElement(pu.a, {
+        }, H.a.createElement(vu.a, {
             id: e,
             style: a,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             key: r,
             width: i,
             height: l,
             src: c,
             fallback: s,
             preview: d
         }))
     }
 
-    function mu(d) {
+    function _u(d) {
         function p(t) {
             t = t.width, e(t < 768, !0)
         }
-        var t = Object(xu.a)(!1),
+        var t = Object(Mu.a)(!1),
             f = (t = Object(Gt.a)(t, 2))[0],
             e = t[1];
         return Wt.createElement(q.a, null, function(t) {
             var e = t.getPrefixCls,
                 n = t.pageHeader,
                 t = t.direction,
                 a = d.prefixCls,
@@ -118776,76 +118918,76 @@
                 o = d.footer,
                 i = d.children,
                 l = d.breadcrumb,
                 c = d.breadcrumbRender,
                 s = d.className,
                 u = !0,
                 n = ("ghost" in d ? u = d.ghost : n && "ghost" in n && (u = n.ghost), e("page-header", a)),
-                a = null != l && l.routes ? (e = l, Wt.createElement($l, Object(Et.a)({}, e))) : null,
+                a = null != l && l.routes ? (e = l, Wt.createElement(Xl, Object(Et.a)({}, e))) : null,
                 e = l && "props" in l,
                 c = null != (c = null == c ? void 0 : c(d, a)) ? c : a,
                 a = e ? l : c,
                 l = Kt()(n, s, (e = {
                     "has-breadcrumb": !!a,
                     "has-footer": !!o
                 }, Object(Vt.a)(e, "".concat(n, "-ghost"), u), Object(Vt.a)(e, "".concat(n, "-rtl"), "rtl" === t), Object(Vt.a)(e, "".concat(n, "-compact"), f), e));
-            return Wt.createElement(lt.a, {
+            return Wt.createElement(dt.a, {
                 onResize: p
             }, Wt.createElement("div", {
                 className: l,
                 style: r
             }, a, function(t, e, n) {
                 var n = 2 < arguments.length && void 0 !== n ? n : "ltr",
                     a = e.title,
                     r = e.avatar,
                     o = e.subTitle,
                     i = e.tags,
                     l = e.extra,
                     c = e.onBack,
                     s = "".concat(t, "-heading"),
                     u = a || o || i || l;
-                return u ? (e = Ou(e, n), n = _u(t, e, c), Wt.createElement("div", {
+                return u ? (e = Cu(e, n), n = Eu(t, e, c), Wt.createElement("div", {
                     className: s
                 }, (n || r || u) && Wt.createElement("div", {
                     className: "".concat(s, "-left")
-                }, n, r && Wt.createElement(Bc.a, Object(Et.a)({}, r)), a && Wt.createElement("span", {
+                }, n, r && Wt.createElement(Uc.a, Object(Et.a)({}, r)), a && Wt.createElement("span", {
                     className: "".concat(s, "-title"),
                     title: "string" == typeof a ? a : void 0
                 }, a), o && Wt.createElement("span", {
                     className: "".concat(s, "-sub-title"),
                     title: "string" == typeof o ? o : void 0
                 }, o), i && Wt.createElement("span", {
                     className: "".concat(s, "-tags")
                 }, i)), l && Wt.createElement("span", {
                     className: "".concat(s, "-extra")
-                }, Wt.createElement(za.b, null, l)))) : null
+                }, Wt.createElement(Ia.b, null, l)))) : null
             }(n, d, t), i && (c = i, Wt.createElement("div", {
                 className: "".concat(n, "-content")
             }, c)), (s = o) ? Wt.createElement("div", {
                 className: "".concat(n, "-footer")
             }, s) : null))
         })
     }
 
-    function gu(t) {
+    function Ou(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.title,
             l = t.subTitle,
             c = t.showBackIcon,
             s = t.historyBackDisabled,
             u = t.backClicks,
             d = t.ghost,
             p = t.setProps,
             t = t.loading_state,
             n = j(n);
-        return H.a.createElement(mu, {
+        return H.a.createElement(_u, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             title: i,
             subTitle: l,
             backIcon: !!c && void 0,
@@ -118856,15 +118998,15 @@
                 })
             } : function() {
                 return window.history.back()
             },
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
-    hu.propTypes = {
+    xu.propTypes = {
         id: n.a.string,
         className: n.a.oneOfType([n.a.string, n.a.object]),
         style: n.a.object,
         key: n.a.string,
         locale: n.a.oneOf(["zh-cn", "en-us"]),
         alt: n.a.string,
         width: n.a.oneOfType([n.a.number, n.a.string]),
@@ -118875,43 +119017,43 @@
         preview: n.a.bool,
         loading_state: n.a.shape({
             is_loading: n.a.bool,
             prop_name: n.a.string,
             component_name: n.a.string
         }),
         setProps: n.a.func
-    }, hu.defaultProps = {
+    }, xu.defaultProps = {
         preview: !0,
         multiImageMode: "fold",
         locale: "zh-cn",
         fallback: "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAMIAAADDCAYAAADQvc6UAAABRWlDQ1BJQ0MgUHJvZmlsZQAAKJFjYGASSSwoyGFhYGDIzSspCnJ3UoiIjFJgf8LAwSDCIMogwMCcmFxc4BgQ4ANUwgCjUcG3awyMIPqyLsis7PPOq3QdDFcvjV3jOD1boQVTPQrgSkktTgbSf4A4LbmgqISBgTEFyFYuLykAsTuAbJEioKOA7DkgdjqEvQHEToKwj4DVhAQ5A9k3gGyB5IxEoBmML4BsnSQk8XQkNtReEOBxcfXxUQg1Mjc0dyHgXNJBSWpFCYh2zi+oLMpMzyhRcASGUqqCZ16yno6CkYGRAQMDKMwhqj/fAIcloxgHQqxAjIHBEugw5sUIsSQpBobtQPdLciLEVJYzMPBHMDBsayhILEqEO4DxG0txmrERhM29nYGBddr//5/DGRjYNRkY/l7////39v///y4Dmn+LgeHANwDrkl1AuO+pmgAAADhlWElmTU0AKgAAAAgAAYdpAAQAAAABAAAAGgAAAAAAAqACAAQAAAABAAAAwqADAAQAAAABAAAAwwAAAAD9b/HnAAAHlklEQVR4Ae3dP3PTWBSGcbGzM6GCKqlIBRV0dHRJFarQ0eUT8LH4BnRU0NHR0UEFVdIlFRV7TzRksomPY8uykTk/zewQfKw/9znv4yvJynLv4uLiV2dBoDiBf4qP3/ARuCRABEFAoBEgghggQAQZQKAnYEaQBAQaASKIAQJEkAEEegJmBElAoBEgghggQAQZQKAnYEaQBAQaASKIAQJEkAEEegJmBElAoBEgghggQAQZQKAnYEaQBAQaASKIAQJEkAEEegJmBElAoBEgghggQAQZQKAnYEaQBAQaASKIAQJEkAEEegJmBElAoBEgghggQAQZQKAnYEaQBAQaASKIAQJEkAEEegJmBElAoBEgghggQAQZQKAnYEaQBAQaASKIAQJEkAEEegJmBElAoBEgghggQAQZQKAnYEaQBAQaASKIAQJEkAEEegJmBElAoBEgghggQAQZQKAnYEaQBAQaASKIAQJEkAEEegJmBElAoBEgghggQAQZQKAnYEaQBAQaASKIAQJEkAEEegJmBElAoBEgghggQAQZQKAnYEaQBAQaASKIAQJEkAEEegJmBElAoBEgghggQAQZQKAnYEaQBAQaASKIAQJEkAEEegJmBElAoBEgghggQAQZQKAnYEaQBAQaASKIAQJEkAEEegJmBElAoBEgghgg0Aj8i0JO4OzsrPv69Wv+hi2qPHr0qNvf39+iI97soRIh4f3z58/u7du3SXX7Xt7Z2enevHmzfQe+oSN2apSAPj09TSrb+XKI/f379+08+A0cNRE2ANkupk+ACNPvkSPcAAEibACyXUyfABGm3yNHuAECRNgAZLuYPgEirKlHu7u7XdyytGwHAd8jjNyng4OD7vnz51dbPT8/7z58+NB9+/bt6jU/TI+AGWHEnrx48eJ/EsSmHzx40L18+fLyzxF3ZVMjEyDCiEDjMYZZS5wiPXnyZFbJaxMhQIQRGzHvWR7XCyOCXsOmiDAi1HmPMMQjDpbpEiDCiL358eNHurW/5SnWdIBbXiDCiA38/Pnzrce2YyZ4//59F3ePLNMl4PbpiL2J0L979+7yDtHDhw8vtzzvdGnEXdvUigSIsCLAWavHp/+qM0BcXMd/q25n1vF57TYBp0a3mUzilePj4+7k5KSLb6gt6ydAhPUzXnoPR0dHl79WGTNCfBnn1uvSCJdegQhLI1vvCk+fPu2ePXt2tZOYEV6/fn31dz+shwAR1sP1cqvLntbEN9MxA9xcYjsxS1jWR4AIa2Ibzx0tc44fYX/16lV6NDFLXH+YL32jwiACRBiEbf5KcXoTIsQSpzXx4N28Ja4BQoK7rgXiydbHjx/P25TaQAJEGAguWy0+2Q8PD6/Ki4R8EVl+bzBOnZY95fq9rj9zAkTI2SxdidBHqG9+skdw43borCXO/ZcJdraPWdv22uIEiLA4q7nvvCug8WTqzQveOH26fodo7g6uFe/a17W3+nFBAkRYENRdb1vkkz1CH9cPsVy/jrhr27PqMYvENYNlHAIesRiBYwRy0V+8iXP8+/fvX11Mr7L7ECueb/r48eMqm7FuI2BGWDEG8cm+7G3NEOfmdcTQw4h9/55lhm7DekRYKQPZF2ArbXTAyu4kDYB2YxUzwg0gi/41ztHnfQG26HbGel/crVrm7tNY+/1btkOEAZ2M05r4FB7r9GbAIdxaZYrHdOsgJ/wCEQY0J74TmOKnbxxT9n3FgGGWWsVdowHtjt9Nnvf7yQM2aZU/TIAIAxrw6dOnAWtZZcoEnBpNuTuObWMEiLAx1HY0ZQJEmHJ3HNvGCBBhY6jtaMoEiJB0Z29vL6ls58vxPcO8/zfrdo5qvKO+d3Fx8Wu8zf1dW4p/cPzLly/dtv9Ts/EbcvGAHhHyfBIhZ6NSiIBTo0LNNtScABFyNiqFCBChULMNNSdAhJyNSiECRCjUbEPNCRAhZ6NSiAARCjXbUHMCRMjZqBQiQIRCzTbUnAARcjYqhQgQoVCzDTUnQIScjUohAkQo1GxDzQkQIWejUogAEQo121BzAkTI2agUIkCEQs021JwAEXI2KoUIEKFQsw01J0CEnI1KIQJEKNRsQ80JECFno1KIABEKNdtQcwJEyNmoFCJAhELNNtScABFyNiqFCBChULMNNSdAhJyNSiECRCjUbEPNCRAhZ6NSiAARCjXbUHMCRMjZqBQiQIRCzTbUnAARcjYqhQgQoVCzDTUnQIScjUohAkQo1GxDzQkQIWejUogAEQo121BzAkTI2agUIkCEQs021JwAEXI2KoUIEKFQsw01J0CEnI1KIQJEKNRsQ80JECFno1KIABEKNdtQcwJEyNmoFCJAhELNNtScABFyNiqFCBChULMNNSdAhJyNSiECRCjUbEPNCRAhZ6NSiAARCjXbUHMCRMjZqBQiQIRCzTbUnAARcjYqhQgQoVCzDTUnQIScjUohAkQo1GxDzQkQIWejUogAEQo121BzAkTI2agUIkCEQs021JwAEXI2KoUIEKFQsw01J0CEnI1KIQJEKNRsQ80JECFno1KIABEKNdtQcwJEyNmoFCJAhELNNtScABFyNiqFCBChULMNNSdAhJyNSiEC/wGgKKC4YMA4TAAAAABJRU5ErkJggg=="
     };
-    var bu = hu,
-        vu = e(527),
-        yu = e(528),
-        xu = e(82),
-        _u = function(e, n, a) {
-            return n && a ? Wt.createElement(ye.a, {
+    var wu = xu,
+        ku = e(527),
+        ju = e(528),
+        Mu = e(82),
+        Eu = function(e, n, a) {
+            return n && a ? Wt.createElement(we.a, {
                 componentName: "PageHeader"
             }, function(t) {
                 return Wt.createElement("div", {
                     className: "".concat(e, "-back")
-                }, Wt.createElement(Ce.a, {
+                }, Wt.createElement(Pe.a, {
                     onClick: function(t) {
                         null != a && a(t)
                     },
                     className: "".concat(e, "-back-button"),
                     "aria-label": t.back
                 }, n))
             }) : null
         },
-        Ou = function(t) {
-            return void 0 !== t.backIcon ? t.backIcon : "rtl" === (1 < arguments.length && void 0 !== arguments[1] ? arguments[1] : "ltr") ? Wt.createElement(yu.a, null) : Wt.createElement(vu.a, null)
+        Cu = function(t) {
+            return void 0 !== t.backIcon ? t.backIcon : "rtl" === (1 < arguments.length && void 0 !== arguments[1] ? arguments[1] : "ltr") ? Wt.createElement(ju.a, null) : Wt.createElement(ku.a, null)
         },
-        wu = (gu.propTypes = {
+        Su = (Ou.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             title: n.a.node,
             subTitle: n.a.node,
@@ -118921,25 +119063,25 @@
             ghost: n.a.bool,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, gu.defaultProps = {
+        }, Ou.defaultProps = {
             backClicks: 0,
             showBackIcon: !0,
             historyBackDisabled: !1
-        }, gu),
+        }, Ou),
         c = e(250),
-        ku = e(186),
-        ju = e(302),
-        Mu = e(301);
+        Lu = e(186),
+        Pu = e(302),
+        Du = e(301);
 
-    function Eu(t) {
+    function Tu(t) {
         var e = t.fullscreen,
             o = t.validRange,
             i = t.generateConfig,
             n = t.locale,
             a = t.prefixCls,
             l = t.value,
             c = t.onChange,
@@ -118963,15 +119105,15 @@
             },
             getPopupContainer: function() {
                 return r.current
             }
         })
     }
 
-    function Cu(t) {
+    function zu(t) {
         var e, n, a = t.prefixCls,
             r = t.fullscreen,
             o = t.validRange,
             i = t.value,
             l = t.generateConfig,
             c = t.locale,
             s = t.onChange,
@@ -118994,75 +119136,75 @@
             },
             getPopupContainer: function() {
                 return u.current
             }
         })
     }
 
-    function Su(t) {
+    function Au(t) {
         var e = t.prefixCls,
             n = t.locale,
             a = t.mode,
             r = t.fullscreen,
             o = t.onModeChange;
-        return Wt.createElement(ju.a, {
+        return Wt.createElement(Pu.a, {
             onChange: function(t) {
                 t = t.target.value;
                 o(t)
             },
             value: a,
             size: r ? void 0 : "small",
             className: "".concat(e, "-mode-switch")
-        }, Wt.createElement(Mu.a, {
+        }, Wt.createElement(Du.a, {
             value: "month"
-        }, n.month), Wt.createElement(Mu.a, {
+        }, n.month), Wt.createElement(Du.a, {
             value: "year"
         }, n.year))
     }
 
-    function Lu(t) {
+    function Ru(t) {
         var e = t.prefixCls,
             n = t.fullscreen,
             a = t.mode,
             r = t.onChange,
             o = t.onModeChange,
             i = Wt.useRef(null),
-            l = Object(Wt.useContext)(ve.b),
+            l = Object(Wt.useContext)(Oe.b),
             c = Object(Wt.useMemo)(function() {
                 return Object(Et.a)(Object(Et.a)({}, l), {
                     isFormItemInput: !1
                 })
             }, [l]),
             t = Object(Et.a)(Object(Et.a)({}, t), {
                 onChange: r,
                 fullscreen: n,
                 divRef: i
             });
         return Wt.createElement("div", {
             className: "".concat(e, "-header"),
             ref: i
-        }, Wt.createElement(ve.b.Provider, {
+        }, Wt.createElement(Oe.b.Provider, {
             value: c
-        }, Wt.createElement(Eu, Object(Et.a)({}, t)), "month" === a && Wt.createElement(Cu, Object(Et.a)({}, t))), Wt.createElement(Su, Object(Et.a)({}, t, {
+        }, Wt.createElement(Tu, Object(Et.a)({}, t)), "month" === a && Wt.createElement(zu, Object(Et.a)({}, t))), Wt.createElement(Au, Object(Et.a)({}, t, {
             onModeChange: o
         })))
     }
 
-    function Pu(n) {
+    function Iu(n) {
         function a(t, e) {
             null != y && y(t, e)
         }
 
         function r(t) {
             L(t), a(E, t)
         }
 
         function o(t) {
             var e;
-            C(e = t), Ru(e, E) || (("date" === P && !Au(e, E) || "month" === P && !zu(e, E)) && a(e, S), null == v) || v(e), null != x && x(t)
+            C(e = t), Hu(e, E) || (("date" === P && !Fu(e, E) || "month" === P && !Bu(e, E)) && a(e, S), null == v) || v(e), null != x && x(t)
         }
         var t = n.prefixCls,
             i = n.className,
             l = n.style,
             e = n.dateFullCellRender,
             c = n.dateCellRender,
             s = n.monthFullCellRender,
@@ -119078,79 +119220,79 @@
             y = n.onPanelChange,
             x = n.onSelect,
             _ = (M = Wt.useContext(q.b)).getPrefixCls,
             O = M.direction,
             w = _("picker", t),
             k = "".concat(w, "-calendar"),
             j = A.getNow(),
-            M = Object($t.a)(function() {
+            M = Object(Zt.a)(function() {
                 return p || A.getNow()
             }, {
                 defaultValue: f,
                 value: p
             }),
             E = (_ = Object(Gt.a)(M, 2))[0],
             C = _[1],
-            t = Object($t.a)("month", {
+            t = Object(Zt.a)("month", {
                 value: m
             }),
             S = (f = Object(Gt.a)(t, 2))[0],
             L = f[1],
             P = Wt.useMemo(function() {
                 return "year" === S ? "month" : "date"
             }, [S]),
             D = Wt.useCallback(function(t) {
                 return !!g && (A.isAfter(g[0], t) || A.isAfter(t, g[1])) || !(null == h || !h(t))
             }, [h, g]),
             T = Wt.useCallback(function(t) {
                 return e ? e(t) : Wt.createElement("div", {
-                    className: Kt()("".concat(w, "-cell-inner"), "".concat(k, "-date"), Object(Vt.a)({}, "".concat(k, "-date-today"), Ru(j, t)))
+                    className: Kt()("".concat(w, "-cell-inner"), "".concat(k, "-date"), Object(Vt.a)({}, "".concat(k, "-date-today"), Hu(j, t)))
                 }, Wt.createElement("div", {
                     className: "".concat(k, "-date-value")
-                }, bc()(String(A.getDate(t)), 2, "0")), Wt.createElement("div", {
+                }, wc()(String(A.getDate(t)), 2, "0")), Wt.createElement("div", {
                     className: "".concat(k, "-date-content")
                 }, c && c(t)))
             }, [e, c]),
             z = Wt.useCallback(function(t, e) {
                 return s ? s(t) : (e = e.shortMonths || A.locale.getShortMonths(e.locale), Wt.createElement("div", {
-                    className: Kt()("".concat(w, "-cell-inner"), "".concat(k, "-date"), Object(Vt.a)({}, "".concat(k, "-date-today"), Au(j, t)))
+                    className: Kt()("".concat(w, "-cell-inner"), "".concat(k, "-date"), Object(Vt.a)({}, "".concat(k, "-date-today"), Fu(j, t)))
                 }, Wt.createElement("div", {
                     className: "".concat(k, "-date-value")
                 }, e[A.getMonth(t)]), Wt.createElement("div", {
                     className: "".concat(k, "-date-content")
                 }, u && u(t))))
             }, [s, u]);
-        return Wt.createElement(ye.a, {
+        return Wt.createElement(we.a, {
             componentName: "Calendar",
             defaultLocale: function() {
                 var t = n.locale,
-                    e = Object(Et.a)(Object(Et.a)({}, Tu.a), t);
+                    e = Object(Et.a)(Object(Et.a)({}, Yu.a), t);
                 return e.lang = Object(Et.a)(Object(Et.a)({}, e.lang), (t || {}).lang), e
             }
         }, function(e) {
             var t;
             return Wt.createElement("div", {
                 className: Kt()(k, (t = {}, Object(Vt.a)(t, "".concat(k, "-full"), b), Object(Vt.a)(t, "".concat(k, "-mini"), !b), Object(Vt.a)(t, "".concat(k, "-rtl"), "rtl" === O), t), i),
                 style: l
             }, d ? d({
                 value: E,
                 type: S,
                 onChange: o,
                 onTypeChange: r
-            }) : Wt.createElement(Lu, {
+            }) : Wt.createElement(Ru, {
                 prefixCls: k,
                 value: E,
                 generateConfig: A,
                 mode: S,
                 fullscreen: b,
                 locale: e.lang,
                 validRange: g,
                 onChange: o,
                 onModeChange: r
-            }), Wt.createElement(ku.a, {
+            }), Wt.createElement(Lu.a, {
                 value: E,
                 prefixCls: w,
                 locale: e.lang,
                 generateConfig: A,
                 dateRender: T,
                 monthCellRender: function(t) {
                     return z(t, e.lang)
@@ -119160,15 +119302,15 @@
                 picker: P,
                 disabledDate: D,
                 hideHeader: !0
             }))
         })
     }
 
-    function Du(t) {
+    function Nu(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.locale,
             i = t.defaultValue,
             l = t.value,
@@ -119183,15 +119325,15 @@
             o = h && h.locale || o;
         return Object(Wt.useEffect)(function() {
             i && !l && u({
                 value: i
             })
         }, []), H.a.createElement(W.a, {
             locale: K.b.get(o)
-        }, H.a.createElement(Pu, {
+        }, H.a.createElement(Iu, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             defaultValue: i && C()(i, c),
             value: l && C()(l, c),
             onSelect: function(t) {
@@ -119202,29 +119344,29 @@
             fullscreen: "default" !== s,
             persistence: p,
             persisted_props: f,
             persistence_type: t,
             "data-dash-is-loading": d && d.is_loading || void 0
         }))
     }
-    var A, Tu = e(248);
+    var A, Yu = e(248);
     A = c.a;
 
-    function zu(t, e) {
+    function Bu(t, e) {
         return t && e && A.getYear(t) === A.getYear(e)
     }
 
-    function Au(t, e) {
-        return zu(t, e) && A.getMonth(t) === A.getMonth(e)
+    function Fu(t, e) {
+        return Bu(t, e) && A.getMonth(t) === A.getMonth(e)
     }
 
-    function Ru(t, e) {
-        return Au(t, e) && A.getDate(t) === A.getDate(e)
+    function Hu(t, e) {
+        return Fu(t, e) && A.getDate(t) === A.getDate(e)
     }
-    Du.propTypes = {
+    Nu.propTypes = {
         id: n.a.string,
         className: n.a.oneOfType([n.a.string, n.a.object]),
         style: n.a.object,
         key: n.a.string,
         locale: n.a.oneOf(["zh-cn", "en-us"]),
         format: n.a.string,
         size: n.a.oneOf(["default", "large"]),
@@ -119235,32 +119377,32 @@
             prop_name: n.a.string,
             component_name: n.a.string
         }),
         setProps: n.a.func,
         persistence: n.a.oneOfType([n.a.bool, n.a.string, n.a.number]),
         persisted_props: n.a.arrayOf(n.a.oneOf(["value"])),
         persistence_type: n.a.oneOf(["local", "session", "memory"])
-    }, Du.defaultProps = {
+    }, Nu.defaultProps = {
         format: "YYYY-MM-DD",
         size: "default",
         persisted_props: ["value"],
         persistence_type: "local",
         locale: "zh-cn"
     };
 
-    function Iu(t) {
+    function Wu(t) {
         var e = t.actions,
             n = t.author,
             a = t.avatar,
             r = t.children,
             o = t.className,
             i = t.content,
             l = t.prefixCls,
             c = t.datetime,
-            t = Hu(t, ["actions", "author", "avatar", "children", "className", "content", "prefixCls", "datetime"]),
+            t = qu(t, ["actions", "author", "avatar", "children", "className", "content", "prefixCls", "datetime"]),
             s = (u = Wt.useContext(q.b)).getPrefixCls,
             u = u.direction,
             s = s("comment", l),
             l = a ? Wt.createElement("div", {
                 className: "".concat(s, "-avatar")
             }, "string" == typeof a ? Wt.createElement("img", {
                 src: a,
@@ -119291,29 +119433,29 @@
         }), Wt.createElement("div", {
             className: "".concat(s, "-inner")
         }, l, n), r ? (e = s, i = r, Wt.createElement("div", {
             className: Kt()("".concat(e, "-nested"))
         }, i)) : null)
     }
 
-    function Nu(t, e) {
-        return Wt.createElement(to.a, Object(Ct.a)(Object(Ct.a)({}, t), {}, {
+    function Vu(t, e) {
+        return Wt.createElement(ao.a, Object(Ct.a)(Object(Ct.a)({}, t), {}, {
             ref: e,
-            icon: Wu
+            icon: Xu
         }))
     }
 
-    function Yu(t, e) {
-        return Wt.createElement(to.a, Object(Ct.a)(Object(Ct.a)({}, t), {}, {
+    function Ku(t, e) {
+        return Wt.createElement(ao.a, Object(Ct.a)(Object(Ct.a)({}, t), {}, {
             ref: e,
-            icon: Uu
+            icon: Ju
         }))
     }
 
-    function Bu(t) {
+    function Uu(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = (t.key, t.locale),
             i = t.commentId,
             l = t.showLikeDislike,
@@ -119346,41 +119488,41 @@
                 onClick: function() {
                     w({
                         likesCount: "liked" === y ? b - 1 : b + 1,
                         action: "liked" === y ? "default" : "liked",
                         dislikesCount: "disliked" === y ? v - 1 : v
                     })
                 }
-            }, "liked" === y ? H.a.createElement(Vu, {
+            }, "liked" === y ? H.a.createElement($u, {
                 style: {
                     color: "rgb(236, 65, 65)"
                 }
-            }) : H.a.createElement(Ku.a, null), H.a.createElement("span", {
+            }) : H.a.createElement(Zu.a, null), H.a.createElement("span", {
                 className: "comment-action"
             }, b))) : void 0, l ? H.a.createElement(D.a, {
                 key: "comment-basic-dislike",
                 title: "zh-cn" === o ? "反对" : "dislike"
             }, H.a.createElement("span", {
                 onClick: function() {
                     w({
                         dislikesCount: "disliked" === y ? v - 1 : v + 1,
                         action: "disliked" === y ? "default" : "disliked",
                         likesCount: "liked" === y ? b - 1 : b
                     })
                 }
-            }, H.a.createElement("disliked" === y ? Gu : qu.a), H.a.createElement("span", {
+            }, H.a.createElement("disliked" === y ? Qu : td.a), H.a.createElement("span", {
                 className: "comment-action"
             }, v))) : void 0, c ? H.a.createElement("span", {
                 key: "comment-basic-reply-to",
                 onClick: function() {
                     w({
                         replyClicks: u + 1
                     })
                 }
-            }, "zh-cn" === o ? "添加回复" : "Add a reply") : void 0, s ? H.a.createElement(wl.a, {
+            }, "zh-cn" === o ? "添加回复" : "Add a reply") : void 0, s ? H.a.createElement(Ml.a, {
                 title: "zh-cn" === o ? "确认删除" : "Confirm deletion",
                 onConfirm: function() {
                     return w({
                         deleteClicks: d + 1
                     })
                 },
                 okText: "zh-cn" === o ? "确认" : "Yes",
@@ -119389,42 +119531,42 @@
                     return t.parentNode
                 } : void 0
             }, H.a.createElement("span", {
                 key: "comment-basic-delete"
             }, "zh-cn" === o ? "删除" : "Delete")) : void 0]);
         return H.a.createElement(W.a, {
             locale: K.b.get(o)
-        }, H.a.createElement(Iu, {
+        }, H.a.createElement(Wu, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: i,
             actions: k,
             author: H.a.createElement("a", {
                 href: f,
                 target: "_blank"
             }, p),
-            avatar: H.a.createElement(Fc, _),
+            avatar: H.a.createElement(Gc, _),
             content: H.a.createElement("p", null, g),
             datetime: H.a.createElement(D.a, {
                 title: C()().format(h.value),
                 placement: "right"
             }, H.a.createElement("span", null, m ? C()(h.value, h.format || "YYYY-MM-DD HH:mm:ss").fromNow() : h.value)),
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n))
     }
-    var Fu = Du,
-        Hu = function(t, e) {
+    var Gu = Nu,
+        qu = function(t, e) {
             var n = {};
             for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
             if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                 for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
             return n
         },
-        Wu = {
+        Xu = {
             icon: {
                 tag: "svg",
                 attrs: {
                     viewBox: "64 64 896 896",
                     focusable: "false"
                 },
                 children: [{
@@ -119433,17 +119575,17 @@
                         d: "M885.9 533.7c16.8-22.2 26.1-49.4 26.1-77.7 0-44.9-25.1-87.4-65.5-111.1a67.67 67.67 0 00-34.3-9.3H572.4l6-122.9c1.4-29.7-9.1-57.9-29.5-79.4A106.62 106.62 0 00471 99.9c-52 0-98 35-111.8 85.1l-85.9 311h-.3v428h472.3c9.2 0 18.2-1.8 26.5-5.4 47.6-20.3 78.3-66.8 78.3-118.4 0-12.6-1.8-25-5.4-37 16.8-22.2 26.1-49.4 26.1-77.7 0-12.6-1.8-25-5.4-37 16.8-22.2 26.1-49.4 26.1-77.7-.2-12.6-2-25.1-5.6-37.1zM112 528v364c0 17.7 14.3 32 32 32h65V496h-65c-17.7 0-32 14.3-32 32z"
                     }
                 }]
             },
             name: "like",
             theme: "filled"
         },
-        Vu = (Nu.displayName = "LikeFilled", Wt.forwardRef(Nu)),
-        Ku = e(710),
-        Uu = {
+        $u = (Vu.displayName = "LikeFilled", Wt.forwardRef(Vu)),
+        Zu = e(710),
+        Ju = {
             icon: {
                 tag: "svg",
                 attrs: {
                     viewBox: "64 64 896 896",
                     focusable: "false"
                 },
                 children: [{
@@ -119452,17 +119594,17 @@
                         d: "M885.9 490.3c3.6-12 5.4-24.4 5.4-37 0-28.3-9.3-55.5-26.1-77.7 3.6-12 5.4-24.4 5.4-37 0-28.3-9.3-55.5-26.1-77.7 3.6-12 5.4-24.4 5.4-37 0-51.6-30.7-98.1-78.3-118.4a66.1 66.1 0 00-26.5-5.4H273v428h.3l85.8 310.8C372.9 889 418.9 924 470.9 924c29.7 0 57.4-11.8 77.9-33.4 20.5-21.5 31-49.7 29.5-79.4l-6-122.9h239.9c12.1 0 23.9-3.2 34.3-9.3 40.4-23.5 65.5-66.1 65.5-111 0-28.3-9.3-55.5-26.1-77.7zM112 132v364c0 17.7 14.3 32 32 32h65V100h-65c-17.7 0-32 14.3-32 32z"
                     }
                 }]
             },
             name: "dislike",
             theme: "filled"
         },
-        Gu = (Yu.displayName = "DislikeFilled", Wt.forwardRef(Yu)),
-        qu = e(711),
-        Xu = (Bu.propTypes = {
+        Qu = (Ku.displayName = "DislikeFilled", Wt.forwardRef(Ku)),
+        td = e(711),
+        ed = (Uu.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             locale: n.a.oneOf(["zh-cn", "en-us"]),
             commentId: n.a.string,
             authorName: n.a.string,
@@ -119486,51 +119628,51 @@
             popupContainer: n.a.oneOf(["parent", "body"]),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, Bu.defaultProps = {
+        }, Uu.defaultProps = {
             showLikeDislike: !0,
             showReply: !0,
             showDelete: !1,
             likesCount: 0,
             dislikesCount: 0,
             deleteClicks: 0,
             fromNow: !1,
             replyClicks: 0,
             locale: "zh-cn",
             popupContainer: "body"
-        }, Bu),
-        $u = e(84);
+        }, Uu),
+        nd = e(84);
 
-    function Zu(t) {
+    function ad(t) {
         return null != t
     }
 
-    function Ju(t) {
+    function rd(t) {
         var e = t.itemPrefixCls,
             n = t.component,
             a = t.span,
             r = t.className,
             o = t.style,
             i = t.labelStyle,
             l = t.contentStyle,
             c = t.bordered,
             s = t.label,
             u = t.content,
             t = t.colon;
         return c ? Wt.createElement(n, {
-            className: Kt()((c = {}, Object(Vt.a)(c, "".concat(e, "-item-label"), Zu(s)), Object(Vt.a)(c, "".concat(e, "-item-content"), Zu(u)), c), r),
+            className: Kt()((c = {}, Object(Vt.a)(c, "".concat(e, "-item-label"), ad(s)), Object(Vt.a)(c, "".concat(e, "-item-content"), ad(u)), c), r),
             style: o,
             colSpan: a
-        }, Zu(s) && Wt.createElement("span", {
+        }, ad(s) && Wt.createElement("span", {
             style: i
-        }, s), Zu(u) && Wt.createElement("span", {
+        }, s), ad(u) && Wt.createElement("span", {
             style: l
         }, u)) : Wt.createElement(n, {
             className: Kt()("".concat(e, "-item"), r),
             style: o,
             colSpan: a
         }, Wt.createElement("div", {
             className: "".concat(e, "-item-container")
@@ -119539,15 +119681,15 @@
             style: i
         }, s), (u || 0 === u) && Wt.createElement("span", {
             className: Kt()("".concat(e, "-item-content")),
             style: l
         }, u)))
     }
 
-    function Qu(t, e, n) {
+    function od(t, e, n) {
         var u = e.colon,
             d = e.prefixCls,
             p = e.bordered,
             f = n.component,
             h = n.type,
             m = n.showLabel,
             g = n.showContent,
@@ -119562,104 +119704,104 @@
                 i = n.className,
                 l = n.style,
                 c = n.labelStyle,
                 s = n.contentStyle,
                 n = n.span,
                 n = void 0 === n ? 1 : n,
                 t = t.key;
-            return "string" == typeof f ? Wt.createElement(Ju, {
+            return "string" == typeof f ? Wt.createElement(rd, {
                 key: "".concat(h, "-").concat(t || e),
                 className: i,
                 style: l,
                 labelStyle: Object(Et.a)(Object(Et.a)({}, b), c),
                 contentStyle: Object(Et.a)(Object(Et.a)({}, v), s),
                 span: n,
                 colon: u,
                 component: f,
                 itemPrefixCls: o,
                 bordered: p,
                 label: m ? a : null,
                 content: g ? r : null
-            }) : [Wt.createElement(Ju, {
+            }) : [Wt.createElement(rd, {
                 key: "label-".concat(t || e),
                 className: i,
                 style: Object(Et.a)(Object(Et.a)(Object(Et.a)({}, b), l), c),
                 span: 1,
                 colon: u,
                 component: f[0],
                 itemPrefixCls: o,
                 bordered: p,
                 label: a
-            }), Wt.createElement(Ju, {
+            }), Wt.createElement(rd, {
                 key: "content-".concat(t || e),
                 className: i,
                 style: Object(Et.a)(Object(Et.a)(Object(Et.a)({}, v), l), s),
                 span: 2 * n - 1,
                 component: f[1],
                 itemPrefixCls: o,
                 bordered: p,
                 content: r
             })]
         })
     }
 
-    function td(t) {
-        var e = Wt.useContext(ed),
+    function id(t) {
+        var e = Wt.useContext(ld),
             n = t.prefixCls,
             a = t.vertical,
             r = t.row,
             o = t.index,
             i = t.bordered;
         return a ? Wt.createElement(Wt.Fragment, null, Wt.createElement("tr", {
             key: "label-".concat(o),
             className: "".concat(n, "-row")
-        }, Qu(r, t, Object(Et.a)({
+        }, od(r, t, Object(Et.a)({
             component: "th",
             type: "label",
             showLabel: !0
         }, e))), Wt.createElement("tr", {
             key: "content-".concat(o),
             className: "".concat(n, "-row")
-        }, Qu(r, t, Object(Et.a)({
+        }, od(r, t, Object(Et.a)({
             component: "td",
             type: "content",
             showContent: !0
         }, e)))) : Wt.createElement("tr", {
             key: o,
             className: "".concat(n, "-row")
-        }, Qu(r, t, Object(Et.a)({
+        }, od(r, t, Object(Et.a)({
             component: i ? ["th", "td"] : "td",
             type: "item",
             showLabel: !0,
             showContent: !0
         }, e)))
     }
-    var ed = Wt.createContext({}),
-        nd = {
+    var ld = Wt.createContext({}),
+        cd = {
             xxl: 3,
             xl: 3,
             lg: 3,
             md: 3,
             sm: 2,
             xs: 1
         };
 
-    function ad(t, e, n) {
+    function sd(t, e, n) {
         var a = t;
-        return a = void 0 === e || n < e ? Object(je.a)(t, {
+        return a = void 0 === e || n < e ? Object(Ce.a)(t, {
             span: n
         }) : a
     }
 
-    function rd(t) {
+    function ud(t) {
         var r, o, i, l, c, e = t.prefixCls,
             n = t.title,
             a = t.extra,
             s = t.column,
-            u = void 0 === s ? nd : s,
+            u = void 0 === s ? cd : s,
             s = t.colon,
             d = void 0 === s || s,
             p = t.bordered,
             f = t.layout,
             s = t.children,
             h = t.className,
             m = t.style,
@@ -119673,82 +119815,82 @@
             y = Wt.useState({}),
             e = Object(Gt.a)(y, 2),
             y = e[0],
             _ = e[1],
             e = function(t, e) {
                 if ("number" == typeof t) return t;
                 if ("object" === Object(qt.a)(t))
-                    for (var n = 0; n < $u.b.length; n++) {
-                        var a = $u.b[n];
-                        if (e[a] && void 0 !== t[a]) return t[a] || nd[a]
+                    for (var n = 0; n < nd.b.length; n++) {
+                        var a = nd.b[n];
+                        if (e[a] && void 0 !== t[a]) return t[a] || cd[a]
                     }
                 return 3
             }(u, y),
             s = (Wt.useEffect(function() {
-                var t = $u.a.subscribe(function(t) {
+                var t = nd.a.subscribe(function(t) {
                     "object" === Object(qt.a)(u) && _(t)
                 });
                 return function() {
-                    $u.a.unsubscribe(t)
+                    nd.a.unsubscribe(t)
                 }
-            }, []), y = s, r = e, o = Object(Dn.a)(y).filter(function(t) {
+            }, []), y = s, r = e, o = Object(An.a)(y).filter(function(t) {
                 return t
             }), i = [], l = [], c = r, o.forEach(function(t, e) {
                 var n = null == (n = t.props) ? void 0 : n.span,
                     a = n || 1;
-                e === o.length - 1 ? (l.push(ad(t, n, c)), i.push(l)) : a < c ? (c -= a, l.push(t)) : (l.push(ad(t, a, c)), i.push(l), c = r, l = [])
+                e === o.length - 1 ? (l.push(sd(t, n, c)), i.push(l)) : a < c ? (c -= a, l.push(t)) : (l.push(sd(t, a, c)), i.push(l), c = r, l = [])
             }), i),
             e = Wt.useMemo(function() {
                 return {
                     labelStyle: b,
                     contentStyle: v
                 }
             }, [b, v]);
-        return Wt.createElement(ed.Provider, {
+        return Wt.createElement(ld.Provider, {
             value: e
         }, Wt.createElement("div", {
             className: Kt()(x, (y = {}, Object(Vt.a)(y, "".concat(x, "-").concat(g), g && "default" !== g), Object(Vt.a)(y, "".concat(x, "-bordered"), !!p), Object(Vt.a)(y, "".concat(x, "-rtl"), "rtl" === t), y), h),
             style: m
         }, (n || a) && Wt.createElement("div", {
             className: "".concat(x, "-header")
         }, n && Wt.createElement("div", {
             className: "".concat(x, "-title")
         }, n), a && Wt.createElement("div", {
             className: "".concat(x, "-extra")
         }, a)), Wt.createElement("div", {
             className: "".concat(x, "-view")
         }, Wt.createElement("table", null, Wt.createElement("tbody", null, s.map(function(t, e) {
-            return Wt.createElement(td, {
+            return Wt.createElement(id, {
                 key: e,
                 index: e,
                 colon: d,
                 prefixCls: x,
                 vertical: "vertical" === f,
                 bordered: p,
                 row: t
             })
         }))))))
     }
-    rd.Item = function(t) {
+    ud.Item = function(t) {
         return t.children
     };
-    var od = rd,
-        id = ["id", "className", "style", "label", "span", "labelStyle", "contentStyle", "loading_state"];
+    var dd = ud,
+        pd = ["id", "className", "style", "label", "span", "labelStyle", "contentStyle", "loading_state"];
 
-    function ld() {
-        return (ld = Object.assign ? Object.assign.bind() : function(t) {
+    function fd() {
+        return (fd = Object.assign ? Object.assign.bind() : function(t) {
             for (var e = 1; e < arguments.length; e++) {
                 var n, a = arguments[e];
                 for (n in a) Object.prototype.hasOwnProperty.call(a, n) && (t[n] = a[n])
             }
             return t
         }).apply(this, arguments)
     }
 
-    function cd(t) {
+    function hd(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.title,
             l = t.column,
@@ -119761,15 +119903,15 @@
             n = j(n),
             f = new Map([
                 ["small", "small"],
                 ["default", "middle"],
                 ["large", "default"]
             ]),
             n = n.map(function(t) {
-                var e = Y(t),
+                var e = et(t),
                     n = e.id,
                     a = e.className,
                     r = e.style,
                     o = e.label,
                     i = e.span,
                     l = e.labelStyle,
                     c = e.contentStyle,
@@ -119780,27 +119922,27 @@
                             if (null == t) return {};
                             for (var n, a = {}, r = Object.keys(t), o = 0; o < r.length; o++) n = r[o], 0 <= e.indexOf(n) || (a[n] = t[n]);
                             return a
                         }(t, e);
                         if (Object.getOwnPropertySymbols)
                             for (var r = Object.getOwnPropertySymbols(t), o = 0; o < r.length; o++) n = r[o], 0 <= e.indexOf(n) || Object.prototype.propertyIsEnumerable.call(t, n) && (a[n] = t[n]);
                         return a
-                    }(e, id);
-                return H.a.createElement(od.Item, ld({
+                    }(e, pd);
+                return H.a.createElement(dd.Item, fd({
                     id: n,
                     className: a,
                     style: r,
                     label: o,
                     span: i,
                     labelStyle: l,
                     contentStyle: c,
                     loading_state: s
-                }, Ao(["setProps", "persistence", "persistence_type", "persisted_props"], e)), t)
+                }, No(["setProps", "persistence", "persistence_type", "persisted_props"], e)), t)
             });
-        return H.a.createElement(od, {
+        return H.a.createElement(dd, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             title: i,
             column: l,
             bordered: c,
@@ -119808,15 +119950,15 @@
             layout: u,
             labelStyle: d,
             contentStyle: p,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
 
-    function sd(t) {
+    function md(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.label,
             l = t.span,
@@ -119833,15 +119975,15 @@
             span: l,
             labelStyle: c,
             contentStyle: s,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
 
-    function ud(t) {
+    function gd(t) {
         var e = t.children,
             n = t.style,
             a = t.className,
             r = t.markStyle,
             o = t.markClassName,
             i = void 0 === (i = t.zIndex) ? 9 : i,
             u = void 0 === (l = t.gapX) ? 212 : l,
@@ -119898,30 +120040,30 @@
                 }, t ? {
                     backgroundImage: "url('".concat(t, "')")
                 } : null), r)
             })]
         })
     }
 
-    function dd(t) {
+    function bd(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.content,
             l = t.rotate,
             c = t.zIndex,
             s = t.fontColor,
             u = t.fontSize,
             d = t.gapX,
             p = t.gapY,
             t = t.loading_state,
             n = j(n);
-        return H.a.createElement(ud, {
+        return H.a.createElement(gd, {
             id: e,
             className: a,
             style: r,
             key: o,
             content: i,
             rotate: l,
             zIndex: c,
@@ -119929,26 +120071,26 @@
             fontSize: u,
             gapX: d,
             gapY: p,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
 
-    function pd(t) {
+    function vd(t) {
         return t ? {
             left: t.offsetLeft,
             right: t.parentElement.clientWidth - t.clientWidth - t.offsetLeft,
             width: t.clientWidth
         } : null
     }
 
-    function fd(t) {
+    function yd(t) {
         return void 0 !== t ? "".concat(t, "px") : void 0
     }
-    cd.propTypes = {
+    hd.propTypes = {
         id: n.a.string,
         children: n.a.node,
         className: n.a.oneOfType([n.a.string, n.a.object]),
         style: n.a.object,
         key: n.a.string,
         title: n.a.node,
         column: n.a.oneOfType([n.a.number, n.a.exact({
@@ -119966,22 +120108,22 @@
         contentStyle: n.a.object,
         loading_state: n.a.shape({
             is_loading: n.a.bool,
             prop_name: n.a.string,
             component_name: n.a.string
         }),
         setProps: n.a.func
-    }, cd.defaultProps = {
+    }, hd.defaultProps = {
         column: 3,
         bordered: !1,
         layout: "horizontal",
         size: "default"
     };
-    var hd = cd,
-        md = (sd.propTypes = {
+    var xd = hd,
+        _d = (md.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             label: n.a.node,
             span: n.a.number,
@@ -119989,19 +120131,19 @@
             contentStyle: n.a.object,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, sd.defaultProps = {
+        }, md.defaultProps = {
             span: 1
-        }, sd),
+        }, md),
         F = (e(298), e(31)),
-        gd = (dd.propTypes = {
+        Od = (bd.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.string,
             style: n.a.object,
             key: n.a.string,
             content: n.a.string,
             rotate: n.a.number,
@@ -120012,22 +120154,22 @@
             gapY: n.a.number,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, dd.defaultProps = {
+        }, bd.defaultProps = {
             rotate: -22,
             fontSize: 16,
             gapX: 212,
             gapY: 222
-        }, dd);
+        }, bd);
 
-    function bd(t) {
+    function wd(t) {
         function r(t) {
             var t = i(t),
                 e = null == (e = n.current) ? void 0 : e.querySelectorAll(".".concat(a, "-item"))[t];
             return (null == e ? void 0 : e.offsetParent) && e
         }
         var a = t.prefixCls,
             n = t.containerRef,
@@ -120046,24 +120188,24 @@
             t = Object(Gt.a)(t, 2),
             f = t[0],
             h = t[1],
             t = Wt.useState(null),
             t = Object(Gt.a)(t, 2),
             m = t[0],
             g = t[1],
-            b = (Object(ji.a)(function() {
+            b = (Object(Ci.a)(function() {
                 var t, e, n, a;
-                d !== o && (t = r(d), e = r(o), n = pd(t), a = pd(e), p(o), h(n), g(a), (t && e ? l : c)())
+                d !== o && (t = r(d), e = r(o), n = vd(t), a = vd(e), p(o), h(n), g(a), (t && e ? l : c)())
             }, [o]), Wt.useMemo(function() {
-                return fd("rtl" === s ? -(null == f ? void 0 : f.right) : null == f ? void 0 : f.left)
+                return yd("rtl" === s ? -(null == f ? void 0 : f.right) : null == f ? void 0 : f.left)
             }, [s, f])),
             v = Wt.useMemo(function() {
-                return fd("rtl" === s ? -(null == m ? void 0 : m.right) : null == m ? void 0 : m.left)
+                return yd("rtl" === s ? -(null == m ? void 0 : m.right) : null == m ? void 0 : m.left)
             }, [s, m]);
-        return f && m ? Wt.createElement(Er.b, {
+        return f && m ? Wt.createElement(Lr.b, {
             visible: !0,
             motionName: e,
             motionAppear: !0,
             onAppearStart: function() {
                 return {
                     transform: "translateX(var(--thumb-start-left))",
                     width: "var(--thumb-start-width)"
@@ -120079,42 +120221,42 @@
                 h(null), g(null), c()
             }
         }, function(t, e) {
             var n = t.className,
                 t = t.style,
                 t = Object(Ct.a)(Object(Ct.a)({}, t), {}, {
                     "--thumb-start-left": b,
-                    "--thumb-start-width": fd(null == f ? void 0 : f.width),
+                    "--thumb-start-width": yd(null == f ? void 0 : f.width),
                     "--thumb-active-left": v,
-                    "--thumb-active-width": fd(null == m ? void 0 : m.width)
+                    "--thumb-active-width": yd(null == m ? void 0 : m.width)
                 }),
                 e = {
-                    ref: Object(fe.a)(u, e),
+                    ref: Object(be.a)(u, e),
                     style: t,
                     className: Kt()("".concat(a, "-thumb"), n)
                 };
             return Wt.createElement("div", e)
         }) : null
     }
-    var vd = ["prefixCls", "direction", "options", "disabled", "defaultValue", "value", "onChange", "className", "motionName"];
+    var kd = ["prefixCls", "direction", "options", "disabled", "defaultValue", "value", "onChange", "className", "motionName"];
 
-    function yd(t) {
+    function jd(t) {
         return t.map(function(t) {
             var e;
             return "object" === Object(qt.a)(t) && null !== t ? (e = void 0 !== (e = t).title ? e.title : "object" === Object(qt.a)(e.label) || null == (e = e.label) ? void 0 : e.toString(), Object(Ct.a)(Object(Ct.a)({}, t), {}, {
                 title: e
             })) : {
                 label: null == t ? void 0 : t.toString(),
                 title: null == t ? void 0 : t.toString(),
                 value: t
             }
         })
     }
 
-    function xd(t) {
+    function Md(t) {
         var e = t.prefixCls,
             n = t.className,
             a = t.disabled,
             r = t.checked,
             o = t.label,
             i = t.title,
             l = t.value,
@@ -120131,15 +120273,15 @@
             }
         }), Wt.createElement("div", {
             className: "".concat(e, "-item-label"),
             title: i
         }, o))
     }
 
-    function _d(t, e) {
+    function Ed(t, e) {
         var n = {};
         for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
         if (null != t && "function" == typeof Object.getOwnPropertySymbols)
             for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
         return n
     }
     var d = Wt.forwardRef(function(t, e) {
@@ -120154,40 +120296,40 @@
                 l = t.defaultValue,
                 c = t.value,
                 s = t.onChange,
                 u = t.className,
                 u = void 0 === u ? "" : u,
                 d = t.motionName,
                 d = void 0 === d ? "thumb-motion" : d,
-                t = Object(Bt.a)(t, vd),
+                t = Object(Jt.a)(t, kd),
                 p = Wt.useRef(null),
                 f = Wt.useMemo(function() {
-                    return Object(fe.a)(p, e)
+                    return Object(be.a)(p, e)
                 }, [p, e]),
                 h = Wt.useMemo(function() {
-                    return yd(o)
+                    return jd(o)
                 }, [o]),
-                m = Object($t.a)(null == (m = h[0]) ? void 0 : m.value, {
+                m = Object(Zt.a)(null == (m = h[0]) ? void 0 : m.value, {
                     value: c,
                     defaultValue: l
                 }),
                 c = Object(Gt.a)(m, 2),
                 g = c[0],
                 b = c[1],
                 l = Wt.useState(!1),
                 m = Object(Gt.a)(l, 2),
                 v = m[0],
                 y = m[1],
-                c = Object(ct.a)(t, ["children"]);
+                c = Object(pt.a)(t, ["children"]);
             return Wt.createElement("div", Object(Et.a)({}, c, {
                 className: Kt()(r, (l = {}, Object(Vt.a)(l, "".concat(r, "-rtl"), "rtl" === a), Object(Vt.a)(l, "".concat(r, "-disabled"), i), l), u),
                 ref: f
             }), Wt.createElement("div", {
                 className: "".concat(r, "-group")
-            }, Wt.createElement(bd, {
+            }, Wt.createElement(wd, {
                 prefixCls: r,
                 value: g,
                 containerRef: p,
                 motionName: "".concat(r, "-").concat(d),
                 direction: a,
                 getValueIndex: function(e) {
                     return h.findIndex(function(t) {
@@ -120197,106 +120339,106 @@
                 onMotionStart: function() {
                     y(!0)
                 },
                 onMotionEnd: function() {
                     y(!1)
                 }
             }), h.map(function(t) {
-                return Wt.createElement(xd, Object(Et.a)({
+                return Wt.createElement(Md, Object(Et.a)({
                     key: t.value,
                     prefixCls: r,
                     className: Kt()(t.className, "".concat(r, "-item"), Object(Vt.a)({}, "".concat(r, "-item-selected"), t.value === g && !v)),
                     checked: t.value === g,
                     onChange: n
                 }, t, {
                     disabled: !!i || !!t.disabled
                 }))
             })))
         }),
-        Od = (d.displayName = "Segmented", d.defaultProps = {
+        Cd = (d.displayName = "Segmented", d.defaultProps = {
             options: []
         }, d),
-        wd = Wt.forwardRef(function(t, e) {
+        Sd = Wt.forwardRef(function(t, e) {
             var n = t.prefixCls,
                 a = t.className,
                 r = t.block,
                 o = t.options,
                 i = void 0 === o ? [] : o,
                 o = t.size,
                 o = void 0 === o ? "middle" : o,
-                t = _d(t, ["prefixCls", "className", "block", "options", "size"]),
+                t = Ed(t, ["prefixCls", "className", "block", "options", "size"]),
                 l = Wt.useContext(q.b),
                 c = l.getPrefixCls,
                 l = l.direction,
                 s = c("segmented", n),
-                c = Wt.useContext(fi.b),
+                c = Wt.useContext(gi.b),
                 n = o || c,
                 o = Wt.useMemo(function() {
                     return i.map(function(t) {
                         var e, n, a;
-                        return a = t, "object" === Object(qt.a)(a) && null != a && a.icon ? (a = t.icon, e = t.label, n = _d(t, ["icon", "label"]), Object(Et.a)(Object(Et.a)({}, n), {
+                        return a = t, "object" === Object(qt.a)(a) && null != a && a.icon ? (a = t.icon, e = t.label, n = Ed(t, ["icon", "label"]), Object(Et.a)(Object(Et.a)({}, n), {
                             label: Wt.createElement(Wt.Fragment, null, Wt.createElement("span", {
                                 className: "".concat(s, "-item-icon")
                             }, a), e && Wt.createElement("span", null, e))
                         })) : t
                     })
                 }, [i, s]);
-            return Wt.createElement(Od, Object(Et.a)({}, t, {
+            return Wt.createElement(Cd, Object(Et.a)({}, t, {
                 className: Kt()(a, (c = {}, Object(Vt.a)(c, "".concat(s, "-block"), r), Object(Vt.a)(c, "".concat(s, "-sm"), "small" === n), Object(Vt.a)(c, "".concat(s, "-lg"), "large" === n), c)),
                 options: o,
                 ref: e,
                 prefixCls: s,
                 direction: l
             }))
         });
 
-    function kd(t) {
-        return (kd = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
+    function Ld(t) {
+        return (Ld = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
             return typeof t
         } : function(t) {
             return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
         })(t)
     }
 
-    function jd(e, t) {
+    function Pd(e, t) {
         var n, a = Object.keys(e);
         return Object.getOwnPropertySymbols && (n = Object.getOwnPropertySymbols(e), t && (n = n.filter(function(t) {
             return Object.getOwnPropertyDescriptor(e, t).enumerable
         })), a.push.apply(a, n)), a
     }
 
-    function Md(a) {
+    function Dd(a) {
         for (var t = 1; t < arguments.length; t++) {
             var r = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? jd(Object(r), !0).forEach(function(t) {
+            t % 2 ? Pd(Object(r), !0).forEach(function(t) {
                 var e, n;
                 e = a, t = r[n = t], (n = function() {
                     var t = function(t) {
-                        if ("object" !== kd(t) || null === t) return t;
+                        if ("object" !== Ld(t) || null === t) return t;
                         var e = t[Symbol.toPrimitive];
                         if (void 0 === e) return String(t);
                         e = e.call(t, "string");
-                        if ("object" !== kd(e)) return e;
+                        if ("object" !== Ld(e)) return e;
                         throw new TypeError("@@toPrimitive must return a primitive value.")
                     }(n);
-                    return "symbol" === kd(t) ? t : String(t)
+                    return "symbol" === Ld(t) ? t : String(t)
                 }()) in e ? Object.defineProperty(e, n, {
                     value: t,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : e[n] = t
-            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(r)) : jd(Object(r)).forEach(function(t) {
+            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(r)) : Pd(Object(r)).forEach(function(t) {
                 Object.defineProperty(a, t, Object.getOwnPropertyDescriptor(r, t))
             })
         }
         return a
     }
 
-    function Ed(t) {
+    function Td(t) {
         var e = t.id,
             n = t.style,
             a = t.className,
             r = t.key,
             o = t.options,
             i = t.defaultValue,
             l = t.value,
@@ -120310,21 +120452,21 @@
             t = t.loading_state,
             m = Object(Wt.useContext)(G.a),
             o = o || [];
         return Object(Wt.useEffect)(function() {
             i && !l && d({
                 value: i
             })
-        }, []), H.a.createElement(wd, {
+        }, []), H.a.createElement(Sd, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: n,
             key: r,
             options: o.map(function(t) {
-                return Md(Md({}, t), {}, {
+                return Dd(Dd({}, t), {}, {
                     icon: t.icon && H.a.createElement(I.a, {
                         icon: t.icon
                     })
                 })
             }),
             defaultValue: i,
             value: l,
@@ -120339,100 +120481,100 @@
                     value: t
                 })
             },
             "data-dash-is-loading": t && t.is_loading || void 0
         })
     }
 
-    function Cd(t, e) {
-        return t = Object($t.a)(t, e), [(e = Object(Gt.a)(t, 2))[0], e[1]]
+    function zd(t, e) {
+        return t = Object(Zt.a)(t, e), [(e = Object(Gt.a)(t, 2))[0], e[1]]
     }
 
-    function Sd(t) {
+    function Ad(t) {
         var t = t.prefixCls,
             e = "".concat(t, "-loading-block");
         return Object(F.jsxs)("div", {
             className: "".concat(t, "-loading-content"),
-            children: [Object(F.jsx)(ua, {
+            children: [Object(F.jsx)(fa, {
                 gutter: 8,
-                children: Object(F.jsx)(pa, {
+                children: Object(F.jsx)(ma, {
                     span: 22,
                     children: Object(F.jsx)("div", {
                         className: e
                     })
                 })
-            }), Object(F.jsxs)(ua, {
+            }), Object(F.jsxs)(fa, {
                 gutter: 8,
-                children: [Object(F.jsx)(pa, {
+                children: [Object(F.jsx)(ma, {
                     span: 8,
                     children: Object(F.jsx)("div", {
                         className: e
                     })
-                }), Object(F.jsx)(pa, {
+                }), Object(F.jsx)(ma, {
                     span: 15,
                     children: Object(F.jsx)("div", {
                         className: e
                     })
                 })]
-            }), Object(F.jsxs)(ua, {
+            }), Object(F.jsxs)(fa, {
                 gutter: 8,
-                children: [Object(F.jsx)(pa, {
+                children: [Object(F.jsx)(ma, {
                     span: 6,
                     children: Object(F.jsx)("div", {
                         className: e
                     })
-                }), Object(F.jsx)(pa, {
+                }), Object(F.jsx)(ma, {
                     span: 18,
                     children: Object(F.jsx)("div", {
                         className: e
                     })
                 })]
-            }), Object(F.jsxs)(ua, {
+            }), Object(F.jsxs)(fa, {
                 gutter: 8,
-                children: [Object(F.jsx)(pa, {
+                children: [Object(F.jsx)(ma, {
                     span: 13,
                     children: Object(F.jsx)("div", {
                         className: e
                     })
-                }), Object(F.jsx)(pa, {
+                }), Object(F.jsx)(ma, {
                     span: 9,
                     children: Object(F.jsx)("div", {
                         className: e
                     })
                 })]
-            }), Object(F.jsxs)(ua, {
+            }), Object(F.jsxs)(fa, {
                 gutter: 8,
-                children: [Object(F.jsx)(pa, {
+                children: [Object(F.jsx)(ma, {
                     span: 4,
                     children: Object(F.jsx)("div", {
                         className: e
                     })
-                }), Object(F.jsx)(pa, {
+                }), Object(F.jsx)(ma, {
                     span: 3,
                     children: Object(F.jsx)("div", {
                         className: e
                     })
-                }), Object(F.jsx)(pa, {
+                }), Object(F.jsx)(ma, {
                     span: 16,
                     children: Object(F.jsx)("div", {
                         className: e
                     })
                 })]
             })]
         })
     }
 
-    function Ld(n) {
-        var t = Cd(n.defaultChecked || !1, {
+    function Rd(n) {
+        var t = zd(n.defaultChecked || !1, {
                 value: n.checked,
                 onChange: n.onChange
             }),
             a = (t = Object(Gt.a)(t, 2))[0],
             r = t[1],
-            o = Object(Wt.useContext)(Rd),
+            o = Object(Wt.useContext)(Hd),
             t = Object(Wt.useContext)(W.a.ConfigContext).getPrefixCls,
             e = (Object(Wt.useEffect)(function() {
                 var t;
                 return null != o && null != (t = o.registerValue) && t.call(o, n.value),
                     function() {
                         var t;
                         return null == o || null == (t = o.cancelValue) ? void 0 : t.call(o, n.value)
@@ -120441,39 +120583,39 @@
             i = n.className,
             l = n.avatar,
             c = n.title,
             s = n.description,
             u = n.cover,
             d = n.extra,
             p = void 0 === (p = n.style) ? {} : p,
-            f = Object(Bt.a)(n, Id),
+            f = Object(Jt.a)(n, Wd),
             f = Object(Ct.a)({}, f),
             h = t("pro-checkcard", e),
             t = (f.checked = a, !1);
         o && (f.disabled = n.disabled || o.disabled, f.loading = n.loading || o.loading, f.bordered = n.bordered || o.bordered, t = o.multiple, e = o.multiple ? null == (e = o.value) ? void 0 : e.includes(n.value) : o.value === n.value, f.checked = !f.loading && e, f.size = n.size || o.size);
         var m = void 0 !== (e = f.disabled) && e,
             e = f.size,
             g = f.loading,
             b = void 0 === (b = f.bordered) || b,
             f = f.checked,
             e = "large" === e ? "lg" : "small" === e ? "sm" : "",
             e = Kt()(h, i, (i = {}, Object(Vt.a)(i, "".concat(h, "-loading"), g), Object(Vt.a)(i, "".concat(h, "-").concat(e), e), Object(Vt.a)(i, "".concat(h, "-checked"), f), Object(Vt.a)(i, "".concat(h, "-multiple"), t), Object(Vt.a)(i, "".concat(h, "-disabled"), m), Object(Vt.a)(i, "".concat(h, "-bordered"), b), i)),
             f = Object(Wt.useMemo)(function() {
                 var t, e, n, a;
-                return g ? Object(F.jsx)(Sd, {
+                return g ? Object(F.jsx)(Ad, {
                     prefixCls: h || ""
                 }) : u ? (t = h || "", e = u, Object(F.jsx)("div", {
                     className: "".concat(t, "-cover"),
                     children: "string" == typeof e ? Object(F.jsx)("img", {
                         src: e,
                         alt: "checkcard"
                     }) : e
                 })) : (t = l ? Object(F.jsx)("div", {
                     className: "".concat(h, "-avatar"),
-                    children: "string" == typeof l ? Object(F.jsx)(Bc.a, {
+                    children: "string" == typeof l ? Object(F.jsx)(Uc.a, {
                         size: 48,
                         shape: "square",
                         src: l
                     }) : l
                 }) : null, e = (c || d) && Object(F.jsxs)("div", {
                     className: "".concat(h, "-header"),
                     children: [Object(F.jsx)("div", {
@@ -120503,15 +120645,15 @@
                     value: n.value
                 }), null != r && r(e))
             },
             children: f
         })
     }
 
-    function Pd(t) {
+    function Id(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.checked,
             l = t.bordered,
@@ -120525,15 +120667,15 @@
             m = t.persisted_props,
             t = t.persistence_type,
             g = Object(Wt.useContext)(G.a);
         return Object(Wt.useEffect)(function() {
             !Object(V.isUndefined)(s) && Object(V.isUndefined)(i) && p({
                 checked: s
             })
-        }, []), H.a.createElement(Nd, {
+        }, []), H.a.createElement(Vd, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             description: n,
             checked: i,
             bordered: l,
@@ -120549,15 +120691,15 @@
             persistence: h,
             persisted_props: m,
             persistence_type: t,
             "data-dash-is-loading": f && f.is_loading || void 0
         })
     }
 
-    function Dd(t) {
+    function Nd(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.multiple,
             l = t.bordered,
@@ -120571,15 +120713,15 @@
             m = t.persisted_props,
             t = t.persistence_type,
             g = Object(Wt.useContext)(G.a);
         return Object(Wt.useEffect)(function() {
             s && !c && p({
                 value: s
             })
-        }, []), n = j(n), H.a.createElement(Nd.Group, {
+        }, []), n = j(n), H.a.createElement(Vd.Group, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: r,
             key: o,
             multiple: i,
             bordered: l,
             value: c,
@@ -120594,15 +120736,15 @@
             persistence: h,
             persisted_props: m,
             persistence_type: t,
             "data-dash-is-loading": f && f.is_loading || void 0
         }, n)
     }
 
-    function Td(t) {
+    function Yd(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.items,
             i = t.accordion,
             l = t.activeKey,
@@ -120613,15 +120755,15 @@
             p = t.ghost,
             f = t.loading_state,
             h = t.setProps;
         return Object(Wt.useEffect)(function() {
             c && !l && h({
                 activeKey: c
             })
-        }, []), H.a.createElement(la.a, {
+        }, []), H.a.createElement(ua.a, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             accordion: i,
             activeKey: l,
             defaultActiveKey: c,
@@ -120632,27 +120774,27 @@
             onChange: function(t) {
                 return h({
                     activeKey: t
                 })
             },
             "data-dash-is-loading": f && f.is_loading || void 0
         }, o ? o.map(function(t) {
-            return H.a.createElement(Fd, {
+            return H.a.createElement(Gd, {
                 className: Object(V.isString)(t.className) ? t.className : t.className ? Object(U.a)(t.className) : void 0,
                 style: t.style,
                 key: t.key,
                 collapsible: t.collapsible,
                 header: t.title,
                 extra: t.extra,
                 showArrow: t.showArrow,
                 forceRender: t.forceRender
             }, t.children)
         }) : null)
     }
-    Ed.propTypes = {
+    Td.propTypes = {
         id: n.a.string,
         className: n.a.oneOfType([n.a.string, n.a.object]),
         style: n.a.object,
         key: n.a.string,
         options: n.a.arrayOf(n.a.exact({
             label: n.a.oneOfType([n.a.string, n.a.node]).isRequired,
             value: n.a.oneOfType([n.a.string, n.a.number]).isRequired,
@@ -120669,38 +120811,38 @@
             prop_name: n.a.string,
             component_name: n.a.string
         }),
         setProps: n.a.func,
         persistence: n.a.oneOfType([n.a.bool, n.a.string, n.a.number]),
         persisted_props: n.a.arrayOf(n.a.oneOf(["value"])),
         persistence_type: n.a.oneOf(["local", "session", "memory"])
-    }, Ed.defaultProps = {
+    }, Td.defaultProps = {
         block: !1,
         disabled: !1,
         size: "middle",
         persisted_props: ["value"],
         persistence_type: "local"
     };
-    var zd = Ed,
-        Ad = (e(670), e(206), e(482), e(481), ["prefixCls", "className", "style", "options", "loading", "multiple", "bordered", "onChange"]),
-        Rd = Object(Wt.createContext)(null),
-        Id = ["prefixCls", "className", "avatar", "title", "description", "cover", "extra", "style"],
-        Nd = (Ld.Group = function(a) {
+    var Bd = Td,
+        Fd = (e(670), e(206), e(482), e(481), ["prefixCls", "className", "style", "options", "loading", "multiple", "bordered", "onChange"]),
+        Hd = Object(Wt.createContext)(null),
+        Wd = ["prefixCls", "className", "avatar", "title", "description", "cover", "extra", "style"],
+        Vd = (Rd.Group = function(a) {
             var t = a.prefixCls,
                 e = a.className,
                 n = a.style,
                 r = a.options,
                 o = void 0 === r ? [] : r,
                 r = a.loading,
                 i = void 0 !== r && r,
                 r = a.multiple,
                 l = void 0 !== r && r,
                 r = a.bordered,
                 r = void 0 === r || r,
-                c = (a.onChange, Object(Bt.a)(a, Ad)),
+                c = (a.onChange, Object(Jt.a)(a, Fd)),
                 s = Object(Wt.useContext)(W.a.ConfigContext),
                 u = Object(Wt.useCallback)(function() {
                     return null == o ? void 0 : o.map(function(t) {
                         return "string" == typeof t ? {
                             title: t,
                             value: t
                         } : t
@@ -120708,45 +120850,45 @@
                 }, [o]),
                 s = s.getPrefixCls("pro-checkcard", t),
                 t = "".concat(s, "-group"),
                 s = function(t, e) {
                     for (var n = Object.assign({}, t), a = 0; a < e.length; a += 1) delete n[e[a]];
                     return n
                 }(c, ["children", "defaultValue", "value", "disabled", "size"]),
-                c = Cd(a.defaultValue, {
+                c = zd(a.defaultValue, {
                     value: a.value,
                     onChange: a.onChange
                 }),
                 c = Object(Gt.a)(c, 2),
                 d = c[0],
                 p = c[1],
                 f = Object(Wt.useRef)(new Map),
                 c = Object(Wt.useMemo)(function() {
                     var n;
                     return i ? new Array(o.length || H.a.Children.toArray(a.children).length || 1).fill(0).map(function(t, e) {
-                        return Object(F.jsx)(Nd, {
+                        return Object(F.jsx)(Vd, {
                             loading: !0
                         }, e)
                     }) : o && 0 < o.length ? (n = d, u().map(function(t) {
                         var e;
-                        return Object(F.jsx)(Nd, {
+                        return Object(F.jsx)(Vd, {
                             disabled: t.disabled,
                             size: null != (e = t.size) ? e : a.size,
                             value: t.value,
                             checked: l ? null == n ? void 0 : n.includes(t.value) : n === t.value,
                             onChange: t.onChange,
                             title: t.title,
                             avatar: t.avatar,
                             description: t.description,
                             cover: t.cover
                         }, t.value.toString())
                     })) : a.children
                 }, [u, i, l, o, a.children, a.size, d]),
                 t = Kt()(t, e);
-            return Object(F.jsx)(Rd.Provider, {
+            return Object(F.jsx)(Hd.Provider, {
                 value: {
                     toggleOption: function(e) {
                         var t, n, a, r;
                         l || (r = d === e.value ? void 0 : e.value, null == p) || p(r), l && (r = [], n = null == (t = d) ? void 0 : t.includes(e.value), r = Object(Ut.a)(t || []), n || r.push(e.value), n && (r = r.filter(function(t) {
                             return t !== e.value
                         })), a = u(), r = null == (t = r) || null == (n = t.filter(function(t) {
                             return f.current.has(t)
@@ -120776,16 +120918,16 @@
                 children: Object(F.jsx)("div", Object(Ct.a)(Object(Ct.a)({
                     className: t,
                     style: n
                 }, s), {}, {
                     children: c
                 }))
             })
-        }, Ld),
-        Yd = (Pd.propTypes = {
+        }, Rd),
+        Kd = (Id.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             checked: n.a.bool,
             defaultChecked: n.a.bool,
@@ -120798,22 +120940,22 @@
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func,
             persistence: n.a.oneOfType([n.a.bool, n.a.string, n.a.number]),
             persisted_props: n.a.arrayOf(n.a.oneOf(["checked"])),
             persistence_type: n.a.oneOf(["local", "session", "memory"])
-        }, Pd.defaultProps = {
+        }, Id.defaultProps = {
             bordered: !0,
             disabled: !1,
             size: "default",
             persisted_props: ["checked"],
             persistence_type: "local"
-        }, Pd),
-        Bd = (Dd.propTypes = {
+        }, Id),
+        Ud = (Nd.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             multiple: n.a.bool,
             bordered: n.a.bool,
@@ -120826,24 +120968,24 @@
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func,
             persistence: n.a.oneOfType([n.a.bool, n.a.string, n.a.number]),
             persisted_props: n.a.arrayOf(n.a.oneOf(["value"])),
             persistence_type: n.a.oneOf(["local", "session", "memory"])
-        }, Dd.defaultProps = {
+        }, Nd.defaultProps = {
             multiple: !1,
             bordered: !0,
             disabled: !1,
             size: "default",
             persisted_props: ["value"],
             persistence_type: "local"
-        }, Dd),
-        Fd = la.a.Panel,
-        Hd = (Td.propTypes = {
+        }, Nd),
+        Gd = ua.a.Panel,
+        qd = (Yd.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             items: n.a.arrayOf(n.a.exact({
                 children: n.a.node,
@@ -120865,77 +121007,77 @@
             ghost: n.a.bool,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, Td.defaultProps = {
+        }, Yd.defaultProps = {
             accordion: !0,
             bordered: !0,
             expandIconPosition: "left",
             ghost: !1
-        }, Td),
-        Wd = e(696),
-        Vd = e(68),
-        Kd = e(103),
-        Ud = e(81);
+        }, Yd),
+        Xd = e(696),
+        $d = e(68),
+        Zd = e(103),
+        Jd = e(81);
 
-    function Gd(t) {
+    function Qd(t) {
         var e = t.responseText || t.response;
         if (!e) return e;
         try {
             return JSON.parse(e)
         } catch (t) {
             return e
         }
     }
 
-    function qd(a) {
+    function tp(a) {
         var r = new XMLHttpRequest,
             n = (a.onProgress && r.upload && (r.upload.onprogress = function(t) {
                 0 < t.total && (t.percent = t.loaded / t.total * 100), a.onProgress(t)
             }), new FormData),
             e = (a.data && Object.keys(a.data).forEach(function(e) {
                 var t = a.data[e];
                 Array.isArray(t) ? t.forEach(function(t) {
                     n.append("".concat(e, "[]"), t)
                 }) : n.append(e, t)
             }), a.file instanceof Blob ? n.append(a.filename, a.file, a.file.name) : n.append(a.filename, a.file), r.onerror = function(t) {
                 a.onError(t)
             }, r.onload = function() {
-                return r.status < 200 || 300 <= r.status ? a.onError((e = r, n = "cannot ".concat((t = a).method, " ").concat(t.action, " ").concat(e.status, "'"), (n = new Error(n)).status = e.status, n.method = t.method, n.url = t.action, n), Gd(r)) : a.onSuccess(Gd(r), r);
+                return r.status < 200 || 300 <= r.status ? a.onError((e = r, n = "cannot ".concat((t = a).method, " ").concat(t.action, " ").concat(e.status, "'"), (n = new Error(n)).status = e.status, n.method = t.method, n.url = t.action, n), Qd(r)) : a.onSuccess(Qd(r), r);
                 var t, e, n
             }, r.open(a.method, a.action, !0), a.withCredentials && "withCredentials" in r && (r.withCredentials = !0), a.headers || {});
         return null !== e["X-Requested-With"] && r.setRequestHeader("X-Requested-With", "XMLHttpRequest"), Object.keys(e).forEach(function(t) {
             null !== e[t] && r.setRequestHeader(t, e[t])
         }), r.send(n), {
             abort: function() {
                 r.abort()
             }
         }
     }
-    var Xd = +new Date,
-        $d = 0;
+    var ep = +new Date,
+        np = 0;
 
-    function Zd() {
-        return "rc-upload-".concat(Xd, "-").concat(++$d)
+    function ap() {
+        return "rc-upload-".concat(ep, "-").concat(++np)
     }
 
-    function Jd(t, e) {
+    function rp(t, e) {
         var a, r, o;
         return !t || !e || (e = Array.isArray(e) ? e : e.split(","), a = t.name || "", r = t.type || "", o = r.replace(/\/.*$/, ""), e.some(function(t) {
             var e, n = t.trim();
             return !!/^\*(\/\*)?$/.test(t) || ("." === n.charAt(0) ? (e = a.toLowerCase(), (".jpg" !== (t = n.toLowerCase()) && ".jpeg" !== t ? [t] : [".jpg", ".jpeg"]).some(function(t) {
                 return e.endsWith(t)
-            })) : /\/\*$/.test(n) ? o === n.replace(/\/.*$/, "") : r === n || !!/^\w+$/.test(n) && (Object(de.a)(!1, "Upload takes an invalidate 'accept' type '".concat(n, "'.Skip for check.")), !0))
+            })) : /\/\*$/.test(n) ? o === n.replace(/\/.*$/, "") : r === n || !!/^\w+$/.test(n) && (Object(me.a)(!1, "Upload takes an invalidate 'accept' type '".concat(n, "'.Skip for check.")), !0))
         }))
     }
 
-    function Qd(t, e, o) {
+    function op(t, e, o) {
         function i(n, a) {
             var t, r;
             n.path = a || "", n.isFile ? n.file(function(t) {
                 o(t) && (n.fullPath && !t.webkitRelativePath && (Object.defineProperties(t, {
                     webkitRelativePath: {
                         writable: !0
                     }
@@ -120953,16 +121095,16 @@
                 })
             }())
         }
         t.forEach(function(t) {
             i(t.webkitGetAsEntry())
         })
     }
-    var tp, ep = ["component", "prefixCls", "className", "disabled", "id", "style", "multiple", "accept", "capture", "children", "directory", "openFileDialogOnClick", "onMouseEnter", "onMouseLeave"],
-        np = (p = Wt.Component, Object(r.a)(ap, p), tp = Object(o.a)(ap), Object(a.a)(ap, [{
+    var ip, lp = ["component", "prefixCls", "className", "disabled", "id", "style", "multiple", "accept", "capture", "children", "directory", "openFileDialogOnClick", "onMouseEnter", "onMouseLeave"],
+        cp = (p = Wt.Component, Object(r.a)(sp, p), ip = Object(o.a)(sp), Object(a.a)(sp, [{
             key: "componentDidMount",
             value: function() {
                 this._isMounted = !0
             }
         }, {
             key: "componentWillUnmount",
             value: function() {
@@ -120972,15 +121114,15 @@
             key: "post",
             value: function(t) {
                 var e, n, a, r, o, i, l = this,
                     c = t.data,
                     s = t.origin,
                     u = t.action,
                     d = t.parsedFile;
-                this._isMounted && (e = (t = this.props).onStart, i = t.customRequest, n = t.name, a = t.headers, r = t.withCredentials, t = t.method, o = s.uid, i = i || qd, u = {
+                this._isMounted && (e = (t = this.props).onStart, i = t.customRequest, n = t.name, a = t.headers, r = t.withCredentials, t = t.method, o = s.uid, i = i || tp, u = {
                     action: u,
                     filename: n,
                     data: c,
                     file: d,
                     headers: a,
                     withCredentials: r,
                     method: t || "post",
@@ -120998,15 +121140,15 @@
                     }
                 }, e(s), this.reqs[o] = i(u))
             }
         }, {
             key: "reset",
             value: function() {
                 this.setState({
-                    uid: Zd()
+                    uid: ap()
                 })
             }
         }, {
             key: "abort",
             value: function(t) {
                 var e = this.reqs;
                 t ? (t = t.uid || t, e[t] && e[t].abort && e[t].abort(), delete e[t]) : Object.keys(e).forEach(function(t) {
@@ -121027,15 +121169,15 @@
                     c = t.accept,
                     s = t.capture,
                     u = t.children,
                     d = t.directory,
                     p = t.openFileDialogOnClick,
                     f = t.onMouseEnter,
                     h = t.onMouseLeave,
-                    t = Object(Bt.a)(t, ep),
+                    t = Object(Jt.a)(t, lp),
                     n = Kt()((m = {}, Object(Vt.a)(m, n, !0), Object(Vt.a)(m, "".concat(n, "-disabled"), r), Object(Vt.a)(m, a, a), m)),
                     a = d ? {
                         directory: "directory",
                         webkitdirectory: "webkitdirectory"
                     } : {},
                     m = r ? {} : {
                         onClick: p ? this.onClick : function() {},
@@ -121046,15 +121188,15 @@
                         onDragOver: this.onFileDrop,
                         tabIndex: "0"
                     };
                 return H.a.createElement(e, Object(Et.a)({}, m, {
                     className: n,
                     role: "button",
                     style: i
-                }), H.a.createElement("input", Object(Et.a)({}, Object(Ud.a)(t, {
+                }), H.a.createElement("input", Object(Et.a)({}, Object(Jd.a)(t, {
                     aria: !0,
                     data: !0
                 }), {
                     id: o,
                     type: "file",
                     ref: this.saveFileInput,
                     onClick: function(t) {
@@ -121068,64 +121210,64 @@
                 }, a, {
                     multiple: l,
                     onChange: this.onChange
                 }, null != s ? {
                     capture: s
                 } : {})), u)
             }
-        }]), ap);
+        }]), sp);
 
-    function ap() {
+    function sp() {
         var u;
-        Object(i.a)(this, ap);
+        Object(i.a)(this, sp);
         for (var n, t = arguments.length, e = new Array(t), a = 0; a < t; a++) e[a] = arguments[a];
-        return (u = tp.call.apply(tp, [this].concat(e))).state = {
-            uid: Zd()
+        return (u = ip.call.apply(ip, [this].concat(e))).state = {
+            uid: ap()
         }, u.reqs = {}, u.fileInput = void 0, u._isMounted = void 0, u.onChange = function(t) {
             var e = u.props,
                 n = e.accept,
                 a = e.directory,
                 e = t.target.files,
                 t = Object(Ut.a)(e).filter(function(t) {
-                    return !a || Jd(t, n)
+                    return !a || rp(t, n)
                 });
             u.uploadFiles(t), u.reset()
         }, u.onClick = function(t) {
             var e, n, a = u.fileInput;
             a && (n = (e = u.props).children, e = e.onClick, n && "button" === n.type && ((n = a.parentNode).focus(), n.querySelector("button").blur()), a.click(), e) && e(t)
         }, u.onKeyDown = function(t) {
             "Enter" === t.key && u.onClick(t)
         }, u.onFileDrop = function(t) {
             var e = u.props.multiple;
-            t.preventDefault(), "dragover" !== t.type && (u.props.directory ? Qd(Array.prototype.slice.call(t.dataTransfer.items), u.uploadFiles, function(t) {
-                return Jd(t, u.props.accept)
+            t.preventDefault(), "dragover" !== t.type && (u.props.directory ? op(Array.prototype.slice.call(t.dataTransfer.items), u.uploadFiles, function(t) {
+                return rp(t, u.props.accept)
             }) : (t = Object(Ut.a)(t.dataTransfer.files).filter(function(t) {
-                return Jd(t, u.props.accept)
+                return rp(t, u.props.accept)
             }), !1 === e && (t = t.slice(0, 1)), u.uploadFiles(t)))
         }, u.uploadFiles = function(t) {
             var e = Object(Ut.a)(t),
                 t = e.map(function(t) {
-                    return t.uid = Zd(), u.processFile(t, e)
+                    return t.uid = ap(), u.processFile(t, e)
                 });
             Promise.all(t).then(function(t) {
                 var e = u.props.onBatchStart;
                 null != e && e(t.map(function(t) {
                     return {
                         file: t.origin,
                         parsedFile: t.parsedFile
                     }
                 })), t.filter(function(t) {
                     return null !== t.parsedFile
                 }).forEach(function(t) {
                     u.post(t)
                 })
             })
-        }, u.processFile = (n = Object(Kd.a)(Object(Vd.a)().mark(function t(e, n) {
+        }, u.processFile = (n = Object(Zd.a)(Object($d.a)().mark(function t(e, n) {
             var a, r, o, i, l, c, s;
-            return Object(Vd.a)().wrap(function(t) {
+            return Object($d.a)().wrap(function(t) {
                 for (;;) switch (t.prev = t.next) {
                     case 0:
                         if (c = u.props.beforeUpload, a = e, c) return t.prev = 3, t.next = 6, c(e, n);
                         t.next = 14;
                         break;
                     case 6:
                         a = t.sent, t.next = 12;
@@ -121178,78 +121320,78 @@
         })), function(t, e) {
             return n.apply(this, arguments)
         }), u.saveFileInput = function(t) {
             u.fileInput = t
         }, u
     }
 
-    function rp() {}
-    l = Wt.Component, Object(r.a)(ip, l), op = Object(o.a)(ip), Object(a.a)(ip, [{
+    function up() {}
+    l = Wt.Component, Object(r.a)(pp, l), dp = Object(o.a)(pp), Object(a.a)(pp, [{
         key: "abort",
         value: function(t) {
             this.uploader.abort(t)
         }
     }, {
         key: "render",
         value: function() {
-            return H.a.createElement(np, Object(Et.a)({}, this.props, {
+            return H.a.createElement(cp, Object(Et.a)({}, this.props, {
                 ref: this.saveUploader
             }))
         }
     }]);
-    var op, c = ip;
+    var dp, c = pp;
 
-    function ip() {
+    function pp() {
         var e;
-        Object(i.a)(this, ip);
+        Object(i.a)(this, pp);
         for (var t = arguments.length, n = new Array(t), a = 0; a < t; a++) n[a] = arguments[a];
-        return (e = op.call.apply(op, [this].concat(n))).uploader = void 0, e.saveUploader = function(t) {
+        return (e = dp.call.apply(dp, [this].concat(n))).uploader = void 0, e.saveUploader = function(t) {
             e.uploader = t
         }, e
     }
     c.defaultProps = {
         component: "span",
         prefixCls: "rc-upload",
         data: {},
         headers: {},
         name: "file",
         multipart: !1,
-        onStart: rp,
-        onError: rp,
-        onSuccess: rp,
+        onStart: up,
+        onError: up,
+        onSuccess: up,
         multiple: !1,
         beforeUpload: null,
         customRequest: null,
         withCredentials: !1,
         openFileDialogOnClick: !0
     };
 
-    function lp(t, e) {
-        return Wt.createElement(to.a, Object(Ct.a)(Object(Ct.a)({}, t), {}, {
+    function fp(t, e) {
+        return Wt.createElement(ao.a, Object(Ct.a)(Object(Ct.a)({}, t), {}, {
             ref: e,
-            icon: pp
+            icon: vp
         }))
     }
 
-    function cp(t, e) {
-        return Wt.createElement(to.a, Object(Ct.a)(Object(Ct.a)({}, t), {}, {
+    function hp(t, e) {
+        return Wt.createElement(ao.a, Object(Ct.a)(Object(Ct.a)({}, t), {}, {
             ref: e,
-            icon: hp
+            icon: xp
         }))
     }
 
-    function sp(t, e) {
-        return Wt.createElement(to.a, Object(Ct.a)(Object(Ct.a)({}, t), {}, {
+    function mp(t, e) {
+        return Wt.createElement(ao.a, Object(Ct.a)(Object(Ct.a)({}, t), {}, {
             ref: e,
-            icon: gp
+            icon: Op
         }))
     }
-    var up = c,
-        dp = e(70),
-        pp = {
+    var gp = c,
+        bp = e(70),
+        vp = {
             icon: function(t, e) {
                 return {
                     tag: "svg",
                     attrs: {
                         viewBox: "64 64 896 896",
                         focusable: "false"
                     },
@@ -121267,16 +121409,16 @@
                         }
                     }]
                 }
             },
             name: "file",
             theme: "twotone"
         },
-        fp = (lp.displayName = "FileTwoTone", Wt.forwardRef(lp)),
-        hp = {
+        yp = (fp.displayName = "FileTwoTone", Wt.forwardRef(fp)),
+        xp = {
             icon: {
                 tag: "svg",
                 attrs: {
                     viewBox: "64 64 896 896",
                     focusable: "false"
                 },
                 children: [{
@@ -121285,16 +121427,16 @@
                         d: "M779.3 196.6c-94.2-94.2-247.6-94.2-341.7 0l-261 260.8c-1.7 1.7-2.6 4-2.6 6.4s.9 4.7 2.6 6.4l36.9 36.9a9 9 0 0012.7 0l261-260.8c32.4-32.4 75.5-50.2 121.3-50.2s88.9 17.8 121.2 50.2c32.4 32.4 50.2 75.5 50.2 121.2 0 45.8-17.8 88.8-50.2 121.2l-266 265.9-43.1 43.1c-40.3 40.3-105.8 40.3-146.1 0-19.5-19.5-30.2-45.4-30.2-73s10.7-53.5 30.2-73l263.9-263.8c6.7-6.6 15.5-10.3 24.9-10.3h.1c9.4 0 18.1 3.7 24.7 10.3 6.7 6.7 10.3 15.5 10.3 24.9 0 9.3-3.7 18.1-10.3 24.7L372.4 653c-1.7 1.7-2.6 4-2.6 6.4s.9 4.7 2.6 6.4l36.9 36.9a9 9 0 0012.7 0l215.6-215.6c19.9-19.9 30.8-46.3 30.8-74.4s-11-54.6-30.8-74.4c-41.1-41.1-107.9-41-149 0L463 364 224.8 602.1A172.22 172.22 0 00174 724.8c0 46.3 18.1 89.8 50.8 122.5 33.9 33.8 78.3 50.7 122.7 50.7 44.4 0 88.8-16.9 122.6-50.7l309.2-309C824.8 492.7 850 432 850 367.5c.1-64.6-25.1-125.3-70.7-170.9z"
                     }
                 }]
             },
             name: "paper-clip",
             theme: "outlined"
         },
-        mp = (cp.displayName = "PaperClipOutlined", Wt.forwardRef(cp)),
-        gp = {
+        _p = (hp.displayName = "PaperClipOutlined", Wt.forwardRef(hp)),
+        Op = {
             icon: function(t, e) {
                 return {
                     tag: "svg",
                     attrs: {
                         viewBox: "64 64 896 896",
                         focusable: "false"
                     },
@@ -121330,75 +121472,75 @@
                         }
                     }]
                 }
             },
             name: "picture",
             theme: "twotone"
         },
-        bp = (sp.displayName = "PictureTwoTone", Wt.forwardRef(sp));
+        wp = (mp.displayName = "PictureTwoTone", Wt.forwardRef(mp));
 
-    function vp(t) {
+    function kp(t) {
         return Object(Et.a)(Object(Et.a)({}, t), {
             lastModified: t.lastModified,
             lastModifiedDate: t.lastModifiedDate,
             name: t.name,
             size: t.size,
             type: t.type,
             uid: t.uid,
             percent: 0,
             originFileObj: t
         })
     }
 
-    function yp(e, t) {
+    function jp(e, t) {
         var t = Object(Ut.a)(t),
             n = t.findIndex(function(t) {
                 return t.uid === e.uid
             });
         return -1 === n ? t.push(e) : t[n] = e, t
     }
 
-    function xp(e, t) {
+    function Mp(e, t) {
         var n = void 0 !== e.uid ? "uid" : "name";
         return t.filter(function(t) {
             return t[n] === e[n]
         })[0]
     }
 
-    function _p(t) {
+    function Ep(t) {
         var e;
-        return t.type && !t.thumbUrl ? Op(t.type) : (e = function(t) {
+        return t.type && !t.thumbUrl ? Cp(t.type) : (e = function(t) {
             t = (0 < arguments.length && void 0 !== t ? t : "").split("/"), t = t[t.length - 1].split(/#|\?/)[0];
             return (/\.[^./\\]*$/.exec(t) || [""])[0]
         }(t = t.thumbUrl || t.url || ""), !(!/^data:image\//.test(t) && !/(webp|svg|png|gif|jpg|jpeg|jfif|bmp|dpg|ico|heic|heif)$/i.test(e)) || !/^data:/.test(t) && !e)
     }
-    var Op = function(t) {
+    var Cp = function(t) {
         return 0 === t.indexOf("image/")
     };
 
-    function wp(e) {
+    function Sp(e) {
         return new Promise(function(i) {
             var l, c, s, t;
-            e.type && Op(e.type) ? ((l = document.createElement("canvas")).width = 200, l.height = 200, l.style.cssText = "position: fixed; left: 0; top: 0; width: ".concat(200, "px; height: ").concat(200, "px; z-index: 9999; display: none;"), document.body.appendChild(l), c = l.getContext("2d"), (s = new Image).onload = function() {
+            e.type && Cp(e.type) ? ((l = document.createElement("canvas")).width = 200, l.height = 200, l.style.cssText = "position: fixed; left: 0; top: 0; width: ".concat(200, "px; height: ").concat(200, "px; z-index: 9999; display: none;"), document.body.appendChild(l), c = l.getContext("2d"), (s = new Image).onload = function() {
                 var t = s.width,
                     e = s.height,
                     n = 200,
                     a = 200,
                     r = 0,
                     o = 0,
                     t = (e < t ? o = -((a = e * (200 / t)) - n) / 2 : r = -((n = t * (200 / e)) - a) / 2, c.drawImage(s, r, o, n, a), l.toDataURL());
                 document.body.removeChild(l), i(t)
             }, s.crossOrigin = "anonymous", e.type.startsWith("image/svg+xml") ? ((t = new FileReader).addEventListener("load", function() {
                 t.result && (s.src = t.result)
             }), t.readAsDataURL(e)) : s.src = window.URL.createObjectURL(e)) : i("")
         })
     }
-    var kp = e(532),
-        jp = e(194),
-        Mp = Wt.forwardRef(function(t, e) {
+    var Lp = e(532),
+        Pp = e(194),
+        Dp = Wt.forwardRef(function(t, e) {
             var n = t.prefixCls,
                 a = t.className,
                 r = t.style,
                 o = t.locale,
                 i = t.listType,
                 l = t.file,
                 c = t.items,
@@ -121454,18 +121596,18 @@
                 },
                 href: l.url || l.thumbUrl,
                 target: "_blank",
                 rel: "noopener noreferrer"
             }, L)));
             var f = Kt()((u = {}, Object(Vt.a)(u, "".concat(n, "-list-item"), !0), Object(Vt.a)(u, "".concat(n, "-list-item-").concat(k), !0), Object(Vt.a)(u, "".concat(n, "-list-item-list-type-").concat(i), !0), u)),
                 L = "string" == typeof l.linkProps ? JSON.parse(l.linkProps) : l.linkProps,
-                u = m ? d(("function" == typeof v ? v(l) : v) || Wt.createElement(Ee.a, null), function() {
+                u = m ? d(("function" == typeof v ? v(l) : v) || Wt.createElement(Le.a, null), function() {
                     return O(l)
                 }, n, o.removeFile) : null,
-                m = g && "done" === k ? d(("function" == typeof y ? y(l) : y) || Wt.createElement(kp.a, null), function() {
+                m = g && "done" === k ? d(("function" == typeof y ? y(l) : y) || Wt.createElement(Lp.a, null), function() {
                     return _(l)
                 }, n, o.downloadFile) : null,
                 v = "picture-card" !== i && Wt.createElement("span", {
                     key: "download-delete",
                     className: Kt()("".concat(n, "-list-item-card-actions"), {
                         picture: "picture" === i
                     })
@@ -121498,34 +121640,34 @@
                         pointerEvents: "none",
                         opacity: .5
                     },
                     onClick: function(t) {
                         return x(l, t)
                     },
                     title: o.previewFile
-                }, "function" == typeof b ? b(l) : b || Wt.createElement(jp.a, null)) : null,
+                }, "function" == typeof b ? b(l) : b || Wt.createElement(Pp.a, null)) : null,
                 L = "picture-card" === i && "uploading" !== k && Wt.createElement("span", {
                     className: "".concat(n, "-list-item-actions")
                 }, y, "done" === k && m, u),
                 h = l.response && "string" == typeof l.response ? l.response : (null == (g = l.error) ? void 0 : g.statusText) || (null == (v = l.error) ? void 0 : v.message) || o.uploadError,
                 b = Wt.createElement("span", {
                     className: t
                 }, S, d),
                 y = (0, Wt.useContext(q.b).getPrefixCls)(),
                 m = Wt.createElement("div", {
                     className: f
                 }, Wt.createElement("div", {
                     className: "".concat(n, "-list-item-info")
-                }, b), L, M && Wt.createElement(Er.b, {
+                }, b), L, M && Wt.createElement(Lr.b, {
                     motionName: "".concat(y, "-fade"),
                     visible: "uploading" === k,
                     motionDeadline: 2e3
                 }, function(t) {
                     var t = t.className,
-                        e = "percent" in l ? Wt.createElement(kn, Object(Et.a)({}, s, {
+                        e = "percent" in l ? Wt.createElement(En, Object(Et.a)({}, s, {
                             type: "line",
                             percent: l.percent
                         })) : null;
                     return Wt.createElement("div", {
                         className: Kt()("".concat(n, "-list-item-progress"), t)
                     }, e)
                 })),
@@ -121542,59 +121684,59 @@
                 ref: e
             }, p ? p(g, l, c, {
                 download: _.bind(null, l),
                 preview: x.bind(null, l),
                 remove: O.bind(null, l)
             }) : g)
         }),
-        Ep = Object(Et.a)({}, Va.a),
-        Cp = (delete Ep.onAppearEnd, delete Ep.onEnterEnd, delete Ep.onLeaveEnd, Wt.forwardRef(function(t, e) {
+        Tp = Object(Et.a)({}, Ga.a),
+        zp = (delete Tp.onAppearEnd, delete Tp.onEnterEnd, delete Tp.onLeaveEnd, Wt.forwardRef(function(t, e) {
             function r(t, e) {
                 if (u) return null != e && e.preventDefault(), u(t)
             }
 
             function o(t) {
                 "function" == typeof d ? d(t) : t.url && window.open(t.url)
             }
 
             function i(t) {
                 null != p && p(t)
             }
 
             function l(t) {
                 var e, n;
-                return h ? h(t, s) : (e = "uploading" === t.status, t = m && m(t) ? Wt.createElement(bp, null) : Wt.createElement(fp, null), n = e ? Wt.createElement(oo.a, null) : Wt.createElement(mp, null), "picture" === s ? n = e ? Wt.createElement(oo.a, null) : t : "picture-card" === s && (n = e ? f.uploading : t), n)
+                return h ? h(t, s) : (e = "uploading" === t.status, t = m && m(t) ? Wt.createElement(wp, null) : Wt.createElement(yp, null), n = e ? Wt.createElement(co.a, null) : Wt.createElement(_p, null), "picture" === s ? n = e ? Wt.createElement(co.a, null) : t : "picture-card" === s && (n = e ? f.uploading : t), n)
             }
 
             function c(e, n, t, a) {
                 return a = {
                     type: "text",
                     size: "small",
                     title: a,
                     onClick: function(t) {
-                        n(), Object(je.c)(e) && e.props.onClick && e.props.onClick(t)
+                        n(), Object(Ce.c)(e) && e.props.onClick && e.props.onClick(t)
                     },
                     className: "".concat(t, "-list-item-card-actions-btn")
-                }, Object(je.c)(e) ? (t = Object(je.a)(e, Object(Et.a)(Object(Et.a)({}, e.props), {
+                }, Object(Ce.c)(e) ? (t = Object(Ce.a)(e, Object(Et.a)(Object(Et.a)({}, e.props), {
                     onClick: function() {}
                 })), Wt.createElement(z.a, Object(Et.a)({}, a, {
                     icon: t
                 }))) : Wt.createElement(z.a, Object(Et.a)({}, a), Wt.createElement("span", null, e))
             }
             var n = t.listType,
                 s = void 0 === n ? "text" : n,
                 n = t.previewFile,
-                a = void 0 === n ? wp : n,
+                a = void 0 === n ? Sp : n,
                 u = t.onPreview,
                 d = t.onDownload,
                 p = t.onRemove,
                 f = t.locale,
                 h = t.iconRender,
                 n = t.isImageUrl,
-                m = void 0 === n ? _p : n,
+                m = void 0 === n ? Ep : n,
                 n = t.prefixCls,
                 g = t.items,
                 b = void 0 === g ? [] : g,
                 g = t.showPreviewIcon,
                 v = void 0 === g || g,
                 g = t.showRemoveIcon,
                 y = void 0 === g || g,
@@ -121608,15 +121750,15 @@
                     strokeWidth: 2,
                     showInfo: !1
                 } : g,
                 j = t.appendAction,
                 g = t.appendActionVisible,
                 g = void 0 === g || g,
                 M = t.itemRender,
-                E = Object(hc.a)(),
+                E = Object(xc.a)(),
                 t = Wt.useState(!1),
                 t = Object(Gt.a)(t, 2),
                 C = t[0],
                 S = t[1],
                 t = (Wt.useEffect(function() {
                     "picture" !== s && "picture-card" !== s || (b || []).forEach(function(e) {
                         "undefined" != typeof document && "undefined" != typeof window && window.FileReader && window.File && (e.originFileObj instanceof File || e.originFileObj instanceof Blob) && void 0 === e.thumbUrl && (e.thumbUrl = "", a) && a(e.originFileObj).then(function(t) {
@@ -121644,24 +121786,24 @@
                 e = "picture-card" === s ? "animate-inline" : "animate",
                 e = {
                     motionDeadline: 2e3,
                     motionName: "".concat(L, "-").concat(e),
                     keys: t,
                     motionAppear: C
                 };
-            return "picture-card" !== s && (e = Object(Et.a)(Object(Et.a)({}, Ep), e)), Wt.createElement("div", {
+            return "picture-card" !== s && (e = Object(Et.a)(Object(Et.a)({}, Tp), e)), Wt.createElement("div", {
                 className: n
-            }, Wt.createElement(Er.a, Object(Et.a)({}, e, {
+            }, Wt.createElement(Lr.a, Object(Et.a)({}, e, {
                 component: !1
             }), function(t) {
                 var e = t.key,
                     n = t.file,
                     a = t.className,
                     t = t.style;
-                return Wt.createElement(Mp, {
+                return Wt.createElement(Dp, {
                     key: e,
                     locale: f,
                     prefixCls: L,
                     className: a,
                     style: t,
                     file: n,
                     items: b,
@@ -121677,40 +121819,40 @@
                     iconRender: l,
                     actionIconRender: c,
                     itemRender: M,
                     onPreview: r,
                     onDownload: o,
                     onClose: i
                 })
-            }), j && Wt.createElement(Er.b, Object(Et.a)({}, e, {
+            }), j && Wt.createElement(Lr.b, Object(Et.a)({}, e, {
                 visible: g,
                 forceRender: !0
             }), function(t) {
                 var e = t.className,
                     n = t.style;
-                return Object(je.a)(j, function(t) {
+                return Object(Ce.a)(j, function(t) {
                     return {
                         className: Kt()(t.className, e),
                         style: Object(Et.a)(Object(Et.a)(Object(Et.a)({}, n), {
                             pointerEvents: e ? "none" : void 0
                         }), t.style)
                     }
                 })
             }))
         })),
-        Sp = "__LIST_IGNORE_".concat(Date.now(), "__"),
-        Lp = Wt.forwardRef(function(u, t) {
+        Ap = "__LIST_IGNORE_".concat(Date.now(), "__"),
+        Rp = Wt.forwardRef(function(u, t) {
             function e(t) {
                 var r, o = t.filter(function(t) {
-                    return !t.file[Sp]
+                    return !t.file[Ap]
                 });
                 o.length && (t = o.map(function(t) {
-                    return vp(t.file)
+                    return kp(t.file)
                 }), r = Object(Ut.a)(D), t.forEach(function(t) {
-                    r = yp(t, r)
+                    r = jp(t, r)
                 }), t.forEach(function(t, e) {
                     var n = t;
                     if (o[e].parsedFile) t.status = "uploading";
                     else {
                         var a, e = t.originFileObj;
                         try {
                             a = new File([e], e.name, {
@@ -121727,24 +121869,24 @@
                 }))
             }
 
             function n(t, e, n) {
                 try {
                     "string" == typeof t && (t = JSON.parse(t))
                 } catch (t) {}
-                xp(e, D) && ((e = vp(e)).status = "done", e.percent = 100, e.response = t, e.xhr = n, n = yp(e, D), z(e, n))
+                Mp(e, D) && ((e = kp(e)).status = "done", e.percent = 100, e.response = t, e.xhr = n, n = jp(e, D), z(e, n))
             }
 
             function a(t, e) {
                 var n;
-                xp(e, D) && ((e = vp(e)).status = "uploading", e.percent = t.percent, n = yp(e, D), z(e, n, t))
+                Mp(e, D) && ((e = kp(e)).status = "uploading", e.percent = t.percent, n = jp(e, D), z(e, n, t))
             }
 
             function r(t, e, n) {
-                xp(n, D) && ((n = vp(n)).error = t, n.response = e, n.status = "error", t = yp(n, D), z(n, t))
+                Mp(n, D) && ((n = kp(n)).error = t, n.response = e, n.status = "error", t = jp(n, D), z(n, t))
             }
 
             function s(r) {
                 var o;
                 Promise.resolve("function" == typeof d ? d(r) : d).then(function(t) {
                     var e, n, a;
                     !1 !== t && (t = D, n = void 0 !== (e = r).uid ? "uid" : "name", t = (a = t.filter(function(t) {
@@ -121759,26 +121901,26 @@
             }
 
             function o(t) {
                 W(t.type), "drop" !== t.type || null != v && v(t)
             }
 
             function i(l, c) {
-                return f ? Wt.createElement(ye.a, {
+                return f ? Wt.createElement(we.a, {
                     componentName: "Upload",
-                    defaultLocale: xe.a.Upload
+                    defaultLocale: ke.a.Upload
                 }, function(t) {
                     var e = "boolean" == typeof f ? {} : f,
                         n = e.showRemoveIcon,
                         a = e.showPreviewIcon,
                         r = e.showDownloadIcon,
                         o = e.removeIcon,
                         i = e.previewIcon,
                         e = e.downloadIcon;
-                    return Wt.createElement(Cp, {
+                    return Wt.createElement(zp, {
                         prefixCls: A,
                         listType: h,
                         items: D,
                         previewFile: y,
                         onPreview: m,
                         onDownload: g,
                         onRemove: s,
@@ -121829,17 +121971,17 @@
                 M = void 0 !== M && M,
                 E = u.action,
                 E = void 0 === E ? "" : E,
                 C = u.accept,
                 C = void 0 === C ? "" : C,
                 S = u.supportServerRender,
                 S = void 0 === S || S,
-                L = Wt.useContext(pi.b),
+                L = Wt.useContext(mi.b),
                 P = null != p ? p : L,
-                p = Object($t.a)(c || [], {
+                p = Object(Zt.a)(c || [], {
                     value: l,
                     postState: function(t) {
                         return null != t ? t : []
                     }
                 }),
                 L = Object(Gt.a)(p, 2),
                 D = L[0],
@@ -121852,15 +121994,15 @@
                 z = (Wt.useMemo(function() {
                     var n = Date.now();
                     (l || []).forEach(function(t, e) {
                         t.uid || Object.isFrozen(t) || (t.uid = "__AUTO__".concat(n, "_").concat(e, "__"))
                     })
                 }, [l]), function(t, e, n) {
                     var a = Object(Ut.a)(e),
-                        e = (1 === k ? a = a.slice(-1) : k && (a = a.slice(0, k)), Object(dp.flushSync)(function() {
+                        e = (1 === k ? a = a.slice(-1) : k && (a = a.slice(0, k)), Object(bp.flushSync)(function() {
                             H(a)
                         }), {
                             file: t,
                             fileList: a
                         });
                     n && (e.event = n), null != b && b(e)
                 }),
@@ -121887,28 +122029,28 @@
                     multiple: M,
                     action: E,
                     accept: C,
                     supportServerRender: S,
                     prefixCls: A,
                     disabled: P,
                     beforeUpload: function(o, i) {
-                        return c = l = t = void 0, s = Object(Vd.a)().mark(function t() {
+                        return c = l = t = void 0, s = Object($d.a)().mark(function t() {
                             var e, n, a, r;
-                            return Object(Vd.a)().wrap(function(t) {
+                            return Object($d.a)().wrap(function(t) {
                                 for (;;) switch (t.prev = t.next) {
                                     case 0:
                                         if (e = u.beforeUpload, n = u.transformFile, a = o, e) return t.next = 5, e(o, i);
                                         t.next = 13;
                                         break;
                                     case 5:
                                         if (!1 === (r = t.sent)) return t.abrupt("return", !1);
                                         t.next = 8;
                                         break;
                                     case 8:
-                                        if (delete o[Sp], r === Sp) return Object.defineProperty(o, Sp, {
+                                        if (delete o[Ap], r === Ap) return Object.defineProperty(o, Ap, {
                                             value: !0,
                                             configurable: !0
                                         }), t.abrupt("return", !1);
                                         t.next = 12;
                                         break;
                                     case 12:
                                         "object" === Object(qt.a)(r) && r && (a = r);
@@ -121959,25 +122101,25 @@
                 return "uploading" === t.status
             })), Object(Vt.a)(p, "".concat(A, "-drag-hover"), "dragover" === L), Object(Vt.a)(p, "".concat(A, "-disabled"), P), Object(Vt.a)(p, "".concat(A, "-rtl"), "rtl" === t), p), _), Wt.createElement("span", null, Wt.createElement("div", {
                 className: x,
                 onDrop: o,
                 onDragOver: o,
                 onDragLeave: o,
                 style: B
-            }, Wt.createElement(up, Object(Et.a)({}, c, {
+            }, Wt.createElement(gp, Object(Et.a)({}, c, {
                 ref: T,
                 className: "".concat(A, "-btn")
             }), Wt.createElement("div", {
                 className: "".concat(A, "-drag-container")
             }, w))), i())) : (M = Kt()(A, (j = {}, Object(Vt.a)(j, "".concat(A, "-select"), !0), Object(Vt.a)(j, "".concat(A, "-select-").concat(h), !0), Object(Vt.a)(j, "".concat(A, "-disabled"), P), Object(Vt.a)(j, "".concat(A, "-rtl"), "rtl" === t), j)), E = Wt.createElement("div", {
                 className: M,
                 style: w ? void 0 : {
                     display: "none"
                 }
-            }, Wt.createElement(up, Object(Et.a)({}, c, {
+            }, Wt.createElement(gp, Object(Et.a)({}, c, {
                 ref: T
             }))), "picture-card" === h ? Wt.createElement("span", {
                 className: Kt()("".concat(A, "-picture-card-wrapper"), _)
             }, i(E, !!w)) : Wt.createElement("span", {
                 className: _
             }, E, i()))
         }),
@@ -121987,131 +122129,131 @@
                 t = function(t, e) {
                     var n = {};
                     for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
                     if (null != t && "function" == typeof Object.getOwnPropertySymbols)
                         for (var a = 0, r = Object.getOwnPropertySymbols(t); a < r.length; a++) e.indexOf(r[a]) < 0 && Object.prototype.propertyIsEnumerable.call(t, r[a]) && (n[r[a]] = t[r[a]]);
                     return n
                 }(t, ["style", "height"]);
-            return Wt.createElement(Lp, Object(Et.a)({
+            return Wt.createElement(Rp, Object(Et.a)({
                 ref: e
             }, t, {
                 type: "drag",
                 style: Object(Et.a)(Object(Et.a)({}, n), {
                     height: a
                 })
             }))
         }),
-        p = Lp,
-        Pp = (p.Dragger = d, p.LIST_IGNORE = Sp, p),
-        Dp = e(536),
-        Tp = e(3);
-    const zp = /^[v^~<>=]*?(\d+)(?:\.([x*]|\d+)(?:\.([x*]|\d+)(?:\.([x*]|\d+))?(?:-([\da-z\-]+(?:\.[\da-z\-]+)*))?(?:\+[\da-z\-]+(?:\.[\da-z\-]+)*)?)?)?$/i,
-        Ap = t => {
+        p = Rp,
+        Ip = (p.Dragger = d, p.LIST_IGNORE = Ap, p),
+        Np = e(536),
+        Yp = e(3);
+    const Bp = /^[v^~<>=]*?(\d+)(?:\.([x*]|\d+)(?:\.([x*]|\d+)(?:\.([x*]|\d+))?(?:-([\da-z\-]+(?:\.[\da-z\-]+)*))?(?:\+[\da-z\-]+(?:\.[\da-z\-]+)*)?)?)?$/i,
+        Fp = t => {
             if ("string" != typeof t) throw new TypeError("Invalid argument expected string");
-            var e = t.match(zp);
+            var e = t.match(Bp);
             if (e) return e.shift(), e;
             throw new Error(`Invalid argument not valid semver ('${t}' received)`)
         },
-        Rp = t => "*" === t || "x" === t || "X" === t,
-        Ip = t => {
+        Hp = t => "*" === t || "x" === t || "X" === t,
+        Wp = t => {
             var e = parseInt(t, 10);
             return isNaN(e) ? t : e
         },
-        Np = (t, e) => {
-            return Rp(t) || Rp(e) ? 0 : ([t, e] = (t = Ip(t), e = Ip(e), typeof t != typeof e ? [String(t), String(e)] : [t, e]), e < t ? 1 : t < e ? -1 : 0)
+        Vp = (t, e) => {
+            return Hp(t) || Hp(e) ? 0 : ([t, e] = (t = Wp(t), e = Wp(e), typeof t != typeof e ? [String(t), String(e)] : [t, e]), e < t ? 1 : t < e ? -1 : 0)
         },
-        Yp = (e, n) => {
+        Kp = (e, n) => {
             for (let t = 0; t < Math.max(e.length, n.length); t++) {
-                var a = Np(e[t] || "0", n[t] || "0");
+                var a = Vp(e[t] || "0", n[t] || "0");
                 if (0 !== a) return a
             }
             return 0
         };
     Object.keys({
         ">": [1],
         ">=": [0, 1],
         "=": [0],
         "<=": [-1, 0],
         "<": [-1]
     });
-    var Bp = function(t, e) {
-            return (Bp = Object.setPrototypeOf || ({
+    var Up = function(t, e) {
+            return (Up = Object.setPrototypeOf || ({
                     __proto__: []
                 }
                 instanceof Array ? function(t, e) {
                     t.__proto__ = e
                 } : function(t, e) {
                     for (var n in e) Object.prototype.hasOwnProperty.call(e, n) && (t[n] = e[n])
                 }))(t, e)
         },
-        Fp = function() {
-            return (Fp = Object.assign || function(t) {
+        Gp = function() {
+            return (Gp = Object.assign || function(t) {
                 for (var e, n = 1, a = arguments.length; n < a; n++)
                     for (var r in e = arguments[n]) Object.prototype.hasOwnProperty.call(e, r) && (t[r] = e[r]);
                 return t
             }).apply(this, arguments)
         },
         r = (Object.create, Object.create, e(520)),
-        Hp = e.n(r);
+        qp = e.n(r);
 
-    function Wp(t, e, n, a, r) {
-        e = $p(e.width, e.height, r = void 0 === r ? 0 : r), r = e.width, e = e.height;
+    function Xp(t, e, n, a, r) {
+        e = nf(e.width, e.height, r = void 0 === r ? 0 : r), r = e.width, e = e.height;
         return {
-            x: Vp(t.x, r, n.width, a),
-            y: Vp(t.y, e, n.height, a)
+            x: $p(t.x, r, n.width, a),
+            y: $p(t.y, e, n.height, a)
         }
     }
 
-    function Vp(t, e, n, a) {
+    function $p(t, e, n, a) {
         e = e * a / 2 - n / 2;
-        return Zp(t, -e, e)
+        return af(t, -e, e)
     }
 
-    function Kp(t, e) {
+    function Zp(t, e) {
         return Math.sqrt(Math.pow(t.y - e.y, 2) + Math.pow(t.x - e.x, 2))
     }
 
-    function Up(t, e) {
+    function Jp(t, e) {
         return 180 * Math.atan2(e.y - t.y, e.x - t.x) / Math.PI
     }
 
-    function Gp(t, e) {
+    function Qp(t, e) {
         return Math.min(t, Math.max(0, e))
     }
 
-    function qp(t, e) {
+    function tf(t, e) {
         return e
     }
 
-    function Xp(t, e) {
+    function ef(t, e) {
         return {
             x: (e.x + t.x) / 2,
             y: (e.y + t.y) / 2
         }
     }
 
-    function $p(t, e, n) {
+    function nf(t, e, n) {
         n = n * Math.PI / 180;
         return {
             width: Math.abs(Math.cos(n) * t) + Math.abs(Math.sin(n) * e),
             height: Math.abs(Math.sin(n) * t) + Math.abs(Math.cos(n) * e)
         }
     }
 
-    function Zp(t, e, n) {
+    function af(t, e, n) {
         return Math.min(Math.max(t, e), n)
     }
 
-    function Jp() {
+    function rf() {
         for (var t = [], e = 0; e < arguments.length; e++) t[e] = arguments[e];
         return t.filter(function(t) {
             return "string" == typeof t && 0 < t.length
         }).join(" ").trim()
     }
-    Qp = H.a.Component, Bp(tf = f, l = Qp), tf.prototype = null === l ? Object.create(l) : (nf.prototype = l.prototype, new nf), f.prototype.componentDidMount = function() {
+    of = H.a.Component, Up(lf = f, l = of), lf.prototype = null === l ? Object.create(l) : (sf.prototype = l.prototype, new sf), f.prototype.componentDidMount = function() {
         this.currentDoc && this.currentWindow && (this.containerRef && (this.containerRef.ownerDocument && (this.currentDoc = this.containerRef.ownerDocument), this.currentDoc.defaultView && (this.currentWindow = this.currentDoc.defaultView), this.initResizeObserver(), void 0 === window.ResizeObserver && this.currentWindow.addEventListener("resize", this.computeSizes), this.props.zoomWithScroll && this.containerRef.addEventListener("wheel", this.onWheel, {
             passive: !1
         }), this.containerRef.addEventListener("gesturestart", this.onGestureStart)), this.props.disableAutomaticStylesInjection || (this.styleRef = this.currentDoc.createElement("style"), this.styleRef.setAttribute("type", "text/css"), this.props.nonce && this.styleRef.setAttribute("nonce", this.props.nonce), this.styleRef.innerHTML = ".reactEasyCrop_Container {\n  position: absolute;\n  top: 0;\n  left: 0;\n  right: 0;\n  bottom: 0;\n  overflow: hidden;\n  user-select: none;\n  touch-action: none;\n  cursor: move;\n  display: flex;\n  justify-content: center;\n  align-items: center;\n}\n\n.reactEasyCrop_Image,\n.reactEasyCrop_Video {\n  will-change: transform; /* this improves performances and prevent painting issues on iOS Chrome */\n}\n\n.reactEasyCrop_Contain {\n  max-width: 100%;\n  max-height: 100%;\n  margin: auto;\n  position: absolute;\n  top: 0;\n  bottom: 0;\n  left: 0;\n  right: 0;\n}\n.reactEasyCrop_Cover_Horizontal {\n  width: 100%;\n  height: auto;\n}\n.reactEasyCrop_Cover_Vertical {\n  width: auto;\n  height: 100%;\n}\n\n.reactEasyCrop_CropArea {\n  position: absolute;\n  left: 50%;\n  top: 50%;\n  transform: translate(-50%, -50%);\n  border: 1px solid rgba(255, 255, 255, 0.5);\n  box-sizing: border-box;\n  box-shadow: 0 0 0 9999em;\n  color: rgba(0, 0, 0, 0.5);\n  overflow: hidden;\n}\n\n.reactEasyCrop_CropAreaRound {\n  border-radius: 50%;\n}\n\n.reactEasyCrop_CropAreaGrid::before {\n  content: ' ';\n  box-sizing: border-box;\n  position: absolute;\n  border: 1px solid rgba(255, 255, 255, 0.5);\n  top: 0;\n  bottom: 0;\n  left: 33.33%;\n  right: 33.33%;\n  border-top: 0;\n  border-bottom: 0;\n}\n\n.reactEasyCrop_CropAreaGrid::after {\n  content: ' ';\n  box-sizing: border-box;\n  position: absolute;\n  border: 1px solid rgba(255, 255, 255, 0.5);\n  top: 33.33%;\n  bottom: 33.33%;\n  left: 0;\n  right: 0;\n  border-left: 0;\n  border-right: 0;\n}\n", this.currentDoc.head.appendChild(this.styleRef)), this.imageRef.current && this.imageRef.current.complete && this.onMediaLoad(), this.props.setImageRef && this.props.setImageRef(this.imageRef), this.props.setVideoRef) && this.props.setVideoRef(this.videoRef)
     }, f.prototype.componentWillUnmount = function() {
         var t;
         this.currentDoc && this.currentWindow && (void 0 === window.ResizeObserver && this.currentWindow.removeEventListener("resize", this.computeSizes), null != (t = this.resizeObserver) && t.disconnect(), this.containerRef && this.containerRef.removeEventListener("gesturestart", this.preventZoomSafari), this.styleRef && null != (t = this.styleRef.parentNode) && t.removeChild(this.styleRef), this.cleanEvents(), this.props.zoomWithScroll) && this.clearScrollEvent()
     }, f.prototype.componentDidUpdate = function(t) {
@@ -122123,23 +122265,23 @@
         var t = this.props,
             e = t.cropSize,
             t = t.aspect;
         return e ? e.width / e.height : t
     }, f.prototype.onPinchStart = function(t) {
         var e = f.getTouchPoint(t.touches[0]),
             t = f.getTouchPoint(t.touches[1]);
-        this.lastPinchDistance = Kp(e, t), this.lastPinchRotation = Up(e, t), this.onDragStart(Xp(e, t))
+        this.lastPinchDistance = Zp(e, t), this.lastPinchRotation = Jp(e, t), this.onDragStart(ef(e, t))
     }, f.prototype.onPinchMove = function(t) {
         var n, a, r, o = this;
-        this.currentDoc && this.currentWindow && (n = f.getTouchPoint(t.touches[0]), a = f.getTouchPoint(t.touches[1]), r = Xp(n, a), this.onDrag(r), this.rafPinchTimeout && this.currentWindow.cancelAnimationFrame(this.rafPinchTimeout), this.rafPinchTimeout = this.currentWindow.requestAnimationFrame(function() {
-            var t = Kp(n, a),
+        this.currentDoc && this.currentWindow && (n = f.getTouchPoint(t.touches[0]), a = f.getTouchPoint(t.touches[1]), r = ef(n, a), this.onDrag(r), this.rafPinchTimeout && this.currentWindow.cancelAnimationFrame(this.rafPinchTimeout), this.rafPinchTimeout = this.currentWindow.requestAnimationFrame(function() {
+            var t = Zp(n, a),
                 e = o.props.zoom * (t / o.lastPinchDistance),
                 e = (o.setNewZoom(e, r, {
                     shouldUpdatePosition: !1
-                }), o.lastPinchDistance = t, Up(n, a)),
+                }), o.lastPinchDistance = t, Jp(n, a)),
                 t = o.props.rotation + (e - o.lastPinchRotation);
             o.props.onRotationChange && o.props.onRotationChange(t), o.lastPinchRotation = e
         }))
     }, f.prototype.render = function() {
         var e = this,
             t = this.props,
             n = t.image,
@@ -122166,50 +122308,50 @@
             onMouseDown: this.onMouseDown,
             onTouchStart: this.onTouchStart,
             ref: function(t) {
                 return e.containerRef = t
             },
             "data-testid": "container",
             style: f,
-            className: Jp("reactEasyCrop_Container", g)
-        }, n ? H.a.createElement("img", Fp({
+            className: rf("reactEasyCrop_Container", g)
+        }, n ? H.a.createElement("img", Gp({
             alt: "",
-            className: Jp("reactEasyCrop_Image", "contain" === t && "reactEasyCrop_Contain", "horizontal-cover" === t && "reactEasyCrop_Cover_Horizontal", "vertical-cover" === t && "reactEasyCrop_Cover_Vertical", "auto-cover" === t && (this.mediaSize.naturalWidth > this.mediaSize.naturalHeight ? "reactEasyCrop_Cover_Horizontal" : "reactEasyCrop_Cover_Vertical"), m)
+            className: rf("reactEasyCrop_Image", "contain" === t && "reactEasyCrop_Contain", "horizontal-cover" === t && "reactEasyCrop_Cover_Horizontal", "vertical-cover" === t && "reactEasyCrop_Cover_Vertical", "auto-cover" === t && (this.mediaSize.naturalWidth > this.mediaSize.naturalHeight ? "reactEasyCrop_Cover_Horizontal" : "reactEasyCrop_Cover_Vertical"), m)
         }, r, {
             src: n,
             ref: this.imageRef,
-            style: Fp(Fp({}, p), {
+            style: Gp(Gp({}, p), {
                 transform: o || "translate(".concat(l, "px, ").concat(i, "px) rotate(").concat(c, "deg) scale(").concat(s, ")")
             }),
             onLoad: this.onMediaLoad
-        })) : a && H.a.createElement("video", Fp({
+        })) : a && H.a.createElement("video", Gp({
             autoPlay: !0,
             loop: !0,
             muted: !0,
-            className: Jp("reactEasyCrop_Video", "contain" === t && "reactEasyCrop_Contain", "horizontal-cover" === t && "reactEasyCrop_Cover_Horizontal", "vertical-cover" === t && "reactEasyCrop_Cover_Vertical", "auto-cover" === t && (this.mediaSize.naturalWidth > this.mediaSize.naturalHeight ? "reactEasyCrop_Cover_Horizontal" : "reactEasyCrop_Cover_Vertical"), m)
+            className: rf("reactEasyCrop_Video", "contain" === t && "reactEasyCrop_Contain", "horizontal-cover" === t && "reactEasyCrop_Cover_Horizontal", "vertical-cover" === t && "reactEasyCrop_Cover_Vertical", "auto-cover" === t && (this.mediaSize.naturalWidth > this.mediaSize.naturalHeight ? "reactEasyCrop_Cover_Horizontal" : "reactEasyCrop_Cover_Vertical"), m)
         }, r, {
             ref: this.videoRef,
             onLoadedMetadata: this.onMediaLoad,
-            style: Fp(Fp({}, p), {
+            style: Gp(Gp({}, p), {
                 transform: o || "translate(".concat(l, "px, ").concat(i, "px) rotate(").concat(c, "deg) scale(").concat(s, ")")
             }),
             controls: !1
         }), (Array.isArray(a) ? a : [{
             src: a
         }]).map(function(t) {
-            return H.a.createElement("source", Fp({
+            return H.a.createElement("source", Gp({
                 key: t.src
             }, t))
         })), this.state.cropSize && H.a.createElement("div", {
-            style: Fp(Fp({}, h), {
+            style: Gp(Gp({}, h), {
                 width: this.state.cropSize.width,
                 height: this.state.cropSize.height
             }),
             "data-testid": "cropper",
-            className: Jp("reactEasyCrop_CropArea", "round" === u && "reactEasyCrop_CropAreaRound", d && "reactEasyCrop_CropAreaGrid", b)
+            className: rf("reactEasyCrop_CropArea", "round" === u && "reactEasyCrop_CropAreaRound", d && "reactEasyCrop_CropAreaGrid", b)
         }))
     }, f.defaultProps = {
         zoom: 1,
         rotation: 0,
         aspect: 4 / 3,
         maxZoom: 3,
         minZoom: 1,
@@ -122229,18 +122371,18 @@
         }
     }, f.getTouchPoint = function(t) {
         return {
             x: Number(t.clientX),
             y: Number(t.clientY)
         }
     };
-    var Qp, tf, ef = f;
+    var of, lf, cf = f;
 
     function f() {
-        var d = null !== Qp && Qp.apply(this, arguments) || this;
+        var d = null !== of && of.apply(this, arguments) || this;
         return d.imageRef = H.a.createRef(), d.videoRef = H.a.createRef(), d.containerRef = null, d.styleRef = null, d.containerRect = null, d.mediaSize = {
             width: 0,
             height: 0,
             naturalWidth: 0,
             naturalHeight: 0
         }, d.dragStartPosition = {
             x: 0,
@@ -122263,21 +122405,21 @@
         }, d.clearScrollEvent = function() {
             d.containerRef && d.containerRef.removeEventListener("wheel", d.onWheel), d.wheelTimer && clearTimeout(d.wheelTimer)
         }, d.onMediaLoad = function() {
             var t = d.computeSizes();
             t && (d.emitCropData(), d.setInitialCrop(t)), d.props.onMediaLoaded && d.props.onMediaLoaded(d.mediaSize)
         }, d.setInitialCrop = function(t) {
             var e, n, a, r, o, i, l, c;
-            d.props.initialCroppedAreaPercentages ? (a = d.props.initialCroppedAreaPercentages, r = d.mediaSize, o = d.props.rotation, i = t, l = d.props.minZoom, c = d.props.maxZoom, r = $p(r.width, r.height, o), c = (l = {
+            d.props.initialCroppedAreaPercentages ? (a = d.props.initialCroppedAreaPercentages, r = d.mediaSize, o = d.props.rotation, i = t, l = d.props.minZoom, c = d.props.maxZoom, r = nf(r.width, r.height, o), c = (l = {
                 crop: {
-                    x: (o = Zp(i.width / r.width * (100 / a.width), l, c)) * r.width / 2 - i.width / 2 - r.width * o * (a.x / 100),
+                    x: (o = af(i.width / r.width * (100 / a.width), l, c)) * r.width / 2 - i.width / 2 - r.width * o * (a.x / 100),
                     y: o * r.height / 2 - i.height / 2 - r.height * o * (a.y / 100)
                 },
                 zoom: o
-            }).zoom, d.props.onCropChange(l.crop), d.props.onZoomChange && d.props.onZoomChange(c)) : d.props.initialCroppedAreaPixels && (e = d.props.initialCroppedAreaPixels, i = d.mediaSize, r = d.props.rotation, n = t, a = d.props.minZoom, o = d.props.maxZoom, r = $p(i.naturalWidth, i.naturalHeight, r = void 0 === r ? 0 : r), i = Zp(function(t) {
+            }).zoom, d.props.onCropChange(l.crop), d.props.onZoomChange && d.props.onZoomChange(c)) : d.props.initialCroppedAreaPixels && (e = d.props.initialCroppedAreaPixels, i = d.mediaSize, r = d.props.rotation, n = t, a = d.props.minZoom, o = d.props.maxZoom, r = nf(i.naturalWidth, i.naturalHeight, r = void 0 === r ? 0 : r), i = af(function(t) {
                 t = t.width > t.height ? t.width / t.naturalWidth : t.height / t.naturalHeight;
                 return n.height > n.width ? n.height / (e.height * t) : n.width / (e.width * t)
             }(i), a, o), a = n.height > n.width ? n.height / e.height : n.width / e.width, c = (l = {
                 crop: {
                     x: ((r.width - e.width) / 2 - e.x) * a,
                     y: ((r.height - e.height) / 2 - e.y) * a
                 },
@@ -122323,19 +122465,19 @@
                             width: d.containerRect.height * c,
                             height: d.containerRect.height
                         }
                 } else s = {
                     width: r.offsetWidth,
                     height: r.offsetHeight
                 };
-                d.mediaSize = Fp(Fp({}, s), {
+                d.mediaSize = Gp(Gp({}, s), {
                     naturalWidth: i,
                     naturalHeight: l
                 }), d.props.setMediaSize && d.props.setMediaSize(d.mediaSize);
-                var u = d.props.cropSize || (t = d.mediaSize.width, r = d.mediaSize.height, u = d.containerRect.width, e = d.containerRect.height, n = d.props.aspect, a = d.props.rotation, t = $p(t, r, a = void 0 === a ? 0 : a), r = t.width, a = t.height, t = Math.min(r, u), (r = Math.min(a, e)) * n < t ? {
+                var u = d.props.cropSize || (t = d.mediaSize.width, r = d.mediaSize.height, u = d.containerRect.width, e = d.containerRect.height, n = d.props.aspect, a = d.props.rotation, t = nf(t, r, a = void 0 === a ? 0 : a), r = t.width, a = t.height, t = Math.min(r, u), (r = Math.min(a, e)) * n < t ? {
                     width: r * n,
                     height: r
                 } : {
                     width: t,
                     height: t / n
                 });
                 return (null == (a = d.state.cropSize) ? void 0 : a.height) === u.height && (null == (e = d.state.cropSize) ? void 0 : e.width) === u.width || d.props.onCropSizeChange && d.props.onCropSizeChange(u), d.setState({
@@ -122363,31 +122505,31 @@
             d.cleanEvents()
         }, d.onDragStart = function(t) {
             var e = t.x,
                 t = t.y;
             d.dragStartPosition = {
                 x: e,
                 y: t
-            }, d.dragStartCrop = Fp({}, d.props.crop), null != (t = (e = d.props).onInteractionStart) && t.call(e)
+            }, d.dragStartCrop = Gp({}, d.props.crop), null != (t = (e = d.props).onInteractionStart) && t.call(e)
         }, d.onDrag = function(t) {
             var n = t.x,
                 a = t.y;
             d.currentWindow && (d.rafDragTimeout && d.currentWindow.cancelAnimationFrame(d.rafDragTimeout), d.rafDragTimeout = d.currentWindow.requestAnimationFrame(function() {
                 var t, e;
                 d.state.cropSize && void 0 !== n && void 0 !== a && (t = n - d.dragStartPosition.x, e = a - d.dragStartPosition.y, t = {
                     x: d.dragStartCrop.x + t,
                     y: d.dragStartCrop.y + e
-                }, e = d.props.restrictPosition ? Wp(t, d.mediaSize, d.state.cropSize, d.props.zoom, d.props.rotation) : t, d.props.onCropChange(e))
+                }, e = d.props.restrictPosition ? Xp(t, d.mediaSize, d.state.cropSize, d.props.zoom, d.props.rotation) : t, d.props.onCropChange(e))
             }))
         }, d.onDragStopped = function() {
             var t, e;
             d.isTouching = !1, d.cleanEvents(), d.emitCropData(), null != (e = (t = d.props).onInteractionEnd) && e.call(t)
         }, d.onWheel = function(t) {
             var e;
-            !d.currentWindow || d.props.onWheelRequest && !d.props.onWheelRequest(t) || (t.preventDefault(), e = f.getMousePoint(t), t = Hp()(t).pixelY, t = d.props.zoom - t * d.props.zoomSpeed / 200, d.setNewZoom(t, e, {
+            !d.currentWindow || d.props.onWheelRequest && !d.props.onWheelRequest(t) || (t.preventDefault(), e = f.getMousePoint(t), t = qp()(t).pixelY, t = d.props.zoom - t * d.props.zoomSpeed / 200, d.setNewZoom(t, e, {
                 shouldUpdatePosition: !0
             }), d.state.hasWheelJustStarted || d.setState({
                 hasWheelJustStarted: !0
             }, function() {
                 var t, e;
                 return null == (e = (t = d.props).onInteractionStart) ? void 0 : e.call(t)
             }), d.wheelTimer && clearTimeout(d.wheelTimer), d.wheelTimer = d.currentWindow.setTimeout(function() {
@@ -122415,55 +122557,55 @@
             return {
                 x: (e + a.x) / n,
                 y: (t + a.y) / n
             }
         }, d.setNewZoom = function(t, e, n) {
             var n = (void 0 === n ? {} : n).shouldUpdatePosition,
                 n = void 0 === n || n;
-            d.state.cropSize && d.props.onZoomChange && (t = Zp(t, d.props.minZoom, d.props.maxZoom), n && (n = d.getPointOnContainer(e), e = {
+            d.state.cropSize && d.props.onZoomChange && (t = af(t, d.props.minZoom, d.props.maxZoom), n && (n = d.getPointOnContainer(e), e = {
                 x: (e = d.getPointOnMedia(n)).x * t - n.x,
                 y: e.y * t - n.y
-            }, n = d.props.restrictPosition ? Wp(e, d.mediaSize, d.state.cropSize, t, d.props.rotation) : e, d.props.onCropChange(n)), d.props.onZoomChange(t))
+            }, n = d.props.restrictPosition ? Xp(e, d.mediaSize, d.state.cropSize, t, d.props.rotation) : e, d.props.onCropChange(n)), d.props.onZoomChange(t))
         }, d.getCropData = function() {
-            return d.state.cropSize ? (t = d.props.restrictPosition ? Wp(d.props.crop, d.mediaSize, d.state.cropSize, d.props.zoom, d.props.rotation) : d.props.crop, e = d.mediaSize, n = d.state.cropSize, a = d.getAspect(), r = d.props.zoom, o = d.props.rotation, i = (i = void 0 === (i = d.props.restrictPosition) ? !0 : i) ? Gp : qp, l = $p(e.width, e.height, o = void 0 === o ? 0 : o), e = $p(e.naturalWidth, e.naturalHeight, o), o = {
+            return d.state.cropSize ? (t = d.props.restrictPosition ? Xp(d.props.crop, d.mediaSize, d.state.cropSize, d.props.zoom, d.props.rotation) : d.props.crop, e = d.mediaSize, n = d.state.cropSize, a = d.getAspect(), r = d.props.zoom, o = d.props.rotation, i = (i = void 0 === (i = d.props.restrictPosition) ? !0 : i) ? Qp : tf, l = nf(e.width, e.height, o = void 0 === o ? 0 : o), e = nf(e.naturalWidth, e.naturalHeight, o), o = {
                 x: i(100, ((l.width - n.width / r) / 2 - t.x / r) / l.width * 100),
                 y: i(100, ((l.height - n.height / r) / 2 - t.y / r) / l.height * 100),
                 width: i(100, n.width / l.width * 100 / r),
                 height: i(100, n.height / l.height * 100 / r)
             }, t = Math.round(i(e.width, o.width * e.width / 100)), n = Math.round(i(e.height, o.height * e.height / 100)), l = e.width >= e.height * a ? {
                 width: Math.round(n * a),
                 height: n
             } : {
                 width: t,
                 height: Math.round(t / a)
             }, {
                 croppedAreaPercentages: o,
-                croppedAreaPixels: Fp(Fp({}, l), {
+                croppedAreaPixels: Gp(Gp({}, l), {
                     x: Math.round(i(e.width - l.width, o.x * e.width / 100)),
                     y: Math.round(i(e.height - l.height, o.y * e.height / 100))
                 })
             }) : null;
             var t, e, n, a, r, o, i, l
         }, d.emitCropData = function() {
             var t, e = d.getCropData();
             e && (t = e.croppedAreaPercentages, e = e.croppedAreaPixels, d.props.onCropComplete && d.props.onCropComplete(t, e), d.props.onCropAreaChange) && d.props.onCropAreaChange(t, e)
         }, d.emitCropAreaChange = function() {
             var t, e = d.getCropData();
             e && (t = e.croppedAreaPercentages, e = e.croppedAreaPixels, d.props.onCropAreaChange) && d.props.onCropAreaChange(t, e)
         }, d.recomputeCropPosition = function() {
             var t;
-            d.state.cropSize && (t = d.props.restrictPosition ? Wp(d.props.crop, d.mediaSize, d.state.cropSize, d.props.zoom, d.props.rotation) : d.props.crop, d.props.onCropChange(t), d.emitCropData())
+            d.state.cropSize && (t = d.props.restrictPosition ? Xp(d.props.crop, d.mediaSize, d.state.cropSize, d.props.zoom, d.props.rotation) : d.props.crop, d.props.onCropChange(t), d.emitCropData())
         }, d
     }
 
-    function nf() {
-        this.constructor = tf
+    function sf() {
+        this.constructor = lf
     }
-    const af = "img-crop",
-        rf = Object(Wt.forwardRef)((t, e) => {
+    const uf = "img-crop",
+        df = Object(Wt.forwardRef)((t, e) => {
             const {
                 cropperRef: n,
                 zoomSlider: a,
                 rotationSlider: r,
                 aspectSlider: o,
                 showReset: i,
                 image: l,
@@ -122489,15 +122631,15 @@
                 setZoom: g,
                 rotation: b,
                 setRotation: v,
                 cropPixelsRef: k
             }));
             t = "flex items-center w-3/5 mx-auto", e = "flex items-center justify-center w-8 h-8 bg-transparent border-0 font-[inherit] text-[18px] cursor-pointer disabled:opacity-20 disabled:cursor-default";
             return Object(F.jsxs)(F.Fragment, {
-                children: [Object(F.jsx)(ef, Object.assign({}, f, {
+                children: [Object(F.jsx)(cf, Object.assign({}, f, {
                     ref: n,
                     image: l,
                     crop: O,
                     zoom: m,
                     rotation: b,
                     aspect: y,
                     minZoom: s,
@@ -122506,73 +122648,73 @@
                     cropShape: d,
                     showGrid: p,
                     onCropChange: w,
                     onZoomChange: g,
                     onRotationChange: v,
                     onCropComplete: j,
                     classes: {
-                        containerClassName: af + "-container !relative w-full h-[40vh] [&~section:first-of-type]:mt-4 [&~section:last-of-type]:mb-4",
-                        mediaClassName: af + "-media"
+                        containerClassName: uf + "-container !relative w-full h-[40vh] [&~section:first-of-type]:mt-4 [&~section:last-of-type]:mb-4",
+                        mediaClassName: uf + "-media"
                     }
                 })), a && Object(F.jsxs)("section", Object.assign({
-                    className: af + `-control ${af}-control-zoom ` + t
+                    className: uf + `-control ${uf}-control-zoom ` + t
                 }, {
                     children: [Object(F.jsx)("button", Object.assign({
                         className: e,
                         onClick: () => g(m - .1),
                         disabled: !0
                     }, {
                         children: "－"
-                    })), Object(F.jsx)(me, {
+                    })), Object(F.jsx)(ye, {
                         className: "flex-1 mx-2",
                         min: s,
                         max: u,
                         step: .1,
                         value: m,
                         onChange: g
                     }), Object(F.jsx)("button", Object.assign({
                         className: e,
                         onClick: () => g(m + .1),
                         disabled: m + .1 > u
                     }, {
                         children: "＋"
                     }))]
                 })), r && Object(F.jsxs)("section", Object.assign({
-                    className: af + `-control ${af}-control-rotation ` + t
+                    className: uf + `-control ${uf}-control-rotation ` + t
                 }, {
                     children: [Object(F.jsx)("button", Object.assign({
                         className: e + " !text-[16px]",
                         onClick: () => v(b - 1),
                         disabled: -180 === b
                     }, {
                         children: "↺"
-                    })), Object(F.jsx)(me, {
+                    })), Object(F.jsx)(ye, {
                         className: "flex-1 mx-2",
                         min: -180,
                         max: 180,
                         step: 1,
                         value: b,
                         onChange: v
                     }), Object(F.jsx)("button", Object.assign({
                         className: e + " !text-[16px]",
                         onClick: () => v(b + 1),
                         disabled: 180 === b
                     }, {
                         children: "↻"
                     }))]
                 })), o && Object(F.jsxs)("section", Object.assign({
-                    className: af + `-control ${af}-control-aspect ` + t
+                    className: uf + `-control ${uf}-control-aspect ` + t
                 }, {
                     children: [Object(F.jsx)("button", Object.assign({
                         className: e,
                         onClick: () => x(y - .01),
                         disabled: y - .01 < .5
                     }, {
                         children: "↕️"
-                    })), Object(F.jsx)(me, {
+                    })), Object(F.jsx)(ye, {
                         className: "flex-1 mx-2",
                         min: .5,
                         max: 2,
                         step: .01,
                         value: y,
                         onChange: x
                     }), Object(F.jsx)("button", Object.assign({
@@ -122592,19 +122734,19 @@
                         g(1), v(0), x(c)
                     }
                 }, {
                     children: h ? "重置" : "Reset"
                 }))]
             })
         });
-    var of = Object(Wt.memo)(rf);
-    o = ".container{width:100%}@media (min-width:640px){.container{max-width:640px}}@media (min-width:768px){.container{max-width:768px}}@media (min-width:1024px){.container{max-width:1024px}}@media (min-width:1280px){.container{max-width:1280px}}@media (min-width:1536px){.container{max-width:1536px}}.visible{visibility:visible}.absolute{position:absolute}.\\!relative{position:relative!important}.bottom-\\[20px\\]{bottom:20px}.mx-2{margin-left:.5rem;margin-right:.5rem}.mx-auto{margin-left:auto;margin-right:auto}.flex{display:flex}.grid{display:grid}.h-8{height:2rem}.h-\\[40vh\\]{height:40vh}.w-3\\/5{width:60%}.w-8{width:2rem}.w-full{width:100%}.flex-1{flex:1 1 0%}.cursor-pointer{cursor:pointer}.items-center{align-items:center}.justify-center{justify-content:center}.border-0{border-width:0}.bg-transparent{background-color:transparent}.font-\\[inherit\\]{font-family:inherit}.\\!text-\\[16px\\]{font-size:16px!important}.text-\\[18px\\]{font-size:18px}.disabled\\:cursor-default:disabled{cursor:default}.disabled\\:opacity-20:disabled{opacity:.2}.\\[\\&\\~section\\:first-of-type\\]\\:mt-4~section:first-of-type{margin-top:1rem}.\\[\\&\\~section\\:last-of-type\\]\\:mb-4~section:last-of-type{margin-bottom:1rem}", hh = (hh = void 0 === hh ? {} : hh).insertAt, "undefined" != typeof document && (a = document.head || document.getElementsByTagName("head")[0], (c = document.createElement("style")).type = "text/css", "top" === hh && a.firstChild ? a.insertBefore(c, a.firstChild) : a.appendChild(c), c.styleSheet ? c.styleSheet.cssText = o : c.appendChild(document.createTextNode(o)));
-    const lf = -1 === (d = "4.23.0", p = Ap(p = "5.2.2"), d = Ap(d), r = p.pop(), l = d.pop(), 0 !== (p = Yp(p, d)) ? p : r && l ? Yp(r.split("."), l.split(".")) : r || l ? r ? -1 : 1 : 0) ? "visible" : "open",
-        cf = (t, e, n) => e in t ? (console.error(`\`${e}\` is deprecated, please use \`${n}\` instead`), t[e]) : t[n],
-        sf = Object(Wt.forwardRef)((t, e) => {
+    var pf = Object(Wt.memo)(df);
+    o = ".container{width:100%}@media (min-width:640px){.container{max-width:640px}}@media (min-width:768px){.container{max-width:768px}}@media (min-width:1024px){.container{max-width:1024px}}@media (min-width:1280px){.container{max-width:1280px}}@media (min-width:1536px){.container{max-width:1536px}}.visible{visibility:visible}.absolute{position:absolute}.\\!relative{position:relative!important}.bottom-\\[20px\\]{bottom:20px}.mx-2{margin-left:.5rem;margin-right:.5rem}.mx-auto{margin-left:auto;margin-right:auto}.flex{display:flex}.grid{display:grid}.h-8{height:2rem}.h-\\[40vh\\]{height:40vh}.w-3\\/5{width:60%}.w-8{width:2rem}.w-full{width:100%}.flex-1{flex:1 1 0%}.cursor-pointer{cursor:pointer}.items-center{align-items:center}.justify-center{justify-content:center}.border-0{border-width:0}.bg-transparent{background-color:transparent}.font-\\[inherit\\]{font-family:inherit}.\\!text-\\[16px\\]{font-size:16px!important}.text-\\[18px\\]{font-size:18px}.disabled\\:cursor-default:disabled{cursor:default}.disabled\\:opacity-20:disabled{opacity:.2}.\\[\\&\\~section\\:first-of-type\\]\\:mt-4~section:first-of-type{margin-top:1rem}.\\[\\&\\~section\\:last-of-type\\]\\:mb-4~section:last-of-type{margin-bottom:1rem}", xh = (xh = void 0 === xh ? {} : xh).insertAt, "undefined" != typeof document && (a = document.head || document.getElementsByTagName("head")[0], (c = document.createElement("style")).type = "text/css", "top" === xh && a.firstChild ? a.insertBefore(c, a.firstChild) : a.appendChild(c), c.styleSheet ? c.styleSheet.cssText = o : c.appendChild(document.createTextNode(o)));
+    const ff = -1 === (d = "4.23.0", p = Fp(p = "5.2.2"), d = Fp(d), r = p.pop(), l = d.pop(), 0 !== (p = Kp(p, d)) ? p : r && l ? Kp(r.split("."), l.split(".")) : r || l ? r ? -1 : 1 : 0) ? "visible" : "open",
+        hf = (t, e, n) => e in t ? (console.error(`\`${e}\` is deprecated, please use \`${n}\` instead`), t[e]) : t[n],
+        mf = Object(Wt.forwardRef)((t, e) => {
             const {
                 quality: m = .4,
                 fillColor: g = "white",
                 aspectSlider: n = !1,
                 aspect: a = 1,
                 minZoom: r = 1,
                 maxZoom: o = 3,
@@ -122617,26 +122759,26 @@
                 showReset: p = !1,
                 onModalOk: f,
                 onModalCancel: h,
                 modalProps: b,
                 beforeCrop: v,
                 onUploadFail: y,
                 children: x
-            } = t, _ = cf(t, "zoom", "zoomSlider") || !0, O = cf(t, "rotate", "rotationSlider") || !1, w = cf(t, "shape", "cropShape") || "rect", k = cf(t, "grid", "showGrid") || !1, j = (cf(t, "modalMaskTransitionName", "modalProps.maskTransitionName"), cf(t, "modalTransitionName", "modalProps.transitionName"), Object(Wt.useRef)({})), [M, E] = (j.current.onModalOk = f, j.current.onModalCancel = h, j.current.beforeCrop = v, j.current.onUploadFail = y, Object(Wt.useState)("")), C = Object(Wt.useRef)({}), S = Object(Wt.useRef)(), L = Object(Wt.useRef)(() => {}), P = Object(Wt.useRef)(() => {}), D = Object(Wt.useMemo)(() => {
+            } = t, _ = hf(t, "zoom", "zoomSlider") || !0, O = hf(t, "rotate", "rotationSlider") || !1, w = hf(t, "shape", "cropShape") || "rect", k = hf(t, "grid", "showGrid") || !1, j = (hf(t, "modalMaskTransitionName", "modalProps.maskTransitionName"), hf(t, "modalTransitionName", "modalProps.transitionName"), Object(Wt.useRef)({})), [M, E] = (j.current.onModalOk = f, j.current.onModalCancel = h, j.current.beforeCrop = v, j.current.onUploadFail = y, Object(Wt.useState)("")), C = Object(Wt.useRef)({}), S = Object(Wt.useRef)(), L = Object(Wt.useRef)(() => {}), P = Object(Wt.useRef)(() => {}), D = Object(Wt.useMemo)(() => {
                 var t = Array.isArray(x) ? x[0] : x,
                     e = t.props,
                     {
                         beforeUpload: n,
                         accept: a
                     } = e,
-                    e = Object(Tp.f)(e, ["beforeUpload", "accept"]);
+                    e = Object(Yp.f)(e, ["beforeUpload", "accept"]);
                 return S.current = n, Object.assign(Object.assign({}, t), {
                     props: Object.assign(Object.assign({}, e), {
                         accept: a || "image/*",
-                        beforeUpload: (e, n) => new Promise((a, r) => Object(Tp.b)(void 0, void 0, void 0, function*() {
+                        beforeUpload: (e, n) => new Promise((a, r) => Object(Yp.b)(void 0, void 0, void 0, function*() {
                             if ("function" == typeof j.current.beforeCrop && !(yield j.current.beforeCrop(e, n))) return r();
                             C.current = e, L.current = t => {
                                 var e, n;
                                 null != (n = (e = j.current).onModalOk) && n.call(e, t), a(t)
                             }, P.current = t => {
                                 var e, n;
                                 null != (n = (e = j.current).onUploadFail) && n.call(e, t), r()
@@ -122652,21 +122794,21 @@
                 var t = {};
                 return void 0 !== s && (t.width = s), void 0 !== u && (t.okText = u), void 0 !== d && (t.cancelText = d), t
             }, [d, u, s]), z = () => {
                 E(""), T.current.setZoom(1), T.current.setRotation(0)
             }, I = Object(Wt.useCallback)(() => {
                 var t, e;
                 null != (e = (t = j.current).onModalCancel) && e.call(t), z()
-            }, []), N = Object(Wt.useCallback)(h => Object(Tp.b)(void 0, void 0, void 0, function*() {
+            }, []), N = Object(Wt.useCallback)(h => Object(Yp.b)(void 0, void 0, void 0, function*() {
                 var t;
                 z();
                 const e = document.createElement("canvas"),
                     n = e.getContext("2d"),
                     a = h.target,
-                    r = ((null == (t = null == a ? void 0 : a.getRootNode) ? void 0 : t.call(a)) || document).querySelector(`.${af}-media`),
+                    r = ((null == (t = null == a ? void 0 : a.getRootNode) ? void 0 : t.call(a)) || document).querySelector(`.${uf}-media`),
                     {
                         width: o,
                         height: i,
                         x: l,
                         y: c
                     } = T.current.cropPixelsRef.current;
                 if (O && 0 !== T.current.rotation) {
@@ -122683,41 +122825,41 @@
                     e.width = o, e.height = i, n.putImageData(s, -l, -c)
                 } else e.width = o, e.height = i, n.fillStyle = g, n.fillRect(0, 0, o, i), n.drawImage(r, l, c, o, i, 0, 0, o, i);
                 const {
                     type: d,
                     name: p,
                     uid: f
                 } = C.current;
-                e.toBlob(n => Object(Tp.b)(void 0, void 0, void 0, function*() {
+                e.toBlob(n => Object(Yp.b)(void 0, void 0, void 0, function*() {
                     var t = new File([n], p, {
                         type: d
                     });
                     if (Object.assign(t, {
                             uid: f
                         }), "function" == typeof S.current) try {
                         const n = t,
                             e = yield S.current(n, [n]);
                         !0 === e ? L.current(t) : !1 === e ? P.current(new Error("beforeUpload → false")) : L.current(e)
                     } catch (t) {
                         P.current(new Error("beforeUpload → reject"))
                     } else L.current(t)
                 }), d, m)
-            }), [g, m, O]), Y = af + "-modal" + (l ? " " + l : ""), A = "zh-CN" === ("undefined" == typeof window ? "" : window.navigator.language), B = c || (A ? "编辑图片" : "Edit image");
+            }), [g, m, O]), Y = uf + "-modal" + (l ? " " + l : ""), A = "zh-CN" === ("undefined" == typeof window ? "" : window.navigator.language), B = c || (A ? "编辑图片" : "Edit image");
             return Object(F.jsxs)(F.Fragment, {
-                children: [D, M && Object(F.jsx)(dr, Object.assign({}, b, R, {
-                    [lf]: !0
+                children: [D, M && Object(F.jsx)(hr, Object.assign({}, b, R, {
+                    [ff]: !0
                 }, {
                     title: B,
                     onOk: N,
                     onCancel: I,
                     wrapClassName: Y,
                     maskClosable: !1,
                     destroyOnClose: !0
                 }, {
-                    children: Object(F.jsx)(of, {
+                    children: Object(F.jsx)(pf, {
                         ref: T,
                         cropperRef: e,
                         zoomSlider: _,
                         rotationSlider: O,
                         aspectSlider: n,
                         showReset: p,
                         image: M,
@@ -122729,69 +122871,69 @@
                         cropperProps: i,
                         isCN: A
                     })
                 }))]
             })
         });
 
-    function uf(t) {
-        return (uf = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
+    function gf(t) {
+        return (gf = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
             return typeof t
         } : function(t) {
             return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
         })(t)
     }
 
-    function df() {
-        return (df = Object.assign ? Object.assign.bind() : function(t) {
+    function bf() {
+        return (bf = Object.assign ? Object.assign.bind() : function(t) {
             for (var e = 1; e < arguments.length; e++) {
                 var n, a = arguments[e];
                 for (n in a) Object.prototype.hasOwnProperty.call(a, n) && (t[n] = a[n])
             }
             return t
         }).apply(this, arguments)
     }
 
-    function pf(e, t) {
+    function vf(e, t) {
         var n, a = Object.keys(e);
         return Object.getOwnPropertySymbols && (n = Object.getOwnPropertySymbols(e), t && (n = n.filter(function(t) {
             return Object.getOwnPropertyDescriptor(e, t).enumerable
         })), a.push.apply(a, n)), a
     }
 
-    function ff(a) {
+    function yf(a) {
         for (var t = 1; t < arguments.length; t++) {
             var r = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? pf(Object(r), !0).forEach(function(t) {
+            t % 2 ? vf(Object(r), !0).forEach(function(t) {
                 var e, n;
                 e = a, t = r[n = t], (n = function() {
                     var t = function(t) {
-                        if ("object" !== uf(t) || null === t) return t;
+                        if ("object" !== gf(t) || null === t) return t;
                         var e = t[Symbol.toPrimitive];
                         if (void 0 === e) return String(t);
                         e = e.call(t, "string");
-                        if ("object" !== uf(e)) return e;
+                        if ("object" !== gf(e)) return e;
                         throw new TypeError("@@toPrimitive must return a primitive value.")
                     }(n);
-                    return "symbol" === uf(t) ? t : String(t)
+                    return "symbol" === gf(t) ? t : String(t)
                 }()) in e ? Object.defineProperty(e, n, {
                     value: t,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : e[n] = t
-            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(r)) : pf(Object(r)).forEach(function(t) {
+            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(r)) : vf(Object(r)).forEach(function(t) {
                 Object.defineProperty(a, t, Object.getOwnPropertyDescriptor(r, t))
             })
         }
         return a
     }
 
-    function hf() {
-        hf = function() {
+    function xf() {
+        xf = function() {
             return i
         };
         var i = {},
             t = Object.prototype,
             c = t.hasOwnProperty,
             s = Object.defineProperty || function(t, e, n) {
                 t[e] = n.value
@@ -122905,15 +123047,15 @@
             var e;
             s(this, "_invoke", {
                 value: function(n, a) {
                     function t() {
                         return new l(function(t, e) {
                             ! function e(t, n, a, r) {
                                 var o, t = u(i[t], i, n);
-                                return "throw" !== t.type ? (n = (o = t.arg).value) && "object" == uf(n) && c.call(n, "__await") ? l.resolve(n.__await).then(function(t) {
+                                return "throw" !== t.type ? (n = (o = t.arg).value) && "object" == gf(n) && c.call(n, "__await") ? l.resolve(n.__await).then(function(t) {
                                     e("next", t, a, r)
                                 }, function(t) {
                                     e("throw", t, a, r)
                                 }) : l.resolve(n).then(function(t) {
                                     o.value = t, a(o)
                                 }, function(t) {
                                     return e("throw", t, a, r)
@@ -123077,25 +123219,25 @@
                     resultName: e,
                     nextLoc: n
                 }, "next" === this.method && (this.arg = void 0), d
             }
         }, i
     }
 
-    function mf(t, e, n, a, r, o, i) {
+    function _f(t, e, n, a, r, o, i) {
         try {
             var l = t[o](i),
                 c = l.value
         } catch (t) {
             return n(t)
         }
         l.done ? e(c) : Promise.resolve(c).then(a, r)
     }
 
-    function gf(t, e) {
+    function Of(t, e) {
         return function(t) {
             if (Array.isArray(t)) return t
         }(t) || function(t, e) {
             var n = null == t ? null : "undefined" != typeof Symbol && t[Symbol.iterator] || t["@@iterator"];
             if (null != n) {
                 var a, r, o, i, l = [],
                     c = !0,
@@ -123113,31 +123255,31 @@
                         if (!c && null != n.return && (i = n.return(), Object(i) !== i)) return
                     } finally {
                         if (s) throw r
                     }
                 }
                 return l
             }
-        }(t, e) || bf(t, e) || function() {
+        }(t, e) || wf(t, e) || function() {
             throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function bf(t, e) {
+    function wf(t, e) {
         var n;
-        if (t) return "string" == typeof t ? vf(t, e) : "Map" === (n = "Object" === (n = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : n) || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? vf(t, e) : void 0
+        if (t) return "string" == typeof t ? kf(t, e) : "Map" === (n = "Object" === (n = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : n) || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? kf(t, e) : void 0
     }
 
-    function vf(t, e) {
+    function kf(t, e) {
         (null == e || e > t.length) && (e = t.length);
         for (var n = 0, a = new Array(e); n < e; n++) a[n] = t[n];
         return a
     }
 
-    function yf(t) {
+    function jf(t) {
         function e() {
             return D(!1)
         }
         var n, a = t.id,
             r = t.className,
             o = t.style,
             i = t.key,
@@ -123168,38 +123310,39 @@
             C = t.setProps,
             l = (t = Object(Wt.useContext)(G.a)) && t.locale || l,
             S = (A = w = w || [], n = new Map, A.forEach(function(t) {
                 n.set(t.uid, t.completeTimestamp)
             }), n);
         Object(Wt.useEffect)(function() {
             f || (k && 0 < k.length ? C({
-                uploadId: k[0].taskId || Object(Wd.a)()
+                uploadId: k[0].taskId || Object(Xd.a)()
             }) : C({
-                uploadId: Object(Wd.a)()
+                uploadId: Object(Xd.a)()
             }))
         }, []);
-        var L = (A = gf(Object(Wt.useState)(k || w.map(function(t) {
+        var L = (A = Of(Object(Wt.useState)(k || w.map(function(t) {
                 return {
                     name: t.fileName,
                     status: t.taskStatus,
                     uid: t.uid,
-                    url: t.url
+                    url: t.url,
+                    fileSize: t.fileSize
                 }
             })), 2))[0],
             Y = A[1],
-            P = (A = gf(Object(Wt.useState)(!1), 2))[0],
+            P = (A = Of(Object(Wt.useState)(!1), 2))[0],
             D = A[1],
-            T = (A = gf(Object(Wt.useState)(""), 2))[0],
+            T = (A = Of(Object(Wt.useState)(""), 2))[0],
             B = A[1],
-            z = (A = gf(Object(Wt.useState)(""), 2))[0],
+            z = (A = Of(Object(Wt.useState)(""), 2))[0],
             F = A[1],
             A = function() {
                 var l;
-                l = hf().mark(function t(e) {
-                    return hf().wrap(function(t) {
+                l = xf().mark(function t(e) {
+                    return xf().wrap(function(t) {
                         for (;;) switch (t.prev = t.next) {
                             case 0:
                                 if (e.url || e.preview) {
                                     t.next = 4;
                                     break
                                 }
                                 t.next = 3;
@@ -123226,26 +123369,26 @@
                     return function() {
                         var t = this,
                             i = arguments;
                         return new Promise(function(e, n) {
                             var a = l.apply(t, i);
 
                             function r(t) {
-                                mf(a, e, n, r, o, "next", t)
+                                _f(a, e, n, r, o, "next", t)
                             }
 
                             function o(t) {
-                                mf(a, e, n, r, o, "throw", t)
+                                _f(a, e, n, r, o, "throw", t)
                             }
                             r(void 0)
                         })
                     }.apply(this, arguments)
                 }
             }(),
-            m = H.a.createElement("div", null, H.a.createElement(Dp.a, null), H.a.createElement("div", {
+            m = H.a.createElement("div", null, H.a.createElement(Np.a, null), H.a.createElement("div", {
                 style: {
                     marginTop: 8
                 }
             }, m)),
             c = {
                 name: "file",
                 action: c + "?uploadId=".concat(f),
@@ -123260,15 +123403,15 @@
                 onChange: function(t) {
                     var e, n = "removed" === t.file.status ? 0 : t.fileList.length - w.length,
                         t = ("removed" === t.file.status ? C({
                             listUploadTaskRecord: t.fileList.map(function(t) {
                                 var e = u && "done" === t.status ? {
                                     url: u + "?taskId=".concat(f, "&filename=").concat(t.name)
                                 } : {};
-                                return ff({
+                                return yf({
                                     fileName: t.name,
                                     fileSize: t.size,
                                     completeTimestamp: S.get(t.uid) || (new Date).getTime(),
                                     taskStatus: "done" === t.status ? "success" : "failed",
                                     taskId: f,
                                     uid: t.uid
                                 }, e)
@@ -123281,55 +123424,55 @@
                                 taskStatus: "done" === t.file.status ? "success" : "failed",
                                 taskId: f
                             },
                             listUploadTaskRecord: t.fileList.map(function(t) {
                                 var e = u && "done" === t.status ? {
                                     url: u + "?taskId=".concat(f, "&filename=").concat(t.name)
                                 } : {};
-                                return ff({
+                                return yf({
                                     fileName: t.name,
                                     fileSize: t.size,
                                     completeTimestamp: S.get(t.uid) || (new Date).getTime(),
                                     taskStatus: "done" === t.status ? "success" : "failed",
                                     taskId: f,
                                     uid: t.uid
                                 }, e)
                             })
                         }), "done" === t.file.status && I ? $.b.success("".concat(t.file.name, " 上传成功！")) : "error" === t.file.status && N && $.b.error("".concat(t.file.name, " 上传失败！")), function(t) {
-                            if (Array.isArray(t)) return vf(t)
+                            if (Array.isArray(t)) return kf(t)
                         }(e = t.fileList) || function() {
                             if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
-                        }() || bf(e) || function() {
+                        }() || wf(e) || function() {
                             throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                         }());
                     h && (t = t.slice(-h)), 0 != n && (t = t.slice(0, t.length - n).concat(t.slice(-n).map(function(t) {
                         return "error" !== t.status && t.status || (t.status = "error", t.response = R || "上传失败"), t
                     }))), Y(u ? t.map(function(t) {
-                        return ff(ff({}, t), {}, {
+                        return yf(yf({}, t), {}, {
                             url: u + "?taskId=".concat(f, "&filename=").concat(t.name)
                         })
                     }) : t)
                 }
             };
         return g && 0 != g.length && Object.assign(c, {
             accept: "." + g.join(",.")
         }), d ? H.a.createElement(W.a, {
             locale: K.b.get(l)
         }, H.a.createElement("div", {
             id: a,
             className: Object(V.isString)(r) ? r : r ? Object(U.a)(r) : void 0,
-            style: ff(ff({
+            style: yf(yf({
                 border: "1px solid transparent",
                 transition: "border 0.3s"
-            }, xf.get(M)), o),
+            }, Mf.get(M)), o),
             key: i
-        }, H.a.createElement(sf, df({
+        }, H.a.createElement(mf, bf({
             modalOk: "zh-cn" === l ? "确定" : "OK",
             modalCancel: "zh-cn" === l ? "取消" : "Cancel"
-        }, p), H.a.createElement(Pp, df({}, c, {
+        }, p), H.a.createElement(Ip, bf({}, c, {
             fileList: L,
             listType: "picture-card",
             disabled: t && !Object(V.isUndefined)(t.componentDisabled) ? t.componentDisabled : j,
             progress: O || _ ? {
                 strokeColor: O && O.strokeColor,
                 strokeWidth: O && O.strokeWidth || 2,
                 format: _ ? function(t) {
@@ -123339,26 +123482,26 @@
             showUploadList: {
                 showRemoveIcon: v,
                 showPreviewIcon: y
             },
             onPreview: A,
             onRemove: x ? function() {
                 return new Promise(function(t, e) {
-                    dr.confirm({
+                    hr.confirm({
                         title: K.a.AntdPictureUpload[l].confirmBeforeDeleteTitle,
                         okText: K.a.AntdPictureUpload[l].confirmBeforeDeleteOkText,
                         cancelText: K.a.AntdPictureUpload[l].confirmBeforeDeleteCancelText,
                         onOk: function() {
                             t(!0)
                         }
                     })
                 })
             } : void 0,
             "data-dash-is-loading": E && E.is_loading || void 0
-        }), m)), H.a.createElement(dr, {
+        }), m)), H.a.createElement(hr, {
             visible: P,
             title: z,
             footer: null,
             onCancel: e
         }, H.a.createElement("img", {
             alt: "",
             style: {
@@ -123366,20 +123509,20 @@
             },
             src: T
         })))) : H.a.createElement(W.a, {
             locale: K.b.get(l)
         }, H.a.createElement("div", {
             id: a,
             className: Object(V.isString)(r) ? r : r ? Object(U.a)(r) : void 0,
-            style: ff(ff({
+            style: yf(yf({
                 border: "1px solid transparent",
                 transition: "border 0.3s"
-            }, xf.get(M)), o),
+            }, Mf.get(M)), o),
             key: i
-        }, H.a.createElement(Pp, df({}, c, {
+        }, H.a.createElement(Ip, bf({}, c, {
             fileList: L,
             listType: "picture-card",
             disabled: t && !Object(V.isUndefined)(t.componentDisabled) ? t.componentDisabled : j,
             progress: O || _ ? {
                 strokeColor: O && O.strokeColor,
                 strokeWidth: O && O.strokeWidth || 2,
                 format: _ ? function(t) {
@@ -123389,53 +123532,53 @@
             showUploadList: {
                 showRemoveIcon: v,
                 showPreviewIcon: y
             },
             onPreview: A,
             onRemove: x ? function() {
                 return new Promise(function(t, e) {
-                    dr.confirm({
+                    hr.confirm({
                         title: K.a.AntdPictureUpload[l].confirmBeforeDeleteTitle,
                         okText: K.a.AntdPictureUpload[l].confirmBeforeDeleteOkText,
                         cancelText: K.a.AntdPictureUpload[l].confirmBeforeDeleteCancelText,
                         onOk: function() {
                             t(!0)
                         }
                     })
                 })
             } : void 0,
             "data-dash-is-loading": E && E.is_loading || void 0
-        }), m), H.a.createElement(dr, {
+        }), m), H.a.createElement(hr, {
             visible: P,
             title: z,
             footer: null,
             onCancel: e
         }, H.a.createElement("img", {
             alt: "",
             style: {
                 width: "100%"
             },
             src: T
         }))))
     }
-    var xf = new Map([
+    var Mf = new Map([
             ["warning", {
                 border: "1px solid #faad14",
                 borderRadius: "2px",
                 padding: "6px 10px 0 10px",
                 transition: "border 0.3s"
             }],
             ["error", {
                 border: "1px solid #ff4d4f",
                 borderRadius: "2px",
                 padding: "6px 10px 0 10px",
                 transition: "border 0.3s"
             }]
         ]),
-        _f = (yf.propTypes = {
+        Ef = (jf.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             locale: n.a.oneOf(["zh-cn", "en-us"]),
             apiUrl: n.a.string,
             headers: n.a.object,
@@ -123501,106 +123644,107 @@
                 url: n.a.string
             })),
             defaultFileList: n.a.arrayOf(n.a.exact({
                 name: n.a.string,
                 status: n.a.oneOf(["done", "error", "removed"]),
                 uid: n.a.any,
                 url: n.a.string,
-                taskId: n.a.string
+                taskId: n.a.string,
+                fileSize: n.a.number
             })),
             disabled: n.a.bool,
             status: n.a.oneOf(["error", "warning"]),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, yf.defaultProps = {
+        }, jf.defaultProps = {
             disabled: !1,
             editable: !1,
             fileTypes: ["tiff", "bmp", "gif", "png", "jpeg", "jpg", "webp", "ico", "tif"],
             fileListMaxLength: null,
             fileMaxSize: 10,
             showRemoveIcon: !0,
             showPreviewIcon: !0,
             confirmBeforeDelete: !1,
             showPercent: !1,
             showSuccessMessage: !0,
             showErrorMessage: !0,
             lastUploadTaskRecord: null,
             listUploadTaskRecord: [],
             locale: "zh-cn"
-        }, yf);
+        }, jf);
 
-    function Of(t) {
-        return (Of = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
+    function Cf(t) {
+        return (Cf = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
             return typeof t
         } : function(t) {
             return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
         })(t)
     }
 
-    function wf() {
-        return (wf = Object.assign ? Object.assign.bind() : function(t) {
+    function Sf() {
+        return (Sf = Object.assign ? Object.assign.bind() : function(t) {
             for (var e = 1; e < arguments.length; e++) {
                 var n, a = arguments[e];
                 for (n in a) Object.prototype.hasOwnProperty.call(a, n) && (t[n] = a[n])
             }
             return t
         }).apply(this, arguments)
     }
 
-    function kf(e, t) {
+    function Lf(e, t) {
         var n, a = Object.keys(e);
         return Object.getOwnPropertySymbols && (n = Object.getOwnPropertySymbols(e), t && (n = n.filter(function(t) {
             return Object.getOwnPropertyDescriptor(e, t).enumerable
         })), a.push.apply(a, n)), a
     }
 
-    function jf(a) {
+    function Pf(a) {
         for (var t = 1; t < arguments.length; t++) {
             var r = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? kf(Object(r), !0).forEach(function(t) {
+            t % 2 ? Lf(Object(r), !0).forEach(function(t) {
                 var e, n;
                 e = a, t = r[n = t], (n = function() {
                     var t = function(t) {
-                        if ("object" !== Of(t) || null === t) return t;
+                        if ("object" !== Cf(t) || null === t) return t;
                         var e = t[Symbol.toPrimitive];
                         if (void 0 === e) return String(t);
                         e = e.call(t, "string");
-                        if ("object" !== Of(e)) return e;
+                        if ("object" !== Cf(e)) return e;
                         throw new TypeError("@@toPrimitive must return a primitive value.")
                     }(n);
-                    return "symbol" === Of(t) ? t : String(t)
+                    return "symbol" === Cf(t) ? t : String(t)
                 }()) in e ? Object.defineProperty(e, n, {
                     value: t,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : e[n] = t
-            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(r)) : kf(Object(r)).forEach(function(t) {
+            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(r)) : Lf(Object(r)).forEach(function(t) {
                 Object.defineProperty(a, t, Object.getOwnPropertyDescriptor(r, t))
             })
         }
         return a
     }
 
-    function Mf(t, e) {
+    function Df(t, e) {
         var n;
-        if (t) return "string" == typeof t ? Ef(t, e) : "Map" === (n = "Object" === (n = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : n) || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? Ef(t, e) : void 0
+        if (t) return "string" == typeof t ? Tf(t, e) : "Map" === (n = "Object" === (n = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : n) || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? Tf(t, e) : void 0
     }
 
-    function Ef(t, e) {
+    function Tf(t, e) {
         (null == e || e > t.length) && (e = t.length);
         for (var n = 0, a = new Array(e); n < e; n++) a[n] = t[n];
         return a
     }
 
-    function Cf(t) {
+    function zf(t) {
         var e, n = t.id,
             a = t.className,
             r = t.style,
             o = t.draggerClassName,
             i = t.draggerStyle,
             l = t.key,
             c = t.locale,
@@ -123630,24 +123774,25 @@
             D = t.setProps,
             c = (t = Object(Wt.useContext)(G.a)) && t.locale || c,
             T = (A = E = E || [], e = new Map, A.forEach(function(t) {
                 e.set(t.uid, t.completeTimestamp)
             }), e);
         Object(Wt.useEffect)(function() {
             h || (C && 0 < C.length ? D({
-                uploadId: C[0].taskId || Object(Wd.a)()
+                uploadId: C[0].taskId || Object(Xd.a)()
             }) : D({
-                uploadId: Object(Wd.a)()
+                uploadId: Object(Xd.a)()
             }))
         }, []), A = Object(Wt.useState)(C || E.map(function(t) {
             return {
                 name: t.fileName,
                 status: t.taskStatus,
                 uid: t.uid,
-                url: t.url
+                url: t.url,
+                fileSize: t.fileSize
             }
         })), z = 2;
         var z = (A = function(t) {
                 if (Array.isArray(t)) return t
             }(A) || function(t, e) {
                 var n = null == t ? null : "undefined" != typeof Symbol && t[Symbol.iterator] || t["@@iterator"];
                 if (null != n) {
@@ -123667,15 +123812,15 @@
                             if (!c && null != n.return && (i = n.return(), Object(i) !== i)) return
                         } finally {
                             if (s) throw r
                         }
                     }
                     return l
                 }
-            }(A, z) || Mf(A, z) || function() {
+            }(A, z) || Df(A, z) || function() {
                 throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
             }())[0],
             R = A[1],
             A = {
                 name: "file",
                 action: s + "?uploadId=".concat(h),
                 headers: u,
@@ -123689,15 +123834,15 @@
                 onChange: function(t) {
                     var e, n = "removed" === t.file.status ? 0 : t.fileList.length - E.length,
                         t = (y || x ? "removed" === t.file.status ? D({
                             listUploadTaskRecord: t.fileList.map(function(t) {
                                 var e = d && "done" === t.status ? {
                                     url: d + "?taskId=".concat(h, "&filename=").concat(t.name)
                                 } : {};
-                                return jf({
+                                return Pf({
                                     fileName: t.name,
                                     fileSize: t.size,
                                     completeTimestamp: T.get(t.uid) || (new Date).getTime(),
                                     taskStatus: "done" === t.status ? "success" : "failed",
                                     taskId: h,
                                     uid: t.uid
                                 }, e)
@@ -123716,29 +123861,29 @@
                                     taskId: h
                                 }
                             }),
                             listUploadTaskRecord: t.fileList.map(function(t) {
                                 var e = d && "done" === t.status ? {
                                     url: d + "?taskId=".concat(h, "&filename=").concat(t.name)
                                 } : {};
-                                return jf({
+                                return Pf({
                                     fileName: t.name,
                                     fileSize: t.size,
                                     completeTimestamp: T.get(t.uid) || (new Date).getTime(),
                                     taskStatus: "done" === t.status ? "success" : "failed",
                                     taskId: h,
                                     uid: t.uid
                                 }, e)
                             })
                         }) : "removed" === t.file.status ? D({
                             listUploadTaskRecord: t.fileList.map(function(t) {
                                 var e = d && "done" === t.status ? {
                                     url: d + "?taskId=".concat(h, "&filename=").concat(t.name)
                                 } : {};
-                                return jf({
+                                return Pf({
                                     fileName: t.name,
                                     fileSize: t.size,
                                     completeTimestamp: T.get(t.uid) || (new Date).getTime(),
                                     taskStatus: "done" === t.status ? "success" : "failed",
                                     taskId: h,
                                     uid: t.uid
                                 }, e)
@@ -123751,53 +123896,53 @@
                                 taskStatus: "done" === t.file.status ? "success" : "failed",
                                 taskId: h
                             },
                             listUploadTaskRecord: t.fileList.map(function(t) {
                                 var e = d && "done" === t.status ? {
                                     url: d + "?taskId=".concat(h, "&filename=").concat(t.name)
                                 } : {};
-                                return jf({
+                                return Pf({
                                     fileName: t.name,
                                     fileSize: t.size,
                                     completeTimestamp: T.get(t.uid) || (new Date).getTime(),
                                     taskStatus: "done" === t.status ? "success" : "failed",
                                     taskId: h,
                                     uid: t.uid
                                 }, e)
                             })
                         }), "done" === t.file.status && j ? $.b.success("".concat(t.file.name, " 上传成功！")) : "error" === t.file.status && M && $.b.error("".concat(t.file.name, " 上传失败！")), function(t) {
-                            if (Array.isArray(t)) return Ef(t)
+                            if (Array.isArray(t)) return Tf(t)
                         }(e = t.fileList) || function() {
                             if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
-                        }() || Mf(e) || function() {
+                        }() || Df(e) || function() {
                             throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                         }());
                     m && (t = t.slice(-m)), 0 != n && (t = t.slice(0, t.length - n).concat(t.slice(-n).map(function(t) {
                         return "error" !== t.status && t.status || (t.status = "error", t.response = _ || "上传失败"), t
                     }))), R(d ? t.map(function(t) {
-                        return jf(jf({}, t), {}, {
+                        return Pf(Pf({}, t), {}, {
                             url: d + "?taskId=".concat(h, "&filename=").concat(t.name)
                         })
                     }) : t)
                 }
             };
         return g && 0 != g.length && Object.assign(A, {
             accept: "." + g.join(",.")
         }), H.a.createElement(W.a, {
             locale: K.b.get(c)
         }, H.a.createElement("div", {
             id: n,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
-            style: jf(jf({
+            style: Pf(Pf({
                 border: "1px solid transparent",
                 transition: "border 0.3s"
-            }, Pf.get(L)), r),
+            }, If.get(L)), r),
             key: l,
             "data-dash-is-loading": P && P.is_loading || void 0
-        }, H.a.createElement(Lf, wf({
+        }, H.a.createElement(Rf, Sf({
             draggerStyle: i,
             draggerClassName: Object(V.isString)(o) ? o : o ? Object(U.a)(o) : void 0,
             fileList: z,
             showUploadList: v,
             multiple: y,
             directory: x,
             disabled: t && !Object(V.isUndefined)(t.componentDisabled) ? t.componentDisabled : S,
@@ -123806,15 +123951,15 @@
                 strokeWidth: k && k.strokeWidth || 2,
                 format: w ? function(t) {
                     return t && "".concat(k && k.prefix || "").concat(parseFloat(t.toFixed(1))).concat(k && k.suffix || "%")
                 } : void 0
             } : void 0,
             onRemove: O ? function() {
                 return new Promise(function(t, e) {
-                    dr.confirm({
+                    hr.confirm({
                         title: K.a.AntdPictureUpload[c].confirmBeforeDeleteTitle,
                         okText: K.a.AntdPictureUpload[c].confirmBeforeDeleteOkText,
                         cancelText: K.a.AntdPictureUpload[c].confirmBeforeDeleteCancelText,
                         onOk: function() {
                             t(!0)
                         }
                     })
@@ -123827,36 +123972,36 @@
         })), H.a.createElement("p", {
             className: "ant-upload-text"
         }, p), H.a.createElement("p", {
             className: "ant-upload-hint"
         }, f))))
     }
 
-    function Sf(t, e) {
-        return Wt.createElement(to.a, Object(Ct.a)(Object(Ct.a)({}, t), {}, {
+    function Af(t, e) {
+        return Wt.createElement(ao.a, Object(Ct.a)(Object(Ct.a)({}, t), {}, {
             ref: e,
-            icon: Tf
+            icon: Yf
         }))
     }
-    var Lf = Pp.Dragger,
-        Pf = new Map([
+    var Rf = Ip.Dragger,
+        If = new Map([
             ["warning", {
                 border: "1px solid #faad14",
                 borderRadius: "2px",
                 padding: "6px 10px",
                 transition: "border 0.3s"
             }],
             ["error", {
                 border: "1px solid #ff4d4f",
                 borderRadius: "2px",
                 padding: "6px 10px",
                 transition: "border 0.3s"
             }]
         ]),
-        Df = (Cf.propTypes = {
+        Nf = (zf.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             draggerClassName: n.a.oneOfType([n.a.string, n.a.object]),
             draggerStyle: n.a.object,
             locale: n.a.oneOf(["zh-cn", "en-us"]),
@@ -123919,40 +124064,41 @@
                 url: n.a.string
             }))]),
             defaultFileList: n.a.arrayOf(n.a.exact({
                 name: n.a.string,
                 status: n.a.oneOf(["done", "error", "removed"]),
                 uid: n.a.any,
                 url: n.a.string,
-                taskId: n.a.string
+                taskId: n.a.string,
+                fileSize: n.a.number
             })),
             disabled: n.a.bool,
             status: n.a.oneOf(["error", "warning"]),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, Cf.defaultProps = {
+        }, zf.defaultProps = {
             disabled: !1,
             multiple: !1,
             directory: !1,
             showUploadList: !0,
             fileListMaxLength: null,
             fileMaxSize: 500,
             confirmBeforeDelete: !1,
             showPercent: !1,
             showSuccessMessage: !0,
             showErrorMessage: !0,
             lastUploadTaskRecord: null,
             listUploadTaskRecord: [],
             locale: "zh-cn"
-        }, Cf),
-        Tf = {
+        }, zf),
+        Yf = {
             icon: {
                 tag: "svg",
                 attrs: {
                     viewBox: "64 64 896 896",
                     focusable: "false"
                 },
                 children: [{
@@ -123961,81 +124107,81 @@
                         d: "M400 317.7h73.9V656c0 4.4 3.6 8 8 8h60c4.4 0 8-3.6 8-8V317.7H624c6.7 0 10.4-7.7 6.3-12.9L518.3 163a8 8 0 00-12.6 0l-112 141.7c-4.1 5.3-.4 13 6.3 13zM878 626h-60c-4.4 0-8 3.6-8 8v154H214V634c0-4.4-3.6-8-8-8h-60c-4.4 0-8 3.6-8 8v198c0 17.7 14.3 32 32 32h684c17.7 0 32-14.3 32-32V634c0-4.4-3.6-8-8-8z"
                     }
                 }]
             },
             name: "upload",
             theme: "outlined"
         },
-        zf = (Sf.displayName = "UploadOutlined", Wt.forwardRef(Sf));
+        Bf = (Af.displayName = "UploadOutlined", Wt.forwardRef(Af));
 
-    function Af(t) {
-        return (Af = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
+    function Ff(t) {
+        return (Ff = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
             return typeof t
         } : function(t) {
             return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
         })(t)
     }
 
-    function Rf() {
-        return (Rf = Object.assign ? Object.assign.bind() : function(t) {
+    function Hf() {
+        return (Hf = Object.assign ? Object.assign.bind() : function(t) {
             for (var e = 1; e < arguments.length; e++) {
                 var n, a = arguments[e];
                 for (n in a) Object.prototype.hasOwnProperty.call(a, n) && (t[n] = a[n])
             }
             return t
         }).apply(this, arguments)
     }
 
-    function If(e, t) {
+    function Wf(e, t) {
         var n, a = Object.keys(e);
         return Object.getOwnPropertySymbols && (n = Object.getOwnPropertySymbols(e), t && (n = n.filter(function(t) {
             return Object.getOwnPropertyDescriptor(e, t).enumerable
         })), a.push.apply(a, n)), a
     }
 
-    function Nf(a) {
+    function Vf(a) {
         for (var t = 1; t < arguments.length; t++) {
             var r = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? If(Object(r), !0).forEach(function(t) {
+            t % 2 ? Wf(Object(r), !0).forEach(function(t) {
                 var e, n;
                 e = a, t = r[n = t], (n = function() {
                     var t = function(t) {
-                        if ("object" !== Af(t) || null === t) return t;
+                        if ("object" !== Ff(t) || null === t) return t;
                         var e = t[Symbol.toPrimitive];
                         if (void 0 === e) return String(t);
                         e = e.call(t, "string");
-                        if ("object" !== Af(e)) return e;
+                        if ("object" !== Ff(e)) return e;
                         throw new TypeError("@@toPrimitive must return a primitive value.")
                     }(n);
-                    return "symbol" === Af(t) ? t : String(t)
+                    return "symbol" === Ff(t) ? t : String(t)
                 }()) in e ? Object.defineProperty(e, n, {
                     value: t,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : e[n] = t
-            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(r)) : If(Object(r)).forEach(function(t) {
+            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(r)) : Wf(Object(r)).forEach(function(t) {
                 Object.defineProperty(a, t, Object.getOwnPropertyDescriptor(r, t))
             })
         }
         return a
     }
 
-    function Yf(t, e) {
+    function Kf(t, e) {
         var n;
-        if (t) return "string" == typeof t ? Bf(t, e) : "Map" === (n = "Object" === (n = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : n) || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? Bf(t, e) : void 0
+        if (t) return "string" == typeof t ? Uf(t, e) : "Map" === (n = "Object" === (n = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : n) || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? Uf(t, e) : void 0
     }
 
-    function Bf(t, e) {
+    function Uf(t, e) {
         (null == e || e > t.length) && (e = t.length);
         for (var n = 0, a = new Array(e); n < e; n++) a[n] = t[n];
         return a
     }
 
-    function Ff(t) {
+    function Gf(t) {
         var e, n = t.id,
             a = t.className,
             r = t.style,
             o = t.key,
             i = t.locale,
             l = t.apiUrl,
             c = t.headers,
@@ -124062,24 +124208,25 @@
             S = t.setProps,
             i = (t = Object(Wt.useContext)(G.a)) && t.locale || i,
             L = (T = k = k || [], e = new Map, T.forEach(function(t) {
                 e.set(t.uid, t.completeTimestamp)
             }), e);
         Object(Wt.useEffect)(function() {
             u || (j && 0 < j.length ? S({
-                uploadId: j[0].taskId || Object(Wd.a)()
+                uploadId: j[0].taskId || Object(Xd.a)()
             }) : S({
-                uploadId: Object(Wd.a)()
+                uploadId: Object(Xd.a)()
             }))
         }, []), T = Object(Wt.useState)(j || k.map(function(t) {
             return {
                 name: t.fileName,
                 status: t.taskStatus,
                 uid: t.uid,
-                url: t.url
+                url: t.url,
+                fileSize: t.fileSize
             }
         })), P = 2;
         var P = (T = function(t) {
                 if (Array.isArray(t)) return t
             }(T) || function(t, e) {
                 var n = null == t ? null : "undefined" != typeof Symbol && t[Symbol.iterator] || t["@@iterator"];
                 if (null != n) {
@@ -124099,15 +124246,15 @@
                             if (!c && null != n.return && (i = n.return(), Object(i) !== i)) return
                         } finally {
                             if (s) throw r
                         }
                     }
                     return l
                 }
-            }(T, P) || Yf(T, P) || function() {
+            }(T, P) || Kf(T, P) || function() {
                 throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
             }())[0],
             D = T[1],
             T = {
                 name: "file",
                 action: l + "?uploadId=".concat(u),
                 headers: c,
@@ -124121,15 +124268,15 @@
                 onChange: function(t) {
                     var e, n = "removed" === t.file.status ? 0 : t.fileList.length - k.length,
                         t = (g || b ? "removed" === t.file.status ? S({
                             listUploadTaskRecord: t.fileList.map(function(t) {
                                 var e = s && "done" === t.status ? {
                                     url: s + "?taskId=".concat(u, "&filename=").concat(t.name)
                                 } : {};
-                                return Nf({
+                                return Vf({
                                     fileName: t.name,
                                     fileSize: t.size,
                                     completeTimestamp: L.get(t.uid) || (new Date).getTime(),
                                     taskStatus: "done" === t.status ? "success" : "failed",
                                     taskId: u,
                                     uid: t.uid
                                 }, e)
@@ -124148,29 +124295,29 @@
                                     taskId: u
                                 }
                             }),
                             listUploadTaskRecord: t.fileList.map(function(t) {
                                 var e = s && "done" === t.status ? {
                                     url: s + "?taskId=".concat(u, "&filename=").concat(t.name)
                                 } : {};
-                                return Nf({
+                                return Vf({
                                     fileName: t.name,
                                     fileSize: t.size,
                                     completeTimestamp: L.get(t.uid) || (new Date).getTime(),
                                     taskStatus: "done" === t.status ? "success" : "failed",
                                     taskId: u,
                                     uid: t.uid
                                 }, e)
                             })
                         }) : "removed" === t.file.status ? S({
                             listUploadTaskRecord: t.fileList.map(function(t) {
                                 var e = s && "done" === t.status ? {
                                     url: s + "?taskId=".concat(u, "&filename=").concat(t.name)
                                 } : {};
-                                return Nf({
+                                return Vf({
                                     fileName: t.name,
                                     fileSize: t.size,
                                     completeTimestamp: L.get(t.uid) || (new Date).getTime(),
                                     taskStatus: "done" === t.status ? "success" : "failed",
                                     taskId: u,
                                     uid: t.uid
                                 }, e)
@@ -124183,97 +124330,97 @@
                                 taskStatus: "done" === t.file.status ? "success" : "failed",
                                 taskId: u
                             },
                             listUploadTaskRecord: t.fileList.map(function(t) {
                                 var e = s && "done" === t.status ? {
                                     url: s + "?taskId=".concat(u, "&filename=").concat(t.name)
                                 } : {};
-                                return Nf({
+                                return Vf({
                                     fileName: t.name,
                                     fileSize: t.size,
                                     completeTimestamp: L.get(t.uid) || (new Date).getTime(),
                                     taskStatus: "done" === t.status ? "success" : "failed",
                                     taskId: u,
                                     uid: t.uid
                                 }, e)
                             })
                         }), "done" === t.file.status && O ? $.b.success("".concat(t.file.name, " 上传成功！")) : "error" === t.file.status && w && $.b.error("".concat(t.file.name, " 上传失败！")), function(t) {
-                            if (Array.isArray(t)) return Bf(t)
+                            if (Array.isArray(t)) return Uf(t)
                         }(e = t.fileList) || function() {
                             if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
-                        }() || Yf(e) || function() {
+                        }() || Kf(e) || function() {
                             throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                         }());
                     d && (t = t.slice(-d)), 0 != n && (t = t.slice(0, t.length - n).concat(t.slice(-n).map(function(t) {
                         return "error" !== t.status && t.status || (t.status = "error", t.response = v || "上传失败"), t
                     }))), D(s ? t.map(function(t) {
-                        return Nf(Nf({}, t), {}, {
+                        return Vf(Vf({}, t), {}, {
                             url: s + "?taskId=".concat(u, "&filename=").concat(t.name)
                         })
                     }) : t)
                 }
             };
         return f && 0 != f.length && Object.assign(T, {
             accept: "." + f.join(",.")
         }), H.a.createElement(W.a, {
             locale: K.b.get(i)
         }, H.a.createElement("div", {
             id: n,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
-            style: Nf(Nf({
+            style: Vf(Vf({
                 border: "1px solid transparent",
                 transition: "border 0.3s"
-            }, Hf.get(E)), r),
+            }, qf.get(E)), r),
             key: o
-        }, H.a.createElement(Pp, Rf({}, T, {
+        }, H.a.createElement(Ip, Hf({}, T, {
             fileList: P,
             multiple: g,
             showUploadList: m,
             directory: b,
             disabled: t && !Object(V.isUndefined)(t.componentDisabled) ? t.componentDisabled : M,
             progress: _ || x ? {
                 strokeColor: _ && _.strokeColor,
                 strokeWidth: _ && _.strokeWidth || 2,
                 format: x ? function(t) {
                     return t && "".concat(_ && _.prefix || "").concat(parseFloat(t.toFixed(1))).concat(_ && _.suffix || "%")
                 } : void 0
             } : void 0,
             onRemove: y ? function() {
                 return new Promise(function(t, e) {
-                    dr.confirm({
+                    hr.confirm({
                         title: K.a.AntdPictureUpload[i].confirmBeforeDeleteTitle,
                         okText: K.a.AntdPictureUpload[i].confirmBeforeDeleteOkText,
                         cancelText: K.a.AntdPictureUpload[i].confirmBeforeDeleteCancelText,
                         onOk: function() {
                             t(!0)
                         }
                     })
                 })
             } : void 0,
             "data-dash-is-loading": C && C.is_loading || void 0
         }), H.a.createElement(z.a, {
-            icon: H.a.createElement(zf, null),
+            icon: H.a.createElement(Bf, null),
             disabled: t && !Object(V.isUndefined)(t.componentDisabled) ? t.componentDisabled : M
         }, p || "点击上传文件"))))
     }
-    var Hf = new Map([
+    var qf = new Map([
             ["warning", {
                 border: "1px solid #faad14",
                 borderRadius: "2px",
                 padding: "6px 10px",
                 transition: "border 0.3s"
             }],
             ["error", {
                 border: "1px solid #ff4d4f",
                 borderRadius: "2px",
                 padding: "6px 10px",
                 transition: "border 0.3s"
             }]
         ]),
-        Wf = (Ff.propTypes = {
+        Xf = (Gf.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             locale: n.a.oneOf(["zh-cn", "en-us"]),
             apiUrl: n.a.string,
             headers: n.a.object,
@@ -124325,47 +124472,48 @@
                 url: n.a.string
             })),
             defaultFileList: n.a.arrayOf(n.a.exact({
                 name: n.a.string,
                 status: n.a.oneOf(["done", "error", "removed"]),
                 uid: n.a.any,
                 url: n.a.string,
-                taskId: n.a.string
+                taskId: n.a.string,
+                fileSize: n.a.number
             })),
             disabled: n.a.bool,
             status: n.a.oneOf(["error", "warning"]),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, Ff.defaultProps = {
+        }, Gf.defaultProps = {
             disabled: !1,
             multiple: !1,
             directory: !1,
             showUploadList: !0,
             fileListMaxLength: null,
             fileMaxSize: 500,
             confirmBeforeDelete: !1,
             showPercent: !1,
             showSuccessMessage: !0,
             showErrorMessage: !0,
             lastUploadTaskRecord: null,
             listUploadTaskRecord: [],
             locale: "zh-cn"
-        }, Ff);
+        }, Gf);
 
-    function Vf(t, e) {
+    function $f(t, e) {
         (null == e || e > t.length) && (e = t.length);
         for (var n = 0, a = new Array(e); n < e; n++) a[n] = t[n];
         return a
     }
 
-    function Kf(t) {
+    function Zf(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.children,
             i = t.skeletonContent,
             l = t.loading,
@@ -124398,15 +124546,15 @@
                             if (s) throw r
                         }
                     }
                     return l
                 }
             }(t, l) || function(t, e) {
                 var n;
-                if (t) return "string" == typeof t ? Vf(t, e) : "Map" === (n = "Object" === (n = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : n) || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? Vf(t, e) : void 0
+                if (t) return "string" == typeof t ? $f(t, e) : "Map" === (n = "Object" === (n = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : n) || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? $f(t, e) : void 0
             }(t, l) || function() {
                 throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
             }())[0],
             h = t[1],
             m = Object(Wt.useRef)();
         return Object(Wt.useEffect)(function() {
             p && (m.current && clearTimeout(m.current), p.is_loading && !f ? "default" === c ? (d && console.log(p.component_name + "." + p.prop_name), h(!0)) : "exclude" === c ? -1 === s.indexOf(p.component_name + "." + p.prop_name) && (d && console.log(p.component_name + "." + p.prop_name), h(!0)) : "include" === c && -1 !== u.indexOf(p.component_name + "." + p.prop_name) && (d && console.log(p.component_name + "." + p.prop_name), h(!0)) : !p.is_loading && f && (m.current = setTimeout(function() {
@@ -124417,92 +124565,92 @@
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             "data-dash-is-loading": p && p.is_loading || void 0
         }, f ? i : o)
     }
 
-    function Uf(t) {
+    function Jf(t) {
         var e = t.id,
             n = t.style,
             a = t.className,
             r = t.key,
             o = t.active,
             i = t.shape,
             l = t.size,
             c = t.loading_state;
-        return t.setProps, H.a.createElement(Dl.Avatar, {
+        return t.setProps, H.a.createElement(Al.Avatar, {
             id: e,
             style: n,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             key: r,
             active: o,
             shape: i,
             size: l,
             "data-dash-is-loading": c && c.is_loading || void 0
         })
     }
 
-    function Gf(t) {
+    function Qf(t) {
         var e = t.id,
             n = t.style,
             a = t.className,
             r = t.key,
             o = t.active,
             i = t.block,
             l = t.shape,
             c = t.size,
             s = t.loading_state;
-        return t.setProps, H.a.createElement(Dl.Button, {
+        return t.setProps, H.a.createElement(Al.Button, {
             id: e,
             style: n,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             key: r,
             active: o,
             block: i,
             shape: l,
             size: c,
             "data-dash-is-loading": s && s.is_loading || void 0
         })
     }
 
-    function qf(t) {
+    function th(t) {
         var e = t.id,
             n = t.style,
             a = t.className,
             r = t.key,
             o = t.active,
             i = t.size,
             l = t.loading_state;
-        return t.setProps, H.a.createElement(Dl.Input, {
+        return t.setProps, H.a.createElement(Al.Input, {
             id: e,
             style: n,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             key: r,
             active: o,
             size: i,
             "data-dash-is-loading": l && l.is_loading || void 0
         })
     }
 
-    function Xf(t) {
+    function eh(t) {
         var e = t.id,
             n = t.style,
             a = t.className,
             r = t.key,
             o = t.loading_state;
-        return t.setProps, H.a.createElement(Dl.Image, {
+        return t.setProps, H.a.createElement(Al.Image, {
             id: e,
             style: n,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             key: r,
             "data-dash-is-loading": o && o.is_loading || void 0
         })
     }
-    Kf._dashprivate_isLoadingComponent = !0, Kf.propTypes = {
+    Zf._dashprivate_isLoadingComponent = !0, Zf.propTypes = {
         id: n.a.string,
         children: n.a.node,
         skeletonContent: n.a.node,
         className: n.a.oneOfType([n.a.string, n.a.object]),
         style: n.a.object,
         key: n.a.string,
         loading: n.a.bool,
@@ -124512,155 +124660,155 @@
         includeProps: n.a.arrayOf(n.a.string),
         loading_state: n.a.shape({
             is_loading: n.a.bool,
             prop_name: n.a.string,
             component_name: n.a.string
         }),
         setProps: n.a.func
-    }, Kf.defaultProps = {
+    }, Zf.defaultProps = {
         loading: !1,
         listenPropsMode: "default",
         excludeProps: [],
         includeProps: [],
         debug: !1
     };
-    var $f = Kf,
-        Zf = (Uf.propTypes = {
+    var nh = Zf,
+        ah = (Jf.propTypes = {
             id: n.a.string,
             style: n.a.object,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             key: n.a.string,
             active: n.a.bool,
             shape: n.a.oneOf(["circle", "square"]),
             size: n.a.oneOfType([n.a.number, n.a.oneOf(["large", "small", "default"])]),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, Uf.defaultProps = {
+        }, Jf.defaultProps = {
             active: !1,
             shape: "circle",
             size: "default"
-        }, Uf),
-        Jf = (Gf.propTypes = {
+        }, Jf),
+        rh = (Qf.propTypes = {
             id: n.a.string,
             style: n.a.object,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             key: n.a.string,
             active: n.a.bool,
             block: n.a.bool,
             shape: n.a.oneOf(["circle", "round", "default"]),
             size: n.a.oneOf(["large", "small", "default"]),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, Gf.defaultProps = {
+        }, Qf.defaultProps = {
             active: !1,
             block: !1,
             shape: "default",
             size: "default"
-        }, Gf),
-        Qf = (qf.propTypes = {
+        }, Qf),
+        oh = (th.propTypes = {
             id: n.a.string,
             style: n.a.object,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             key: n.a.string,
             active: n.a.bool,
             size: n.a.oneOf(["large", "small", "default"]),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, qf.defaultProps = {
+        }, th.defaultProps = {
             active: !1,
             size: "default"
-        }, qf),
-        th = (Xf.propTypes = {
+        }, th),
+        ih = (eh.propTypes = {
             id: n.a.string,
             style: n.a.object,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             key: n.a.string,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, Xf.defaultProps = {}, Xf);
+        }, eh.defaultProps = {}, eh);
 
-    function eh(t) {
-        return (eh = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
+    function lh(t) {
+        return (lh = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
             return typeof t
         } : function(t) {
             return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
         })(t)
     }
 
-    function nh(t) {
+    function ch(t) {
         return function(t) {
-            if (Array.isArray(t)) return ah(t)
+            if (Array.isArray(t)) return sh(t)
         }(t) || function() {
             if ("undefined" != typeof Symbol && null != t[Symbol.iterator] || null != t["@@iterator"]) return Array.from(t)
         }() || function(t) {
             var e;
-            if (t) return "string" == typeof t ? ah(t, void 0) : "Map" === (e = "Object" === (e = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : e) || "Set" === e ? Array.from(t) : "Arguments" === e || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(e) ? ah(t, void 0) : void 0
+            if (t) return "string" == typeof t ? sh(t, void 0) : "Map" === (e = "Object" === (e = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : e) || "Set" === e ? Array.from(t) : "Arguments" === e || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(e) ? sh(t, void 0) : void 0
         }(t) || function() {
             throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function ah(t, e) {
+    function sh(t, e) {
         (null == e || e > t.length) && (e = t.length);
         for (var n = 0, a = new Array(e); n < e; n++) a[n] = t[n];
         return a
     }
 
-    function rh(e, t) {
+    function uh(e, t) {
         var n, a = Object.keys(e);
         return Object.getOwnPropertySymbols && (n = Object.getOwnPropertySymbols(e), t && (n = n.filter(function(t) {
             return Object.getOwnPropertyDescriptor(e, t).enumerable
         })), a.push.apply(a, n)), a
     }
 
-    function oh(a) {
+    function dh(a) {
         for (var t = 1; t < arguments.length; t++) {
             var r = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? rh(Object(r), !0).forEach(function(t) {
+            t % 2 ? uh(Object(r), !0).forEach(function(t) {
                 var e, n;
                 e = a, t = r[n = t], (n = function() {
                     var t = function(t) {
-                        if ("object" !== eh(t) || null === t) return t;
+                        if ("object" !== lh(t) || null === t) return t;
                         var e = t[Symbol.toPrimitive];
                         if (void 0 === e) return String(t);
                         e = e.call(t, "string");
-                        if ("object" !== eh(e)) return e;
+                        if ("object" !== lh(e)) return e;
                         throw new TypeError("@@toPrimitive must return a primitive value.")
                     }(n);
-                    return "symbol" === eh(t) ? t : String(t)
+                    return "symbol" === lh(t) ? t : String(t)
                 }()) in e ? Object.defineProperty(e, n, {
                     value: t,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : e[n] = t
-            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(r)) : rh(Object(r)).forEach(function(t) {
+            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(r)) : uh(Object(r)).forEach(function(t) {
                 Object.defineProperty(a, t, Object.getOwnPropertyDescriptor(r, t))
             })
         }
         return a
     }
 
-    function ih(t) {
+    function ph(t) {
         var e = t.id,
             n = t.key,
             a = t.className,
             r = t.style,
             o = t.size,
             i = t.bordered,
             l = t.controls,
@@ -124679,43 +124827,43 @@
             x = t.colorBlockPosition,
             _ = t.colorBlockStyle,
             O = t.pureLegendLabelStyle,
             w = t.loading_state,
             k = t.setProps,
             c = (t = Object(Wt.useContext)(G.a)) && !Object(V.isUndefined)(t.componentDisabled) ? t.componentDisabled : c,
             o = t && !Object(V.isUndefined)(t.componentSize) ? t.componentSize : o;
-        return H.a.createElement(za.b, {
+        return H.a.createElement(Ia.b, {
             id: e,
             key: n,
-            style: oh({
+            style: dh({
                 borderRadius: "2px",
                 padding: "12px 20px"
             }, r),
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             direction: "vertical",
             "data-dash-is-loading": w && w.is_loading || void 0
         }, b.slice(0, b.length - 1).map(function(t, n) {
-            return H.a.createElement(za.b, {
+            return H.a.createElement(Ia.b, {
                 style: {
                     display: "flex"
                 },
                 size: "small"
             }, "left" === x ? H.a.createElement("div", {
-                style: oh({
-                    height: sh.get(o),
+                style: dh({
+                    height: mh.get(o),
                     backgroundColor: v[n],
-                    width: sh.get(o)
+                    width: mh.get(o)
                 }, _)
-            }) : null, g ? H.a.createElement(H.a.Fragment, null, H.a.createElement(ch, {
+            }) : null, g ? H.a.createElement(H.a.Fragment, null, H.a.createElement(hh, {
                 style: O
-            }, b[n].toFixed(h)), H.a.createElement(ch, {
+            }, b[n].toFixed(h)), H.a.createElement(hh, {
                 style: O
-            }, "~"), H.a.createElement(ch, {
+            }, "~"), H.a.createElement(hh, {
                 style: O
-            }, b[n + 1].toFixed(h))) : H.a.createElement(H.a.Fragment, null, H.a.createElement(Ql.a, {
+            }, b[n + 1].toFixed(h))) : H.a.createElement(H.a.Fragment, null, H.a.createElement(oc.a, {
                 style: y,
                 size: o,
                 bordered: i,
                 controls: l,
                 disabled: c,
                 keyboard: s,
                 placeholder: u,
@@ -124723,24 +124871,24 @@
                 max: p,
                 step: f,
                 precision: h,
                 readOnly: m,
                 value: b[n],
                 onChange: function(t) {
                     var e;
-                    null !== t && 0 === n && t < b[n + 1] ? ((e = nh(b))[n] = t, k({
+                    null !== t && 0 === n && t < b[n + 1] ? ((e = ch(b))[n] = t, k({
                         breakpoints: e
-                    })) : null !== t && 0 < n && t > b[n - 1] && t < b[n + 1] ? ((e = nh(b))[n] = t, k({
+                    })) : null !== t && 0 < n && t > b[n - 1] && t < b[n + 1] ? ((e = ch(b))[n] = t, k({
                         breakpoints: e
                     })) : null !== t && $.b.warning({
                         content: "数值超出相邻断点，请调整后再输入！",
                         duration: 1.5
                     })
                 }
-            }), H.a.createElement("span", null, "~"), H.a.createElement(Ql.a, {
+            }), H.a.createElement("span", null, "~"), H.a.createElement(oc.a, {
                 style: y,
                 size: o,
                 bordered: i,
                 controls: l,
                 disabled: c,
                 keyboard: s,
                 placeholder: u,
@@ -124748,66 +124896,66 @@
                 max: p,
                 step: f,
                 precision: h,
                 readOnly: m,
                 value: b[n + 1],
                 onChange: function(t) {
                     var e;
-                    null !== t && n === b.length - 2 && t > b[n] ? ((e = nh(b))[n + 1] = t, k({
+                    null !== t && n === b.length - 2 && t > b[n] ? ((e = ch(b))[n + 1] = t, k({
                         breakpoints: e
-                    })) : null !== t && t > b[n] && t < b[n + 2] ? ((e = nh(b))[n + 1] = t, k({
+                    })) : null !== t && t > b[n] && t < b[n + 2] ? ((e = ch(b))[n + 1] = t, k({
                         breakpoints: e
                     })) : null !== t && $.b.warning({
                         content: "数值超出相邻断点，请调整后再输入！",
                         duration: 1.5
                     })
                 }
             })), "right" === x ? H.a.createElement("div", {
-                style: oh({
-                    height: sh.get(o),
+                style: dh({
+                    height: mh.get(o),
                     backgroundColor: v[n],
-                    width: sh.get(o)
+                    width: mh.get(o)
                 }, _)
             }) : null)
         }))
     }
 
-    function lh(t) {
+    function fh(t) {
         var e = t.id,
             n = t.className,
             a = t.style,
             r = t.key,
             o = t.locale,
             i = t.text,
             l = t.beforeIcon,
             c = t.afterIcon,
             t = (t.setProps, t.loading_state),
             s = Object(Wt.useContext)(G.a),
             o = s && s.locale || o;
         return H.a.createElement(W.a, {
             locale: K.b.get(o)
-        }, H.a.createElement(dh, {
+        }, H.a.createElement(bh, {
             id: e,
             className: Object(V.isString)(n) ? n : n ? Object(U.a)(n) : void 0,
             style: a,
             key: r,
             copyable: {
                 text: i,
                 icon: [l, c]
             },
             "data-dash-is-loading": t && t.is_loading || void 0
         }))
     }
-    var ch = u.a.Text,
-        sh = new Map([
+    var hh = u.a.Text,
+        mh = new Map([
             ["small", "24px"],
             ["middle", "32px"],
             ["large", "40px"]
         ]),
-        uh = (ih.propTypes = {
+        gh = (ph.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             breakpoints: n.a.arrayOf(n.a.number).isRequired,
             colors: n.a.arrayOf(n.a.string).isRequired,
             controls: n.a.bool,
@@ -124828,50 +124976,50 @@
             pureLegendLabelStyle: n.a.object,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, ih.defaultProps = {
+        }, ph.defaultProps = {
             size: "middle",
             bordered: !0,
             controls: !0,
             disabled: !1,
             keyboard: !0,
             step: .01,
             precision: 2,
             colorBlockPosition: "right",
             pureLegend: !1
-        }, ih),
-        dh = u.a.Text,
-        ph = (lh.propTypes = {
+        }, ph),
+        bh = u.a.Text,
+        vh = (fh.propTypes = {
             id: n.a.string,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             key: n.a.string,
             locale: n.a.oneOf(["zh-cn", "en-us"]),
             text: n.a.string,
             beforeIcon: n.a.node,
             afterIcon: n.a.node,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, lh.defaultProps = {
+        }, fh.defaultProps = {
             locale: "zh-cn",
             text: ""
-        }, lh),
-        fh = e(718),
-        hh = e(521),
-        mh = e.n(hh);
+        }, fh),
+        yh = e(718),
+        xh = e(521),
+        _h = e.n(xh);
 
-    function gh(t, e) {
+    function Oh(t, e) {
         return function(t) {
             if (Array.isArray(t)) return t
         }(t) || function(t, e) {
             var n = null == t ? null : "undefined" != typeof Symbol && t[Symbol.iterator] || t["@@iterator"];
             if (null != n) {
                 var a, r, o, i, l = [],
                     c = !0,
@@ -124891,27 +125039,27 @@
                         if (s) throw r
                     }
                 }
                 return l
             }
         }(t, e) || function(t, e) {
             var n;
-            if (t) return "string" == typeof t ? bh(t, e) : "Map" === (n = "Object" === (n = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : n) || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? bh(t, e) : void 0
+            if (t) return "string" == typeof t ? wh(t, e) : "Map" === (n = "Object" === (n = Object.prototype.toString.call(t).slice(8, -1)) && t.constructor ? t.constructor.name : n) || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? wh(t, e) : void 0
         }(t, e) || function() {
             throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function bh(t, e) {
+    function wh(t, e) {
         (null == e || e > t.length) && (e = t.length);
         for (var n = 0, a = new Array(e); n < e; n++) a[n] = t[n];
         return a
     }
 
-    function vh(t) {
+    function kh(t) {
         var e = t.id,
             n = t.children,
             a = t.className,
             r = t.key,
             o = t.style,
             i = t.visible,
             l = t.title,
@@ -124920,26 +125068,26 @@
             u = t.closable,
             d = t.closeIconType,
             p = t.draggable,
             f = t.zIndex,
             h = t.bodyStyle,
             m = t.setProps,
             t = t.loading_state,
-            g = gh(Object(Wt.useState)(!1), 2),
+            g = Oh(Object(Wt.useState)(!1), 2),
             b = g[0],
             v = g[1],
-            y = (g = gh(Object(Wt.useState)({
+            y = (g = Oh(Object(Wt.useState)({
                 left: 0,
                 top: 0,
                 bottom: 0,
                 right: 0
             }), 2))[0],
             x = g[1],
             _ = Object(Wt.useRef)(null);
-        return H.a.createElement(dr, {
+        return H.a.createElement(hr, {
             id: e,
             className: Object(V.isString)(a) ? a : a ? Object(U.a)(a) : void 0,
             style: o,
             key: r,
             title: H.a.createElement("div", {
                 style: {
                     width: "100%",
@@ -124947,41 +125095,41 @@
                 },
                 onMouseOver: function() {
                     b && v(!1)
                 },
                 onMouseOut: function() {
                     v(!0)
                 }
-            }, l, u ? "outlined" === d ? H.a.createElement(Ya.a, {
+            }, l, u ? "outlined" === d ? H.a.createElement(Ha.a, {
                 style: {
                     position: "absolute",
                     top: -12,
                     right: -12,
                     fontSize: 24,
                     cursor: "pointer"
                 },
                 onClick: function() {
                     return m({
                         visible: !1
                     })
                 }
-            }) : "two-tone" == d ? H.a.createElement(fh.a, {
+            }) : "two-tone" == d ? H.a.createElement(yh.a, {
                 style: {
                     position: "absolute",
                     top: -12,
                     right: -12,
                     fontSize: 24,
                     cursor: "pointer"
                 },
                 onClick: function() {
                     return m({
                         visible: !1
                     })
                 }
-            }) : H.a.createElement(dn.a, {
+            }) : H.a.createElement(hn.a, {
                 style: {
                     position: "absolute",
                     top: -12,
                     right: -12,
                     fontSize: 24,
                     cursor: "pointer"
                 },
@@ -124998,15 +125146,15 @@
             bodyStyle: h,
             mask: !1,
             maskClosable: !1,
             closable: !1,
             footer: !1,
             wrapClassName: "ant-modal-wrap-overwrite",
             modalRender: p ? function(t) {
-                return H.a.createElement(mh.a, {
+                return H.a.createElement(_h.a, {
                     disabled: b,
                     bounds: y,
                     onStart: function(t, e) {
                         var n, a, r;
                         e = e, n = window.document.documentElement, a = n.clientWidth, n = n.clientHeight, (r = _.current.getBoundingClientRect()) && x({
                             left: -r.left + e.x,
                             right: a - (r.right - e.x),
@@ -125018,15 +125166,15 @@
                     ref: _
                 }, t))
             } : void 0,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n)
     }
 
-    function yh(t) {
+    function jh(t) {
         var e = t.id,
             n = t.children,
             a = t.key,
             r = t.primaryColor,
             o = t.componentDisabled,
             i = t.componentSize,
             l = t.locale,
@@ -125045,15 +125193,15 @@
             }
         }, H.a.createElement(W.a, {
             id: e,
             key: a,
             "data-dash-is-loading": t && t.is_loading || void 0
         }, n))
     }
-    vh.propTypes = {
+    kh.propTypes = {
         id: n.a.string,
         children: n.a.node,
         className: n.a.oneOfType([n.a.string, n.a.object]),
         style: n.a.object,
         key: n.a.string,
         title: n.a.node,
         visible: n.a.bool,
@@ -125066,126 +125214,126 @@
         bodyStyle: n.a.object,
         setProps: n.a.func,
         loading_state: n.a.shape({
             is_loading: n.a.bool,
             prop_name: n.a.string,
             component_name: n.a.string
         })
-    }, vh.defaultProps = {
+    }, kh.defaultProps = {
         transitionType: "fade",
         closeIconType: "default",
         draggable: !1,
         visible: !0,
         closable: !0,
         zIndex: 1e3
     };
-    var xh = vh,
-        _h = (yh.propTypes = {
+    var Mh = kh,
+        Eh = (jh.propTypes = {
             id: n.a.string,
             children: n.a.node,
             key: n.a.string,
             primaryColor: n.a.string,
             componentDisabled: n.a.bool,
             componentSize: n.a.oneOf(["small", "middle", "large"]),
             locale: n.a.oneOf(["zh-cn", "en-us"]),
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, yh.defaultProps = {}, yh),
-        Oh = e(117),
-        wh = function(t) {
+        }, jh.defaultProps = {}, jh),
+        Ch = e(117),
+        Sh = function(t) {
             var e = Object(Wt.useRef)(0),
-                t = Object(Tp.e)(Object(Wt.useState)(t), 2),
+                t = Object(Yp.e)(Object(Wt.useState)(t), 2),
                 n = t[0],
                 a = t[1],
                 t = Object(Wt.useCallback)(function(t) {
                     cancelAnimationFrame(e.current), e.current = requestAnimationFrame(function() {
                         a(t)
                     })
                 }, []);
-            return Object(Oh.a)(function() {
+            return Object(Ch.a)(function() {
                 cancelAnimationFrame(e.current)
             }), [n, t]
         },
-        kh = e(116),
-        jh = e(99);
+        Lh = e(116),
+        Ph = e(99);
 
-    function Mh(t, e) {
-        if (jh.a) return t ? Object(kh.a)(t) ? t() : "current" in t ? t.current : t : e
+    function Dh(t, e) {
+        if (Ph.a) return t ? Object(Lh.a)(t) ? t() : "current" in t ? t.current : t : e
     }
 
-    function Eh(t) {
+    function Th(t) {
         return function(n, a, r) {
             var o = Object(Wt.useRef)(!1),
                 i = Object(Wt.useRef)([]),
                 l = Object(Wt.useRef)([]),
                 c = Object(Wt.useRef)();
             t(function() {
                 var t, e = (Array.isArray(r) ? r : [r]).map(function(t) {
-                    return Mh(t)
+                    return Dh(t)
                 });
-                o.current ? e.length === i.current.length && Object(Ch.a)(e, i.current) && Object(Ch.a)(a, l.current) || (null != (t = c.current) && t.call(c), i.current = e, l.current = a, c.current = n()) : (o.current = !0, i.current = e, l.current = a, c.current = n())
-            }), Object(Oh.a)(function() {
+                o.current ? e.length === i.current.length && Object(zh.a)(e, i.current) && Object(zh.a)(a, l.current) || (null != (t = c.current) && t.call(c), i.current = e, l.current = a, c.current = n()) : (o.current = !0, i.current = e, l.current = a, c.current = n())
+            }), Object(Ch.a)(function() {
                 var t;
                 null != (t = c.current) && t.call(c), o.current = !1
             })
         }
     }
-    var Ch = e(213),
-        a = Eh(Wt.useEffect),
-        c = Eh(Wt.useLayoutEffect),
-        Sh = jh.a ? c : a;
+    var zh = e(213),
+        a = Th(Wt.useEffect),
+        c = Th(Wt.useLayoutEffect),
+        Ah = Ph.a ? c : a;
 
-    function Lh(t) {
-        return (Lh = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
+    function Rh(t) {
+        return (Rh = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
             return typeof t
         } : function(t) {
             return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
         })(t)
     }
 
-    function Ph(e, t) {
+    function Ih(e, t) {
         var n, a = Object.keys(e);
         return Object.getOwnPropertySymbols && (n = Object.getOwnPropertySymbols(e), t && (n = n.filter(function(t) {
             return Object.getOwnPropertyDescriptor(e, t).enumerable
         })), a.push.apply(a, n)), a
     }
 
-    function Dh(a) {
+    function Nh(a) {
         for (var t = 1; t < arguments.length; t++) {
             var r = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? Ph(Object(r), !0).forEach(function(t) {
+            t % 2 ? Ih(Object(r), !0).forEach(function(t) {
                 var e, n;
                 e = a, t = r[n = t], (n = function() {
                     var t = function(t) {
-                        if ("object" !== Lh(t) || null === t) return t;
+                        if ("object" !== Rh(t) || null === t) return t;
                         var e = t[Symbol.toPrimitive];
                         if (void 0 === e) return String(t);
                         e = e.call(t, "string");
-                        if ("object" !== Lh(e)) return e;
+                        if ("object" !== Rh(e)) return e;
                         throw new TypeError("@@toPrimitive must return a primitive value.")
                     }(n);
-                    return "symbol" === Lh(t) ? t : String(t)
+                    return "symbol" === Rh(t) ? t : String(t)
                 }()) in e ? Object.defineProperty(e, n, {
                     value: t,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : e[n] = t
-            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(r)) : Ph(Object(r)).forEach(function(t) {
+            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(r)) : Ih(Object(r)).forEach(function(t) {
                 Object.defineProperty(a, t, Object.getOwnPropertyDescriptor(r, t))
             })
         }
         return a
     }
 
-    function Th(t) {
+    function Yh(t) {
         var n, e, a, r = t.id,
             o = t.children,
             i = t.className,
             l = t.style,
             c = t.key,
             s = t.locale,
             u = t.contentClassName,
@@ -125195,23 +125343,23 @@
             h = t.labelPosition,
             m = t.open,
             g = t.maxHeight,
             b = t.transitionDuration,
             v = t.loading_state,
             y = t.setProps,
             t = Object(Wt.useRef)(null),
-            x = (n = t, x = Object(Tp.e)(wh(function() {
-                var t = Mh(n);
+            x = (n = t, x = Object(Yp.e)(Sh(function() {
+                var t = Dh(n);
                 return t ? {
                     width: t.clientWidth,
                     height: t.clientHeight
                 } : void 0
-            }), 2), e = x[0], a = x[1], Sh(function() {
-                var t, e = Mh(n);
-                if (e) return (t = new Is.a(function(t) {
+            }), 2), e = x[0], a = x[1], Ah(function() {
+                var t, e = Dh(n);
+                if (e) return (t = new Ws.a(function(t) {
                         t.forEach(function(t) {
                             var t = t.target,
                                 e = t.clientWidth,
                                 t = t.clientHeight;
                             a({
                                 width: e,
                                 height: t
@@ -125226,38 +125374,38 @@
             id: r,
             key: c,
             className: Object(V.isString)(i) ? i : i ? Object(U.a)(i) : void 0,
             style: l,
             "data-dash-is-loading": v && v.is_loading || void 0
         }, H.a.createElement("div", {
             className: Object(V.isString)(u) ? u : u ? Object(U.a)(u) : void 0,
-            style: Dh(Dh({
+            style: Nh(Nh({
                 transitionTimingFunction: "ease"
             }, d), {}, {
                 maxHeight: m ? x && x.height : g,
                 transitionDuration: "".concat(b, "s"),
                 transitionProperty: "max-height",
                 overflow: "hidden"
             })
         }, H.a.createElement("div", {
             ref: t
         }, o)), H.a.createElement("div", {
             style: {
                 textAlign: h
             }
-        }, H.a.createElement(zh, {
+        }, H.a.createElement(Bh, {
             onClick: function() {
                 y({
                     open: !m
                 })
             }
         }, m ? p || K.a.AntdSpoiler[s].hideLabel : f || K.a.AntdSpoiler[s].showLabel)))
     }
-    var zh = u.a.Link,
-        Ah = (Th.propTypes = {
+    var Bh = u.a.Link,
+        Fh = (Yh.propTypes = {
             id: n.a.string,
             children: n.a.node,
             className: n.a.oneOfType([n.a.string, n.a.object]),
             style: n.a.object,
             contentClassName: n.a.oneOfType([n.a.string, n.a.object]),
             contentStyle: n.a.object,
             key: n.a.string,
@@ -125270,209 +125418,209 @@
             transitionDuration: n.a.number,
             loading_state: n.a.shape({
                 is_loading: n.a.bool,
                 prop_name: n.a.string,
                 component_name: n.a.string
             }),
             setProps: n.a.func
-        }, Th.defaultProps = {
+        }, Yh.defaultProps = {
             locale: "zh-cn",
             open: !1,
             maxHeight: 50,
             transitionDuration: .1,
             labelPosition: "left"
-        }, Th);
+        }, Yh);
     e.d(t, "AntdDatePicker", function() {
         return _
     }), e.d(t, "AntdDateRangePicker", function() {
         return O
     }), e.d(t, "AntdDivider", function() {
         return k
     }), e.d(t, "AntdButton", function() {
         return M
     }), e.d(t, "AntdSelect", function() {
         return P
     }), e.d(t, "AntdTree", function() {
-        return rt
+        return ct
     }), e.d(t, "AntdTable", function() {
-        return ot.a
+        return st.a
     }), e.d(t, "AntdAnchor", function() {
-        return Yt
+        return Xt
     }), e.d(t, "AntdSlider", function() {
-        return ge
+        return xe
     }), e.d(t, "AntdTransfer", function() {
-        return Xe
+        return Je
     }), e.d(t, "AntdSteps", function() {
-        return An
+        return Nn
     }), e.d(t, "AntdMenu", function() {
-        return ia
-    }), e.d(t, "AntdCollapse", function() {
         return sa
+    }), e.d(t, "AntdCollapse", function() {
+        return pa
     }), e.d(t, "AntdRow", function() {
-        return da
+        return ha
     }), e.d(t, "AntdCol", function() {
-        return wa
+        return Ma
     }), e.d(t, "AntdLayout", function() {
-        return ja
+        return Ca
     }), e.d(t, "AntdHeader", function() {
-        return Ea
+        return La
     }), e.d(t, "AntdContent", function() {
-        return Sa
+        return Da
     }), e.d(t, "AntdFooter", function() {
-        return Pa
+        return za
     }), e.d(t, "AntdSider", function() {
-        return Ta
+        return Ra
     }), e.d(t, "AntdSpace", function() {
-        return Ia
+        return Ba
     }), e.d(t, "AntdModal", function() {
-        return pr
+        return mr
     }), e.d(t, "AntdAlert", function() {
-        return Gr
+        return $r
     }), e.d(t, "AntdNotification", function() {
-        return Xr
+        return Jr
     }), e.d(t, "AntdMessage", function() {
-        return $r
+        return Qr
     }), e.d(t, "AntdTag", function() {
-        return Jr
+        return eo
     }), e.d(t, "AntdResult", function() {
-        return io
+        return so
     }), e.d(t, "AntdInput", function() {
-        return uo
+        return ho
     }), e.d(t, "AntdTooltip", function() {
-        return po
+        return mo
     }), e.d(t, "AntdCheckbox", function() {
-        return fo
+        return go
     }), e.d(t, "AntdCheckboxGroup", function() {
-        return ho
+        return bo
     }), e.d(t, "AntdSpin", function() {
-        return Oo
+        return jo
     }), e.d(t, "AntdSwitch", function() {
-        return ko
+        return Eo
     }), e.d(t, "AntdParagraph", function() {
-        return Mo
+        return So
     }), e.d(t, "AntdText", function() {
-        return Co
+        return Po
     }), e.d(t, "AntdTitle", function() {
-        return Lo
+        return To
     }), e.d(t, "AntdTabPane", function() {
-        return Po
+        return zo
     }), e.d(t, "AntdTabs", function() {
-        return Vo
+        return Go
     }), e.d(t, "AntdPagination", function() {
-        return Ko
+        return qo
     }), e.d(t, "AntdTreeSelect", function() {
-        return wi
+        return Mi
     }), e.d(t, "AntdDrawer", function() {
-        return Bi
+        return Wi
     }), e.d(t, "AntdPopover", function() {
-        return Fi
-    }), e.d(t, "AntdEmpty", function() {
         return Vi
+    }), e.d(t, "AntdEmpty", function() {
+        return Gi
     }), e.d(t, "AntdCascader", function() {
-        return xl
+        return wl
     }), e.d(t, "AntdRadioGroup", function() {
-        return Ol
+        return jl
     }), e.d(t, "AntdUpload", function() {
-        return Wf
+        return Xf
     }), e.d(t, "AntdIcon", function() {
         return I.a
     }), e.d(t, "AntdPopconfirm", function() {
-        return kl
+        return El
     }), e.d(t, "AntdBackTop", function() {
-        return Cl
+        return Pl
     }), e.d(t, "AntdSkeleton", function() {
-        return Nl
+        return Fl
     }), e.d(t, "AntdAffix", function() {
-        return Yl
+        return Hl
     }), e.d(t, "AntdBreadcrumb", function() {
-        return Zl
+        return $l
     }), e.d(t, "AntdDropdown", function() {
-        return Jl
+        return rc
     }), e.d(t, "AntdInputNumber", function() {
-        return tc
+        return ic
     }), e.d(t, "AntdRate", function() {
-        return fc
+        return yc
     }), e.d(t, "AntdStatistic", function() {
-        return Tc
+        return Yc
     }), e.d(t, "AntdCountdown", function() {
-        return Ac
+        return Fc
     }), e.d(t, "AntdTimeline", function() {
-        return Nc
+        return Vc
     }), e.d(t, "AntdProgress", function() {
-        return Yc
+        return Kc
     }), e.d(t, "AntdAvatar", function() {
-        return Fc
+        return Gc
     }), e.d(t, "AntdAvatarGroup", function() {
-        return Hc
+        return qc
     }), e.d(t, "AntdBadge", function() {
-        return Vc
+        return $c
     }), e.d(t, "AntdRibbon", function() {
-        return Kc
+        return Zc
     }), e.d(t, "AntdTimePicker", function() {
-        return Xc
+        return es
     }), e.d(t, "AntdTimeRangePicker", function() {
-        return Zc
+        return as
     }), e.d(t, "AntdCarousel", function() {
-        return tu
+        return iu
     }), e.d(t, "AntdDraggerUpload", function() {
-        return Df
+        return Nf
     }), e.d(t, "AntdFormItem", function() {
-        return nu
+        return cu
     }), e.d(t, "AntdForm", function() {
-        return au
+        return su
     }), e.d(t, "AntdCardGrid", function() {
-        return ou
+        return du
     }), e.d(t, "AntdCard", function() {
-        return uu
+        return gu
     }), e.d(t, "AntdMentions", function() {
-        return du.a
+        return bu.a
     }), e.d(t, "AntdImage", function() {
-        return bu
-    }), e.d(t, "AntdPageHeader", function() {
         return wu
+    }), e.d(t, "AntdPageHeader", function() {
+        return Su
     }), e.d(t, "AntdCalendar", function() {
-        return Fu
+        return Gu
     }), e.d(t, "AntdComment", function() {
-        return Xu
+        return ed
     }), e.d(t, "AntdDescriptions", function() {
-        return hd
+        return xd
     }), e.d(t, "AntdDescriptionItem", function() {
-        return md
+        return _d
     }), e.d(t, "AntdWatermark", function() {
-        return gd
+        return Od
     }), e.d(t, "AntdSegmented", function() {
-        return zd
+        return Bd
     }), e.d(t, "AntdCheckCard", function() {
-        return Yd
+        return Kd
     }), e.d(t, "AntdCheckCardGroup", function() {
-        return Bd
+        return Ud
     }), e.d(t, "AntdAccordion", function() {
-        return Hd
+        return qd
     }), e.d(t, "AntdPictureUpload", function() {
-        return _f
+        return Ef
     }), e.d(t, "AntdCustomSkeleton", function() {
-        return $f
+        return nh
     }), e.d(t, "AntdSkeletonAvatar", function() {
-        return Zf
+        return ah
     }), e.d(t, "AntdSkeletonButton", function() {
-        return Jf
+        return rh
     }), e.d(t, "AntdSkeletonInput", function() {
-        return Qf
+        return oh
     }), e.d(t, "AntdSkeletonImage", function() {
-        return th
+        return ih
     }), e.d(t, "AntdSegmentedColoring", function() {
-        return uh
+        return gh
     }), e.d(t, "AntdCopyText", function() {
-        return ph
+        return vh
     }), e.d(t, "AntdPopupCard", function() {
-        return xh
+        return Mh
     }), e.d(t, "AntdConfigProvider", function() {
-        return _h
+        return Eh
     }), e.d(t, "AntdSpoiler", function() {
-        return Ah
+        return Fh
     })
 }, function(t, e, n) {
     "use strict";
     var u = n(0),
         d = n.n(u),
         p = n(119),
         f = n(120),
@@ -125836,15 +125984,15 @@
         wt = e(43),
         kt = e(41),
         Rt = e(30),
         jt = e(35),
         Mt = e(37),
         Et = e(69),
         It = e(63),
-        Ct = e(156),
+        Ct = e(157),
         St = e(235),
         Lt = e(78),
         d = {
             icon: {
                 tag: "svg",
                 attrs: {
                     viewBox: "64 64 896 896",
@@ -126298,15 +126446,15 @@
             return mt.createElement(c, Object(ft.a)({
                 ref: e
             }, t, {
                 ellipsis: a,
                 component: "span"
             }))
         }),
-        e = e(57),
+        e = e(58),
         h = Object(e.b)(1, 2, 3, 4, 5),
         e = mt.forwardRef(function(t, e) {
             var n = t.level,
                 n = void 0 === n ? 1 : n,
                 t = function(t, e) {
                     var n = {};
                     for (r in t) Object.prototype.hasOwnProperty.call(t, r) && e.indexOf(r) < 0 && (n[r] = t[r]);
@@ -127447,17 +127595,17 @@
         w = n(5),
         k = n(13),
         j = n(8),
         a = n(7),
         M = n.n(a),
         E = n(0),
         C = n(69),
-        S = n(255),
+        S = n(254),
         L = n(84),
-        a = n(57),
+        a = n(58),
         P = n(256);
 
     function D(n, a) {
         var t = E.useState("string" == typeof n ? n : ""),
             t = Object(j.a)(t, 2),
             e = t[0],
             r = t[1];
```

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/metadata.json` & `feffery_antd_components-0.2.6/feffery_antd_components/metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999894667461885%*

 * *Differences: {"'src/lib/components/AntdDropdown.react.js'": "{'props': {'freePosition': OrderedDict([('type', "*

 * *                                               "OrderedDict([('name', 'bool')])), ('required', "*

 * *                                               "False), ('description', ''), ('defaultValue', "*

 * *                                               "OrderedDict([('value', 'false'), ('computed', "*

 * *                                               "False)]))]), 'freePositionStyle': "*

 * *                                         […]*

```diff
@@ -5591,14 +5591,39 @@
                 },
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
+            "freePosition": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "false"
+                },
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "bool"
+                }
+            },
+            "freePositionClassName": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            },
+            "freePositionStyle": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "object"
+                }
+            },
             "id": {
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
@@ -14087,14 +14112,20 @@
                     "name": "arrayOf",
                     "value": {
                         "name": "objectOf",
                         "value": {
                             "name": "union",
                             "value": [
                                 {
+                                    "name": "arrayOf",
+                                    "value": {
+                                        "name": "any"
+                                    }
+                                },
+                                {
                                     "name": "string"
                                 },
                                 {
                                     "name": "number"
                                 },
                                 {
                                     "name": "exact",
@@ -14715,16 +14746,24 @@
                                                 "name": "exact",
                                                 "value": {
                                                     "label": {
                                                         "name": "string",
                                                         "required": false
                                                     },
                                                     "value": {
-                                                        "name": "string",
-                                                        "required": false
+                                                        "name": "union",
+                                                        "required": false,
+                                                        "value": [
+                                                            {
+                                                                "name": "string"
+                                                            },
+                                                            {
+                                                                "name": "number"
+                                                            }
+                                                        ]
                                                     }
                                                 }
                                             }
                                         },
                                         "placeholder": {
                                             "name": "string",
                                             "required": false
@@ -17476,14 +17515,31 @@
                         },
                         {
                             "name": "number"
                         }
                     ]
                 }
             },
+            "clickedContextMenu": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "exact",
+                    "value": {
+                        "menuKey": {
+                            "name": "string",
+                            "required": false
+                        },
+                        "nodeKey": {
+                            "name": "string",
+                            "required": false
+                        }
+                    }
+                }
+            },
             "defaultCheckedKeys": {
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "arrayOf",
                     "value": {
                         "name": "string"
@@ -23166,14 +23222,18 @@
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "arrayOf",
                     "value": {
                         "name": "exact",
                         "value": {
+                            "fileSize": {
+                                "name": "number",
+                                "required": false
+                            },
                             "name": {
                                 "name": "string",
                                 "required": false
                             },
                             "status": {
                                 "name": "enum",
                                 "required": false,
@@ -23719,14 +23779,18 @@
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "arrayOf",
                     "value": {
                         "name": "exact",
                         "value": {
+                            "fileSize": {
+                                "name": "number",
+                                "required": false
+                            },
                             "name": {
                                 "name": "string",
                                 "required": false
                             },
                             "status": {
                                 "name": "enum",
                                 "required": false,
@@ -24269,14 +24333,18 @@
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "arrayOf",
                     "value": {
                         "name": "exact",
                         "value": {
+                            "fileSize": {
+                                "name": "number",
+                                "required": false
+                            },
                             "name": {
                                 "name": "string",
                                 "required": false
                             },
                             "status": {
                                 "name": "enum",
                                 "required": false,
```

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components/package-info.json` & `feffery_antd_components-0.2.6/feffery_antd_components/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'0.2.6'"}*

```diff
@@ -84,9 +84,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_antd_components -p package-info.json --r-prefix 'feffery' --jl-prefix 'feffery'",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.2.5"
+    "version": "0.2.6"
 }
```

### Comparing `feffery_antd_components-0.2.5/feffery_antd_components.egg-info/SOURCES.txt` & `feffery_antd_components-0.2.6/feffery_antd_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.5/package.json` & `feffery_antd_components-0.2.6/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'0.2.6'"}*

```diff
@@ -84,9 +84,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_antd_components -p package-info.json --r-prefix 'feffery' --jl-prefix 'feffery'",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.2.5"
+    "version": "0.2.6"
 }
```

### Comparing `feffery_antd_components-0.2.5/setup.py` & `feffery_antd_components-0.2.6/setup.py`

 * *Files identical despite different names*

