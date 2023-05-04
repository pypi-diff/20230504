# Comparing `tmp/NodeGraphQt-0.5.7.tar.gz` & `tmp/NodeGraphQt-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NodeGraphQt-0.5.7.tar", last modified: Sun Apr 23 10:29:34 2023, max compression
+gzip compressed data, was "NodeGraphQt-0.5.8.tar", last modified: Thu May  4 10:20:26 2023, max compression
```

## Comparing `NodeGraphQt-0.5.7.tar` & `NodeGraphQt-0.5.8.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 10:29:34.923777 NodeGraphQt-0.5.7/
--rw-rw-rw-   0        0        0     1102 2021-06-18 10:54:50.000000 NodeGraphQt-0.5.7/LICENSE.md
--rw-rw-rw-   0        0        0       49 2022-05-22 21:37:50.000000 NodeGraphQt-0.5.7/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-04-23 10:29:34.853762 NodeGraphQt-0.5.7/NodeGraphQt/
--rw-rw-rw-   0        0        0     2469 2023-02-12 22:21:30.000000 NodeGraphQt-0.5.7/NodeGraphQt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:29:34.876766 NodeGraphQt-0.5.7/NodeGraphQt/base/
--rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.7/NodeGraphQt/base/__init__.py
--rw-rw-rw-   0        0        0    12642 2023-04-03 22:08:42.000000 NodeGraphQt-0.5.7/NodeGraphQt/base/commands.py
--rw-rw-rw-   0        0        0     2816 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.7/NodeGraphQt/base/factory.py
--rw-rw-rw-   0        0        0    96067 2023-04-18 09:06:39.000000 NodeGraphQt-0.5.7/NodeGraphQt/base/graph.py
--rw-rw-rw-   0        0        0     8273 2023-04-18 09:06:39.000000 NodeGraphQt-0.5.7/NodeGraphQt/base/menu.py
--rw-rw-rw-   0        0        0    14329 2023-02-15 08:13:57.000000 NodeGraphQt-0.5.7/NodeGraphQt/base/model.py
--rw-rw-rw-   0        0        0    15016 2023-04-18 09:06:39.000000 NodeGraphQt-0.5.7/NodeGraphQt/base/node.py
--rw-rw-rw-   0        0        0    12137 2023-04-18 09:06:39.000000 NodeGraphQt-0.5.7/NodeGraphQt/base/port.py
--rw-rw-rw-   0        0        0     7417 2023-04-18 09:06:39.000000 NodeGraphQt-0.5.7/NodeGraphQt/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:29:34.879768 NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/
--rw-rw-rw-   0        0        0        0 2022-05-08 02:47:52.000000 NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/__init__.py
--rw-rw-rw-   0        0        0    11914 2023-04-18 09:06:39.000000 NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/nodes_palette.py
--rw-rw-rw-   0        0        0     4749 2023-04-18 09:06:39.000000 NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/nodes_tree.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:29:34.888769 NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/properties_bin/
--rw-rw-rw-   0        0        0        0 2022-12-21 22:27:30.000000 NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/properties_bin/__init__.py
--rw-rw-rw-   0        0        0     3550 2023-01-27 07:27:32.000000 NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
--rw-rw-rw-   0        0        0     2455 2023-03-15 09:23:02.000000 NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
--rw-rw-rw-   0        0        0     4995 2023-04-03 22:08:42.000000 NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
--rw-rw-rw-   0        0        0     6304 2022-12-21 22:27:30.000000 NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
--rw-rw-rw-   0        0        0     2948 2023-03-15 09:23:02.000000 NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
--rw-rw-rw-   0        0        0     2489 2023-03-15 09:23:02.000000 NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py
--rw-rw-rw-   0        0        0    20765 2023-04-18 09:06:39.000000 NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py
--rw-rw-rw-   0        0        0      761 2022-12-21 22:27:30.000000 NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
--rw-rw-rw-   0        0        0     7267 2022-12-21 22:27:30.000000 NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
--rw-rw-rw-   0        0        0      406 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.7/NodeGraphQt/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:29:34.895771 NodeGraphQt-0.5.7/NodeGraphQt/nodes/
--rw-rw-rw-   0        0        0        0 2022-05-08 02:47:52.000000 NodeGraphQt-0.5.7/NodeGraphQt/nodes/__init__.py
--rw-rw-rw-   0        0        0     4465 2023-04-18 09:06:39.000000 NodeGraphQt-0.5.7/NodeGraphQt/nodes/backdrop_node.py
--rw-rw-rw-   0        0        0    23281 2023-04-18 09:06:39.000000 NodeGraphQt-0.5.7/NodeGraphQt/nodes/base_node.py
--rw-rw-rw-   0        0        0     1253 2023-04-18 09:06:39.000000 NodeGraphQt-0.5.7/NodeGraphQt/nodes/base_node_circle.py
--rw-rw-rw-   0        0        0     5144 2023-04-18 09:06:39.000000 NodeGraphQt-0.5.7/NodeGraphQt/nodes/group_node.py
--rw-rw-rw-   0        0        0     4409 2023-04-18 09:06:39.000000 NodeGraphQt-0.5.7/NodeGraphQt/nodes/port_node.py
--rw-rw-rw-   0        0        0      239 2023-04-23 10:23:31.000000 NodeGraphQt-0.5.7/NodeGraphQt/pkg_info.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:29:34.907774 NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/
--rw-rw-rw-   0        0        0        0 2021-06-18 10:54:50.000000 NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/__init__.py
--rw-rw-rw-   0        0        0     7060 2023-04-19 08:52:02.000000 NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/node_abstract.py
--rw-rw-rw-   0        0        0    10763 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/node_backdrop.py
--rw-rw-rw-   0        0        0    36771 2023-04-21 11:39:42.000000 NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/node_base.py
--rw-rw-rw-   0        0        0    21204 2023-04-23 01:40:25.000000 NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/node_circle.py
--rw-rw-rw-   0        0        0    12346 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/node_group.py
--rw-rw-rw-   0        0        0     4273 2022-05-08 02:47:52.000000 NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/node_overlay_disabled.py
--rw-rw-rw-   0        0        0     8159 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/node_port_in.py
--rw-rw-rw-   0        0        0     8158 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/node_port_out.py
--rw-rw-rw-   0        0        0     3749 2022-05-08 02:47:52.000000 NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/node_text_item.py
--rw-rw-rw-   0        0        0    17657 2023-04-03 22:08:42.000000 NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/pipe.py
--rw-rw-rw-   0        0        0    10582 2023-04-22 02:08:59.000000 NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/port.py
--rw-rw-rw-   0        0        0     2885 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/slicer.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:29:34.915776 NodeGraphQt-0.5.7/NodeGraphQt/widgets/
--rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.7/NodeGraphQt/widgets/__init__.py
--rw-rw-rw-   0        0        0     3709 2022-12-21 07:01:38.000000 NodeGraphQt-0.5.7/NodeGraphQt/widgets/actions.py
--rw-rw-rw-   0        0        0     1873 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.7/NodeGraphQt/widgets/dialogs.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:29:34.916776 NodeGraphQt-0.5.7/NodeGraphQt/widgets/icons/
--rw-rw-rw-   0        0        0    17542 2021-06-18 10:54:50.000000 NodeGraphQt-0.5.7/NodeGraphQt/widgets/icons/node_base.png
--rw-rw-rw-   0        0        0     4531 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.7/NodeGraphQt/widgets/node_graph.py
--rw-rw-rw-   0        0        0    14045 2023-04-18 09:06:39.000000 NodeGraphQt-0.5.7/NodeGraphQt/widgets/node_widgets.py
--rw-rw-rw-   0        0        0     5681 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.7/NodeGraphQt/widgets/scene.py
--rw-rw-rw-   0        0        0    11436 2023-04-03 22:08:42.000000 NodeGraphQt-0.5.7/NodeGraphQt/widgets/tab_search.py
--rw-rw-rw-   0        0        0    47453 2023-04-23 01:40:25.000000 NodeGraphQt-0.5.7/NodeGraphQt/widgets/viewer.py
--rw-rw-rw-   0        0        0     6506 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.7/NodeGraphQt/widgets/viewer_nav.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:29:34.869766 NodeGraphQt-0.5.7/NodeGraphQt.egg-info/
--rw-rw-rw-   0        0        0     2303 2023-04-23 10:29:34.000000 NodeGraphQt-0.5.7/NodeGraphQt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2543 2023-04-23 10:29:34.000000 NodeGraphQt-0.5.7/NodeGraphQt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 10:29:34.000000 NodeGraphQt-0.5.7/NodeGraphQt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-04-23 10:29:34.000000 NodeGraphQt-0.5.7/NodeGraphQt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-23 10:29:34.000000 NodeGraphQt-0.5.7/NodeGraphQt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2303 2023-04-23 10:29:34.924777 NodeGraphQt-0.5.7/PKG-INFO
--rw-rw-rw-   0        0        0     1599 2023-04-23 10:23:31.000000 NodeGraphQt-0.5.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 10:29:34.846760 NodeGraphQt-0.5.7/examples/
-drwxrwxrwx   0        0        0        0 2023-04-23 10:29:34.918776 NodeGraphQt-0.5.7/examples/hotkeys/
--rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.7/examples/hotkeys/__init__.py
--rw-rw-rw-   0        0        0     5721 2023-04-23 01:34:58.000000 NodeGraphQt-0.5.7/examples/hotkeys/hotkey_functions.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:29:34.923777 NodeGraphQt-0.5.7/examples/nodes/
--rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.7/examples/nodes/__init__.py
--rw-rw-rw-   0        0        0     2157 2023-04-23 01:40:25.000000 NodeGraphQt-0.5.7/examples/nodes/basic_nodes.py
--rw-rw-rw-   0        0        0     3671 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.7/examples/nodes/custom_ports_node.py
--rw-rw-rw-   0        0        0      507 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.7/examples/nodes/group_node.py
--rw-rw-rw-   0        0        0     1822 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.7/examples/nodes/widget_nodes.py
--rw-rw-rw-   0        0        0     1070 2023-04-23 10:29:34.926777 NodeGraphQt-0.5.7/setup.cfg
--rw-rw-rw-   0        0        0      123 2022-12-21 06:31:06.000000 NodeGraphQt-0.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.471355 NodeGraphQt-0.5.8/
+-rw-rw-rw-   0        0        0     1102 2021-06-18 10:54:50.000000 NodeGraphQt-0.5.8/LICENSE.md
+-rw-rw-rw-   0        0        0       49 2022-05-22 21:37:50.000000 NodeGraphQt-0.5.8/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.214610 NodeGraphQt-0.5.8/NodeGraphQt/
+-rw-rw-rw-   0        0        0     2469 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.264239 NodeGraphQt-0.5.8/NodeGraphQt/base/
+-rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/NodeGraphQt/base/__init__.py
+-rw-rw-rw-   0        0        0    12642 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/base/commands.py
+-rw-rw-rw-   0        0        0     2816 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/NodeGraphQt/base/factory.py
+-rw-rw-rw-   0        0        0    97821 2023-05-04 10:16:17.000000 NodeGraphQt-0.5.8/NodeGraphQt/base/graph.py
+-rw-rw-rw-   0        0        0     8273 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/base/menu.py
+-rw-rw-rw-   0        0        0    14329 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/base/model.py
+-rw-rw-rw-   0        0        0    15016 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/base/node.py
+-rw-rw-rw-   0        0        0    12137 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/base/port.py
+-rw-rw-rw-   0        0        0     7417 2023-05-03 04:38:45.000000 NodeGraphQt-0.5.8/NodeGraphQt/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.276242 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/
+-rw-rw-rw-   0        0        0        0 2022-05-08 02:47:52.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/__init__.py
+-rw-rw-rw-   0        0        0    11914 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/nodes_palette.py
+-rw-rw-rw-   0        0        0     4749 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/nodes_tree.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.326253 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/
+-rw-rw-rw-   0        0        0        0 2022-12-21 22:27:30.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/__init__.py
+-rw-rw-rw-   0        0        0     3550 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
+-rw-rw-rw-   0        0        0     2455 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
+-rw-rw-rw-   0        0        0     4995 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
+-rw-rw-rw-   0        0        0     6304 2022-12-21 22:27:30.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
+-rw-rw-rw-   0        0        0     2948 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
+-rw-rw-rw-   0        0        0     2489 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py
+-rw-rw-rw-   0        0        0    20765 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py
+-rw-rw-rw-   0        0        0      761 2022-12-21 22:27:30.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
+-rw-rw-rw-   0        0        0     7267 2022-12-21 22:27:30.000000 NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
+-rw-rw-rw-   0        0        0      406 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/NodeGraphQt/errors.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.346258 NodeGraphQt-0.5.8/NodeGraphQt/nodes/
+-rw-rw-rw-   0        0        0        0 2022-05-08 02:47:52.000000 NodeGraphQt-0.5.8/NodeGraphQt/nodes/__init__.py
+-rw-rw-rw-   0        0        0     4465 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/nodes/backdrop_node.py
+-rw-rw-rw-   0        0        0    23281 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/nodes/base_node.py
+-rw-rw-rw-   0        0        0     1253 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/nodes/base_node_circle.py
+-rw-rw-rw-   0        0        0     5817 2023-05-04 10:15:30.000000 NodeGraphQt-0.5.8/NodeGraphQt/nodes/group_node.py
+-rw-rw-rw-   0        0        0     4409 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/nodes/port_node.py
+-rw-rw-rw-   0        0        0      239 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/pkg_info.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.410273 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/
+-rw-rw-rw-   0        0        0        0 2021-06-18 10:54:50.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/__init__.py
+-rw-rw-rw-   0        0        0     7060 2023-04-19 08:52:02.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_abstract.py
+-rw-rw-rw-   0        0        0    10763 2023-05-03 01:54:07.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_backdrop.py
+-rw-rw-rw-   0        0        0    36771 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_base.py
+-rw-rw-rw-   0        0        0    21204 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_circle.py
+-rw-rw-rw-   0        0        0    12346 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_group.py
+-rw-rw-rw-   0        0        0     4273 2022-05-08 02:47:52.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_overlay_disabled.py
+-rw-rw-rw-   0        0        0     8159 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_port_in.py
+-rw-rw-rw-   0        0        0     8158 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_port_out.py
+-rw-rw-rw-   0        0        0     3749 2022-05-08 02:47:52.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_text_item.py
+-rw-rw-rw-   0        0        0    21504 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/pipe.py
+-rw-rw-rw-   0        0        0    10582 2023-04-30 08:29:15.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/port.py
+-rw-rw-rw-   0        0        0     2885 2023-05-03 09:02:56.000000 NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/slicer.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.447351 NodeGraphQt-0.5.8/NodeGraphQt/widgets/
+-rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/NodeGraphQt/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3709 2022-12-21 07:01:38.000000 NodeGraphQt-0.5.8/NodeGraphQt/widgets/actions.py
+-rw-rw-rw-   0        0        0     1873 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/NodeGraphQt/widgets/dialogs.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.448351 NodeGraphQt-0.5.8/NodeGraphQt/widgets/icons/
+-rw-rw-rw-   0        0        0    17542 2021-06-18 10:54:50.000000 NodeGraphQt-0.5.8/NodeGraphQt/widgets/icons/node_base.png
+-rw-rw-rw-   0        0        0     4550 2023-05-03 09:15:23.000000 NodeGraphQt-0.5.8/NodeGraphQt/widgets/node_graph.py
+-rw-rw-rw-   0        0        0    14045 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/widgets/node_widgets.py
+-rw-rw-rw-   0        0        0     5681 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/NodeGraphQt/widgets/scene.py
+-rw-rw-rw-   0        0        0    11436 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/NodeGraphQt/widgets/tab_search.py
+-rw-rw-rw-   0        0        0    51080 2023-05-03 09:00:22.000000 NodeGraphQt-0.5.8/NodeGraphQt/widgets/viewer.py
+-rw-rw-rw-   0        0        0     6914 2023-05-04 05:49:13.000000 NodeGraphQt-0.5.8/NodeGraphQt/widgets/viewer_nav.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.232613 NodeGraphQt-0.5.8/NodeGraphQt.egg-info/
+-rw-rw-rw-   0        0        0     2738 2023-05-04 10:20:26.000000 NodeGraphQt-0.5.8/NodeGraphQt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2543 2023-05-04 10:20:26.000000 NodeGraphQt-0.5.8/NodeGraphQt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 10:20:26.000000 NodeGraphQt-0.5.8/NodeGraphQt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-04 10:20:26.000000 NodeGraphQt-0.5.8/NodeGraphQt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-04 10:20:26.000000 NodeGraphQt-0.5.8/NodeGraphQt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2738 2023-05-04 10:20:26.471355 NodeGraphQt-0.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2034 2023-05-03 10:36:51.000000 NodeGraphQt-0.5.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.192605 NodeGraphQt-0.5.8/examples/
+drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.450350 NodeGraphQt-0.5.8/examples/hotkeys/
+-rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/examples/hotkeys/__init__.py
+-rw-rw-rw-   0        0        0     6199 2023-05-04 10:16:17.000000 NodeGraphQt-0.5.8/examples/hotkeys/hotkey_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:20:26.470355 NodeGraphQt-0.5.8/examples/nodes/
+-rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/examples/nodes/__init__.py
+-rw-rw-rw-   0        0        0     2157 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.8/examples/nodes/basic_nodes.py
+-rw-rw-rw-   0        0        0     3671 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/examples/nodes/custom_ports_node.py
+-rw-rw-rw-   0        0        0      507 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.8/examples/nodes/group_node.py
+-rw-rw-rw-   0        0        0     1822 2023-05-02 10:58:55.000000 NodeGraphQt-0.5.8/examples/nodes/widget_nodes.py
+-rw-rw-rw-   0        0        0     1070 2023-05-04 10:20:26.476357 NodeGraphQt-0.5.8/setup.cfg
+-rw-rw-rw-   0        0        0      123 2022-12-21 06:31:06.000000 NodeGraphQt-0.5.8/setup.py
```

### Comparing `NodeGraphQt-0.5.7/LICENSE.md` & `NodeGraphQt-0.5.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/__init__.py` & `NodeGraphQt-0.5.8/NodeGraphQt/__init__.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/base/commands.py` & `NodeGraphQt-0.5.8/NodeGraphQt/base/commands.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/base/factory.py` & `NodeGraphQt-0.5.8/NodeGraphQt/base/factory.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/base/graph.py` & `NodeGraphQt-0.5.8/NodeGraphQt/base/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1319,15 +1319,17 @@
         if not nodes:
             return
         if len(nodes) == 1:
             self.delete_node(nodes[0], push_undo=push_undo)
             return
         node_ids = [n.id for n in nodes]
         if push_undo:
-            self._undo_stack.beginMacro('deleted "{}" nodes'.format(len(nodes)))
+            self._undo_stack.beginMacro(
+                'deleted "{}" node(s)'.format(len(nodes))
+            )
         for node in nodes:
 
             # collapse group node before removing.
             if isinstance(node, GroupNode) and node.is_expanded:
                 node.collapse()
 
             if isinstance(node, BaseNode):
@@ -1347,14 +1349,62 @@
                 self._undo_stack.push(NodeRemovedCmd(self, node))
             else:
                 NodeRemovedCmd(self, node).redo()
         if push_undo:
             self._undo_stack.endMacro()
         self.nodes_deleted.emit(node_ids)
 
+    def extract_nodes(self, nodes, push_undo=True, prompt_warning=True):
+        """
+        Extract select nodes from it connections.
+
+        Args:
+            nodes (list[NodeGraphQt.BaseNode]): list of node instances.
+            push_undo (bool): register the command to the undo stack. (default: True)
+            prompt_warning (bool): prompt warning dialog box.
+        """
+        if not nodes:
+            return
+
+        locked_ports = []
+        base_nodes = []
+        for node in nodes:
+            if not isinstance(node, BaseNode):
+                continue
+
+            for port in node.input_ports() + node.output_ports():
+                if port.locked():
+                    locked_ports.append('{0.node.name}: {0.name}'.format(port))
+
+            base_nodes.append(node)
+
+        if locked_ports:
+            message = (
+                'Selected nodes cannot be extracted because the following '
+                'ports are locked:\n{}'.format('\n'.join(sorted(locked_ports)))
+            )
+            if prompt_warning:
+                self._viewer.message_dialog(message, 'Can\'t Extract Nodes')
+            return
+
+        if push_undo:
+            self._undo_stack.beginMacro(
+                'extracted "{}" node(s)'.format(len(nodes))
+            )
+
+        for node in base_nodes:
+            for port in node.input_ports() + node.output_ports():
+                for connected_port in port.connected_ports():
+                    if connected_port.node() in base_nodes:
+                        continue
+                    port.disconnect_from(connected_port, push_undo=push_undo)
+
+        if push_undo:
+            self._undo_stack.endMacro()
+
     def all_nodes(self):
         """
         Return all nodes in the node graph.
 
         Returns:
             list[NodeGraphQt.BaseNode]: list of nodes.
         """
```

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/base/menu.py` & `NodeGraphQt-0.5.8/NodeGraphQt/base/menu.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/base/model.py` & `NodeGraphQt-0.5.8/NodeGraphQt/base/model.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/base/node.py` & `NodeGraphQt-0.5.8/NodeGraphQt/base/node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/base/port.py` & `NodeGraphQt-0.5.8/NodeGraphQt/base/port.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/constants.py` & `NodeGraphQt-0.5.8/NodeGraphQt/constants.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/nodes_palette.py` & `NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/nodes_palette.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/nodes_tree.py` & `NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/nodes_tree.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py` & `NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py` & `NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py` & `NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py` & `NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py` & `NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py` & `NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py` & `NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py` & `NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py` & `NodeGraphQt-0.5.8/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/nodes/backdrop_node.py` & `NodeGraphQt-0.5.8/NodeGraphQt/nodes/backdrop_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/nodes/base_node.py` & `NodeGraphQt-0.5.8/NodeGraphQt/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/nodes/base_node_circle.py` & `NodeGraphQt-0.5.8/NodeGraphQt/nodes/base_node_circle.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/nodes/group_node.py` & `NodeGraphQt-0.5.8/NodeGraphQt/nodes/group_node.py`

 * *Files 18% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     def get_sub_graph(self):
         """
         Returns the sub graph controller to the group node if initialized
         or returns None.
 
         Returns:
-            SubGraph or None: sub graph controller.
+            SubGraph: sub graph controller.
         """
         return self.graph.sub_graphs.get(self.id)
 
     def get_sub_graph_session(self):
         """
         Returns the serialized sub graph session.
 
@@ -87,14 +87,30 @@
 
         See Also:
             :meth:`NodeGraph.collapse_group_node`,
             :meth:`SubGraph.collapse_group_node`.
         """
         self.graph.collapse_group_node(self)
 
+    def set_name(self, name=''):
+        super(GroupNode, self).set_name(name)
+        # update the tab bar and navigation labels.
+        sub_graph = self.get_sub_graph()
+        if sub_graph:
+            nav_widget = sub_graph.navigation_widget
+            nav_widget.update_label_item(self.name(), self.id)
+
+            if sub_graph.parent_graph.is_root:
+                root_graph = sub_graph.parent_graph
+                tab_bar = root_graph.widget.tabBar()
+                for idx in range(tab_bar.count()):
+                    if tab_bar.tabToolTip(idx) == self.id:
+                        tab_bar.setTabText(idx, self.name())
+                        break
+
     def add_input(self, name='input', multi_input=False, display_name=True,
                   color=None, locked=False, painter_func=None):
         port = super(GroupNode, self).add_input(
             name=name,
             multi_input=multi_input,
             display_name=display_name,
             color=color,
```

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/nodes/port_node.py` & `NodeGraphQt-0.5.8/NodeGraphQt/nodes/port_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/node_abstract.py` & `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_abstract.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/node_backdrop.py` & `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_backdrop.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/node_base.py` & `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_base.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/node_circle.py` & `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_circle.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/node_group.py` & `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_group.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/node_overlay_disabled.py` & `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_overlay_disabled.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/node_port_in.py` & `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_port_in.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/node_port_out.py` & `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_port_out.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/node_text_item.py` & `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/node_text_item.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/pipe.py` & `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/pipe.py`

 * *Files 11% similar despite different names*

```diff
@@ -412,20 +412,41 @@
         if self.output_port and self.output_port.connected_pipes:
             self.output_port.remove_pipe(self)
         if self.scene():
             self.scene().removeItem(self)
 
 
 class LivePipeItem(PipeItem):
+    """
+    Live Pipe item used for drawing the live connection with the cursor.
+    """
 
     def __init__(self):
         super(LivePipeItem, self).__init__()
         self.setZValue(Z_VAL_NODE_WIDGET + 1)
         self.shift_selected = False
 
+        color = QtGui.QColor(*PipeEnum.ACTIVE_COLOR.value)
+        pen = QtGui.QPen(color, PipeEnum.WIDTH.value + 0.35)
+        pen.setJoinStyle(QtCore.Qt.MiterJoin)
+        pen.setCapStyle(QtCore.Qt.RoundCap)
+
+        self._idx_pointer = LivePipePolygonItem(self)
+        self._idx_pointer.setPolygon(self._arrow)
+        self._idx_pointer.setBrush(color.darker(300))
+        self._idx_pointer.setPen(pen)
+
+        color = QtGui.QColor(*PipeEnum.ACTIVE_COLOR.value)
+        color.setAlpha(50)
+        self._idx_text = QtWidgets.QGraphicsTextItem(self)
+        self._idx_text.setDefaultTextColor(color)
+        font = self._idx_text.font()
+        font.setPointSize(7)
+        self._idx_text.setFont(font)
+
     def paint(self, painter, option, widget):
         """
         Draws the connection line.
 
         Args:
             painter (QtGui.QPainter): painter used for drawing the item.
             option (QtGui.QStyleOptionGraphicsItem):
@@ -445,29 +466,20 @@
         painter.setRenderHint(painter.Antialiasing, True)
         painter.drawPath(self.path())
 
         cen_x = self.path().pointAtPercent(0.5).x()
         cen_y = self.path().pointAtPercent(0.5).y()
         loc_pt = self.path().pointAtPercent(0.9)
         tgt_pt = self.path().pointAtPercent(1.0)
-        start_pt = self.path().pointAtPercent(0.0)
 
         dist = math.hypot(tgt_pt.x() - cen_x, tgt_pt.y() - cen_y)
         if dist < 0.05:
             painter.restore()
             return
 
-        # draw start circle
-        size = 5.0
-        rect = QtCore.QRectF(start_pt.x() - (size / 2),
-                             start_pt.y() - (size / 2),
-                             size, size)
-        painter.setBrush(color)
-        painter.drawEllipse(rect)
-
         # draw middle circle
         size = 10.0
         if dist < 50.0:
             size *= (dist / 50.0)
         rect = QtCore.QRectF(cen_x-(size/2), cen_y-(size/2), size, size)
         painter.setBrush(color)
         painter.setPen(QtGui.QPen(color.darker(130), pen_width))
@@ -486,13 +498,96 @@
         transform.translate(tgt_pt.x(), tgt_pt.y())
 
         radians = math.atan2(tgt_pt.y() - loc_pt.y(),
                              tgt_pt.x() - loc_pt.x())
         degrees = math.degrees(radians) + 90
         transform.rotate(degrees)
 
-        scale = 1.0
-        if dist < 20.0:
-            scale = dist / 20.0
-        transform.scale(scale, scale)
-        painter.drawPolygon(transform.map(self._arrow))
+        painter.restore()
+
+    def draw_path(self, start_port, end_port=None, cursor_pos=None,
+                  color_mode=None):
+        """
+        re-implemented to also update the index pointer arrow position.
+
+        Args:
+            start_port (PortItem): port used to draw the starting point.
+            end_port (PortItem): port used to draw the end point.
+            cursor_pos (QtCore.QPointF): cursor position if specified this
+                will be the draw end point.
+            color_mode (str): arrow index pointer color mode
+                              ('accept', 'reject' or None).
+        """
+        super(LivePipeItem, self).draw_path(start_port, end_port, cursor_pos)
+        self.draw_index_pointer(start_port, cursor_pos, color_mode)
+
+    def draw_index_pointer(self, start_port, cursor_pos, color_mode=None):
+        """
+        Update the index pointer arrow position and direction when the
+        live pipe path is redrawn.
+
+        Args:
+            start_port (PortItem): start port item.
+            cursor_pos (QtCore.QPoint): cursor scene position.
+            color_mode (str): arrow index pointer color mode
+                              ('accept', 'reject' or None).
+        """
+        text_rect = self._idx_text.boundingRect()
+
+        transform = QtGui.QTransform()
+        transform.translate(cursor_pos.x(), cursor_pos.y())
+        if self.viewer_layout_direction() is LayoutDirectionEnum.VERTICAL.value:
+            text_pos = (
+                cursor_pos.x() + (text_rect.width() / 2.5),
+                cursor_pos.y() - (text_rect.height() / 2)
+            )
+            if start_port.port_type == PortTypeEnum.OUT.value:
+                transform.rotate(180)
+        elif self.viewer_layout_direction() is LayoutDirectionEnum.HORIZONTAL.value:
+            text_pos = (
+                cursor_pos.x() - (text_rect.width() / 2),
+                cursor_pos.y() - (text_rect.height() * 1.25)
+            )
+            if start_port.port_type == PortTypeEnum.IN.value:
+                transform.rotate(-90)
+            else:
+                transform.rotate(90)
+        self._idx_text.setPos(*text_pos)
+        self._idx_text.setPlainText('{}'.format(start_port.name))
+
+        self._idx_pointer.setPolygon(transform.map(self._arrow))
+
+        if color_mode == 'accept':
+            color = QtGui.QColor(*PipeEnum.HIGHLIGHT_COLOR.value)
+        elif color_mode == 'reject':
+            color = QtGui.QColor(*PipeEnum.DISABLED_COLOR.value)
+        else:
+            color = QtGui.QColor(*PipeEnum.ACTIVE_COLOR.value)
+
+        pen = self._idx_pointer.pen()
+        pen.setColor(color)
+        self._idx_pointer.setBrush(color.darker(300))
+        self._idx_pointer.setPen(pen)
+
+
+class LivePipePolygonItem(QtWidgets.QGraphicsPolygonItem):
+    """
+    Custom live pipe polygon shape.
+    """
+
+    def __init__(self, parent):
+        super(LivePipePolygonItem, self).__init__(parent)
+        self.setFlag(self.ItemIsSelectable, True)
+
+    def paint(self, painter, option, widget):
+        """
+        Args:
+            painter (QtGui.QPainter): painter used for drawing the item.
+            option (QtGui.QStyleOptionGraphicsItem):
+                used to describe the parameters needed to draw.
+            widget (QtWidgets.QWidget): not used.
+        """
+        painter.save()
+        painter.setBrush(self.brush())
+        painter.setPen(self.pen())
+        painter.drawPolygon(self.polygon())
         painter.restore()
```

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/port.py` & `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/port.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/qgraphics/slicer.py` & `NodeGraphQt-0.5.8/NodeGraphQt/qgraphics/slicer.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/widgets/actions.py` & `NodeGraphQt-0.5.8/NodeGraphQt/widgets/actions.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/widgets/dialogs.py` & `NodeGraphQt-0.5.8/NodeGraphQt/widgets/dialogs.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/widgets/icons/node_base.png` & `NodeGraphQt-0.5.8/NodeGraphQt/widgets/icons/node_base.png`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/widgets/node_graph.py` & `NodeGraphQt-0.5.8/NodeGraphQt/widgets/node_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 class NodeGraphWidget(QtWidgets.QTabWidget):
 
     def __init__(self, parent=None):
         super(NodeGraphWidget, self).__init__(parent)
         self.setTabsClosable(True)
         self.setTabBarAutoHide(True)
-        text_color = self.palette().text().color().getRgb()
         bg_color = QtGui.QColor(
             *ViewerEnum.BACKGROUND_COLOR.value).darker(120).getRgb()
+        text_color = tuple(map(lambda i, j: i - j, (255, 255, 255), bg_color))
         style_dict = {
             'QWidget': {
                 'background-color': 'rgb({0},{1},{2})'.format(
                     *ViewerEnum.BACKGROUND_COLOR.value
                 ),
             },
             'QTabWidget::pane': {
```

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/widgets/node_widgets.py` & `NodeGraphQt-0.5.8/NodeGraphQt/widgets/node_widgets.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/widgets/scene.py` & `NodeGraphQt-0.5.8/NodeGraphQt/widgets/scene.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/widgets/tab_search.py` & `NodeGraphQt-0.5.8/NodeGraphQt/widgets/tab_search.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/widgets/viewer.py` & `NodeGraphQt-0.5.8/NodeGraphQt/widgets/viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 import math
 from distutils.version import LooseVersion
 
 from Qt import QtGui, QtCore, QtWidgets
 
 from NodeGraphQt.base.menu import BaseMenu
 from NodeGraphQt.constants import (
-    LayoutDirectionEnum, PortTypeEnum, PipeLayoutEnum
+    LayoutDirectionEnum,
+    PortTypeEnum,
+    PipeLayoutEnum,
+    ViewerEnum,
+    Z_VAL_NODE_WIDGET
 )
 from NodeGraphQt.qgraphics.node_abstract import AbstractNodeItem
 from NodeGraphQt.qgraphics.node_backdrop import BackdropNodeItem
 from NodeGraphQt.qgraphics.pipe import PipeItem, LivePipeItem
 from NodeGraphQt.qgraphics.port import PortItem
 from NodeGraphQt.qgraphics.slicer import SlicerPipeItem
 from NodeGraphQt.widgets.dialogs import BaseDialog, FileDialog
@@ -85,14 +89,27 @@
         self._prev_selection_pipes = []
         self._node_positions = {}
         self._rubber_band = QtWidgets.QRubberBand(
             QtWidgets.QRubberBand.Rectangle, self
         )
         self._rubber_band.isActive = False
 
+        text_color = QtGui.QColor(*tuple(map(
+            lambda i, j: i - j, (255, 255, 255),
+            ViewerEnum.BACKGROUND_COLOR.value
+        )))
+        text_color.setAlpha(50)
+        self._cusor_text = QtWidgets.QGraphicsTextItem()
+        self._cusor_text.setDefaultTextColor(text_color)
+        self._cusor_text.setZValue(Z_VAL_NODE_WIDGET + 1)
+        font = self._cusor_text.font()
+        font.setPointSize(7)
+        self._cusor_text.setFont(font)
+        self.scene().addItem(self._cusor_text)
+
         self._LIVE_PIPE = LivePipeItem()
         self._LIVE_PIPE.setVisible(False)
         self.scene().addItem(self._LIVE_PIPE)
 
         self._SLICER_PIPE = SlicerPipeItem()
         self._SLICER_PIPE.setVisible(False)
         self.scene().addItem(self._SLICER_PIPE)
@@ -381,33 +398,70 @@
                 return
 
         # pan mode.
         if self.ALT_state:
             return
 
         items = self._items_near(map_pos, None, 20, 20)
-        nodes = [i for i in items if isinstance(i, AbstractNodeItem)]
-        # pipes = [i for i in items if isinstance(i, PipeItem)]
+        pipes = []
+        nodes = []
+        backdrop = None
+        for itm in items:
+            if isinstance(itm, PipeItem):
+                pipes.append(itm)
+            elif isinstance(itm, AbstractNodeItem):
+                if isinstance(itm, BackdropNodeItem):
+                    backdrop = itm
+                    continue
+                nodes.append(itm)
 
         if nodes:
             self.MMB_state = False
 
-        # toggle extend node selection.
+        # record the node selection as "self.selected_nodes()" is not updated
+        # here on the mouse press event.
+        selection = set([])
+
         if self.LMB_state:
+            # toggle extend node selection.
             if self.SHIFT_state:
-                for node in nodes:
-                    node.selected = not node.selected
+                if items and backdrop == items[0]:
+                    backdrop.selected = not backdrop.selected
+                    if backdrop.selected:
+                        selection.add(backdrop)
+                    for n in backdrop.get_nodes():
+                        n.selected = backdrop.selected
+                        if backdrop.selected:
+                            selection.add(n)
+                else:
+                    for node in nodes:
+                        node.selected = not node.selected
+                        if node.selected:
+                            selection.add(node)
+            # unselected nodes with the "ctrl" key.
             elif self.CTRL_state:
+                if items and backdrop == items[0]:
+                    backdrop.selected = False
+                else:
+                    for node in nodes:
+                        node.selected = False
+            # if no modifier keys then add to selection set.
+            else:
+                if backdrop:
+                    selection.add(backdrop)
+                    for n in backdrop.get_nodes():
+                        selection.add(n)
                 for node in nodes:
-                    node.selected = False
+                    if node.selected:
+                        selection.add(node)
+
+        selection.update(self.selected_nodes())
 
         # update the recorded node positions.
-        self._node_positions.update(
-            {n: n.xy_pos for n in self.selected_nodes()}
-        )
+        self._node_positions.update({n: n.xy_pos for n in selection})
 
         # show selection selection marquee.
         if self.LMB_state and not items:
             rect = QtCore.QRect(self._previous_pos, QtCore.QSize())
             rect = rect.normalized()
             map_rect = self.mapToScene(rect).boundingRect()
             self.scene().update(map_rect)
@@ -507,14 +561,18 @@
             self._set_viewer_zoom(zoom, 0.05, pos=event.pos())
         elif self.MMB_state or (self.LMB_state and self.ALT_state):
             previous_pos = self.mapToScene(self._previous_pos)
             current_pos = self.mapToScene(event.pos())
             delta = previous_pos - current_pos
             self._set_viewer_pan(delta.x(), delta.y())
 
+        if not self.ALT_state:
+            if self.SHIFT_state or self.CTRL_state:
+                self._cusor_text.setPos(self.mapToScene(event.pos()))
+
         if self.LMB_state and self._rubber_band.isActive:
             rect = QtCore.QRect(self._origin_pos, event.pos()).normalized()
             # if the rubber band is too small, do not show it.
             if max(rect.width(), rect.height()) > 5:
                 if not self._rubber_band.isVisible():
                     self._rubber_band.show()
                 map_rect = self.mapToScene(rect).boundingRect()
@@ -611,14 +669,31 @@
         self.SHIFT_state = event.modifiers() == QtCore.Qt.ShiftModifier
 
         # Todo: find a better solution to catch modifier keys.
         if event.modifiers() == (QtCore.Qt.AltModifier | QtCore.Qt.ShiftModifier):
             self.ALT_state = True
             self.SHIFT_state = True
 
+        # show cursor text
+        self._cusor_text.setVisible(False)
+        if not self.ALT_state:
+            if self.SHIFT_state:
+                self._cusor_text.setPlainText(
+                    '\n    SHIFT:'
+                    '\n    Toggle/Extend Selection'
+                )
+            elif self.CTRL_state:
+                self._cusor_text.setPlainText(
+                    '\n    CTRL:'
+                    '\n    Deselect Nodes'
+                )
+            if self.SHIFT_state or self.CTRL_state:
+                self._cusor_text.setPos(self.mapToScene(self._previous_pos))
+                self._cusor_text.setVisible(True)
+
         super(NodeViewer, self).keyPressEvent(event)
 
     def keyReleaseEvent(self, event):
         """
         Key release event re-implemented to update the states for attributes:
         - ALT_state
         - CTRL_state
@@ -628,40 +703,56 @@
             event (QtGui.QKeyEvent): key event.
         """
         self.ALT_state = event.modifiers() == QtCore.Qt.AltModifier
         self.CTRL_state = event.modifiers() == QtCore.Qt.ControlModifier
         self.SHIFT_state = event.modifiers() == QtCore.Qt.ShiftModifier
         super(NodeViewer, self).keyReleaseEvent(event)
 
+        # hide and reset cursor text.
+        self._cusor_text.setPlainText('')
+        self._cusor_text.setVisible(False)
+
     # --- scene events ---
 
     def sceneMouseMoveEvent(self, event):
         """
         triggered mouse move event for the scene.
-         - redraw the connection pipe.
+         - redraw the live connection pipe.
 
         Args:
             event (QtWidgets.QGraphicsSceneMouseEvent):
                 The event handler from the QtWidgets.QGraphicsScene
         """
         if not self._LIVE_PIPE.isVisible():
             return
         if not self._start_port:
             return
 
         pos = event.scenePos()
-        items = self.scene().items(pos)
-        if items and isinstance(items[0], PortItem):
-            x = items[0].boundingRect().width() / 2
-            y = items[0].boundingRect().height() / 2
-            pos = items[0].scenePos()
-            pos.setX(pos.x() + x)
-            pos.setY(pos.y() + y)
+        color_mode = None
+        for item in self.scene().items(pos):
+            if isinstance(item, PortItem):
+                x = item.boundingRect().width() / 2
+                y = item.boundingRect().height() / 2
+                pos = item.scenePos()
+                pos.setX(pos.x() + x)
+                pos.setY(pos.y() + y)
+                if item == self._start_port:
+                    break
+                color_mode = 'accept'
+                if self.acyclic:
+                    if item.node == self._start_port.node:
+                        color_mode = 'reject'
+                    elif item.port_type == self._start_port.port_type:
+                        color_mode = 'reject'
+                break
 
-        self._LIVE_PIPE.draw_path(self._start_port, cursor_pos=pos)
+        self._LIVE_PIPE.draw_path(
+            self._start_port, cursor_pos=pos, color_mode=color_mode
+        )
 
     def sceneMousePressEvent(self, event):
         """
         triggered mouse press event for the scene (takes priority over viewer event).
          - detect selected pipe and start connection.
          - remap Shift and Ctrl modifier.
 
@@ -870,14 +961,18 @@
             return
         self._start_port = selected_port
         if self._start_port.type == PortTypeEnum.IN.value:
             self._LIVE_PIPE.input_port = self._start_port
         elif self._start_port == PortTypeEnum.OUT.value:
             self._LIVE_PIPE.output_port = self._start_port
         self._LIVE_PIPE.setVisible(True)
+        self._LIVE_PIPE.draw_index_pointer(
+            selected_port,
+            self.mapToScene(self._origin_pos)
+        )
 
     def end_live_connection(self):
         """
         delete live connection pipe and reset start port.
         (hides the pipe item used for drawing the live connection)
         """
         self._LIVE_PIPE.reset_path()
```

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt/widgets/viewer_nav.py` & `NodeGraphQt-0.5.8/NodeGraphQt/widgets/viewer_nav.py`

 * *Files 9% similar despite different names*

```diff
@@ -64,15 +64,18 @@
                     x, rect.center().y() - (size / 2), size, size)
                 painter.setBrush(clr)
                 painter.drawRoundedRect(itm_rect, 2.0, 2.0)
                 size -= 5.0
                 x += 2.5
 
         # text
-        pen_color = option.palette.text().color()
+        # pen_color = option.palette.text().color()
+        pen_color = QtGui.QColor(*tuple(map(
+            lambda i, j: i - j, (255, 255, 255), bg_color.getRgb()
+        )))
         pen = QtGui.QPen(pen_color, 0.5)
         pen.setCapStyle(QtCore.Qt.RoundCap)
         painter.setPen(pen)
 
         font = painter.font()
         font_metrics = QtGui.QFontMetrics(font)
         item_text = item.text().replace(' ', '_')
@@ -80,15 +83,16 @@
             font_width = font_metrics.horizontalAdvance(item_text)
         else:
             font_width = font_metrics.width(item_text)
         font_height = font_metrics.height()
         text_rect = QtCore.QRectF(
             rect.center().x() - (font_width / 2) + txt_offset,
             rect.center().y() - (font_height / 2),
-            font_width, font_height)
+            font_width, font_height
+        )
         painter.drawText(text_rect, item.text())
         painter.restore()
 
 
 class NodeNavigationWidget(QtWidgets.QListView):
 
     navigation_changed = QtCore.Signal(str, list)
@@ -137,23 +141,31 @@
         self.model().sourceMode().clear()
 
     def add_label_item(self, label, node_id):
         item = QtGui.QStandardItem(label)
         item.setToolTip(node_id)
         metrics = QtGui.QFontMetrics(item.font())
         if hasattr(metrics, 'horizontalAdvance'):
-            width = metrics.horizontalAdvance(item.text()) + 30
+            width = metrics.horizontalAdvance(item.text())
         else:
-            width = metrics.width(item.text()) + 30
+            width = metrics.width(item.text())
+        width *= 1.5
         item.setSizeHint(QtCore.QSize(width, 20))
         self.model().appendRow(item)
         self.selectionModel().setCurrentIndex(
             self.model().indexFromItem(item),
             QtCore.QItemSelectionModel.ClearAndSelect)
 
+    def update_label_item(self, label, node_id):
+        rows = reversed(range(self.model().rowCount()))
+        for r in rows:
+            item = self.model().item(r, 0)
+            if item.toolTip() == node_id:
+                item.setText(label)
+
     def remove_label_item(self, node_id):
         rows = reversed(range(1, self.model().rowCount()))
         node_ids = [self.model().item(r, 0).toolTip() for r in rows]
         if node_id not in node_ids:
             return
         index = node_ids.index(node_id)
         if index == 0:
```

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt.egg-info/PKG-INFO` & `NodeGraphQt-0.5.8/NodeGraphQt.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NodeGraphQt
-Version: 0.5.7
+Version: 0.5.8
 Summary: Node graph framework for PySide2/PyQt5 that can be
 Home-page: https://github.com/jchanvfx/NodeGraphQt
 Author: Johnny Chan
 License: MIT License
 Project-URL: Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/
 Project-URL: Tracker, https://github.com/jchanvfx/NodeGraphQt/issues
@@ -26,14 +26,22 @@
 </p>
 
 ``NodeGraphQt`` is a node graph UI framework for `PySide2` that can be implemented and re-purposed into 
 applications.
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/screenshot.png" width="100%" title="NodeGraphQt">
 
+## Install
+
+NodeGraphQt is avaliable on The Python Package Index (PyPI) here https://pypi.org/project/NodeGraphQt so it can be installed with:
+```
+pip install NodeGraphQt
+```
+or you can download previous versions from the [releases](https://github.com/jchanvfx/NodeGraphQt/releases) page.
+
 
 ## Documentation
 
 <a href="https://jchanvfx.github.io/NodeGraphQt" target="_blank">https://jchanvfx.github.io/NodeGraphQt</a>
 
 See the [basic_example.py](/examples/basic_example.py) python script from this repo.
 
@@ -53,7 +61,8 @@
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/pipe_layout_types.gif" width="600" title="Pipe Layout">
 
 ## Custom Widgets
 
 https://jchanvfx.github.io/NodeGraphQt/api/html/custom_widgets.html
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/prop_bin.png" width="600" title="Properties Bin">
+<img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/nodes_palette.png" width="600" title="Node Palette">
```

#### html2text {}

```diff
@@ -1,27 +1,33 @@
-Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.5.7 Summary: Node graph
+Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.5.8 Summary: Node graph
 framework for PySide2/PyQt5 that can be Home-page: https://github.com/jchanvfx/
 NodeGraphQt Author: Johnny Chan License: MIT License Project-URL:
 Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/ Project-URL:
 Tracker, https://github.com/jchanvfx/NodeGraphQt/issues Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: PySide2 License-File:
 LICENSE.md # NodeGraphQt
   [https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
                                    logo.png]
 ``NodeGraphQt`` is a node graph UI framework for `PySide2` that can be
 implemented and re-purposed into applications. [https://
 raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
-screenshot.png] ## Documentation https://jchanvfx.github.io/NodeGraphQt See the
-[basic_example.py](/examples/basic_example.py) python script from this repo.
-More examples can be found in the API documentation:
+screenshot.png] ## Install NodeGraphQt is avaliable on The Python Package Index
+(PyPI) here https://pypi.org/project/NodeGraphQt so it can be installed with:
+``` pip install NodeGraphQt ``` or you can download previous versions from the
+[releases](https://github.com/jchanvfx/NodeGraphQt/releases) page. ##
+Documentation https://jchanvfx.github.io/NodeGraphQt See the [basic_example.py]
+(/examples/basic_example.py) python script from this repo. More examples can be
+found in the API documentation:
 https://jchanvfx.github.io/NodeGraphQt/api/html/examples/
 ex_overview.html#simple-example ## Vertical Layout https://jchanvfx.github.io/
 NodeGraphQt/api/html/examples/ex_pipe.html#layout-direction [https://
 raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
 vertical_layout.png] ## Pipe Layout https://jchanvfx.github.io/NodeGraphQt/api/
 html/examples/ex_pipe.html#layout-styles [https://raw.githubusercontent.com/
 jchanvfx/NodeGraphQt/main/docs/_images/pipe_layout_types.gif] ## Custom Widgets
 https://jchanvfx.github.io/NodeGraphQt/api/html/custom_widgets.html [https://
 raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/prop_bin.png]
+[https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
+nodes_palette.png]
```

### Comparing `NodeGraphQt-0.5.7/NodeGraphQt.egg-info/SOURCES.txt` & `NodeGraphQt-0.5.8/NodeGraphQt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/PKG-INFO` & `NodeGraphQt-0.5.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NodeGraphQt
-Version: 0.5.7
+Version: 0.5.8
 Summary: Node graph framework for PySide2/PyQt5 that can be
 Home-page: https://github.com/jchanvfx/NodeGraphQt
 Author: Johnny Chan
 License: MIT License
 Project-URL: Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/
 Project-URL: Tracker, https://github.com/jchanvfx/NodeGraphQt/issues
@@ -26,14 +26,22 @@
 </p>
 
 ``NodeGraphQt`` is a node graph UI framework for `PySide2` that can be implemented and re-purposed into 
 applications.
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/screenshot.png" width="100%" title="NodeGraphQt">
 
+## Install
+
+NodeGraphQt is avaliable on The Python Package Index (PyPI) here https://pypi.org/project/NodeGraphQt so it can be installed with:
+```
+pip install NodeGraphQt
+```
+or you can download previous versions from the [releases](https://github.com/jchanvfx/NodeGraphQt/releases) page.
+
 
 ## Documentation
 
 <a href="https://jchanvfx.github.io/NodeGraphQt" target="_blank">https://jchanvfx.github.io/NodeGraphQt</a>
 
 See the [basic_example.py](/examples/basic_example.py) python script from this repo.
 
@@ -53,7 +61,8 @@
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/pipe_layout_types.gif" width="600" title="Pipe Layout">
 
 ## Custom Widgets
 
 https://jchanvfx.github.io/NodeGraphQt/api/html/custom_widgets.html
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/prop_bin.png" width="600" title="Properties Bin">
+<img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/nodes_palette.png" width="600" title="Node Palette">
```

#### html2text {}

```diff
@@ -1,27 +1,33 @@
-Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.5.7 Summary: Node graph
+Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.5.8 Summary: Node graph
 framework for PySide2/PyQt5 that can be Home-page: https://github.com/jchanvfx/
 NodeGraphQt Author: Johnny Chan License: MIT License Project-URL:
 Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/ Project-URL:
 Tracker, https://github.com/jchanvfx/NodeGraphQt/issues Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: PySide2 License-File:
 LICENSE.md # NodeGraphQt
   [https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
                                    logo.png]
 ``NodeGraphQt`` is a node graph UI framework for `PySide2` that can be
 implemented and re-purposed into applications. [https://
 raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
-screenshot.png] ## Documentation https://jchanvfx.github.io/NodeGraphQt See the
-[basic_example.py](/examples/basic_example.py) python script from this repo.
-More examples can be found in the API documentation:
+screenshot.png] ## Install NodeGraphQt is avaliable on The Python Package Index
+(PyPI) here https://pypi.org/project/NodeGraphQt so it can be installed with:
+``` pip install NodeGraphQt ``` or you can download previous versions from the
+[releases](https://github.com/jchanvfx/NodeGraphQt/releases) page. ##
+Documentation https://jchanvfx.github.io/NodeGraphQt See the [basic_example.py]
+(/examples/basic_example.py) python script from this repo. More examples can be
+found in the API documentation:
 https://jchanvfx.github.io/NodeGraphQt/api/html/examples/
 ex_overview.html#simple-example ## Vertical Layout https://jchanvfx.github.io/
 NodeGraphQt/api/html/examples/ex_pipe.html#layout-direction [https://
 raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
 vertical_layout.png] ## Pipe Layout https://jchanvfx.github.io/NodeGraphQt/api/
 html/examples/ex_pipe.html#layout-styles [https://raw.githubusercontent.com/
 jchanvfx/NodeGraphQt/main/docs/_images/pipe_layout_types.gif] ## Custom Widgets
 https://jchanvfx.github.io/NodeGraphQt/api/html/custom_widgets.html [https://
 raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/prop_bin.png]
+[https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
+nodes_palette.png]
```

### Comparing `NodeGraphQt-0.5.7/README.md` & `NodeGraphQt-0.5.8/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 </p>
 
 ``NodeGraphQt`` is a node graph UI framework for `PySide2` that can be implemented and re-purposed into 
 applications.
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/screenshot.png" width="100%" title="NodeGraphQt">
 
+## Install
+
+NodeGraphQt is avaliable on The Python Package Index (PyPI) here https://pypi.org/project/NodeGraphQt so it can be installed with:
+```
+pip install NodeGraphQt
+```
+or you can download previous versions from the [releases](https://github.com/jchanvfx/NodeGraphQt/releases) page.
+
 
 ## Documentation
 
 <a href="https://jchanvfx.github.io/NodeGraphQt" target="_blank">https://jchanvfx.github.io/NodeGraphQt</a>
 
 See the [basic_example.py](/examples/basic_example.py) python script from this repo.
 
@@ -35,7 +43,8 @@
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/pipe_layout_types.gif" width="600" title="Pipe Layout">
 
 ## Custom Widgets
 
 https://jchanvfx.github.io/NodeGraphQt/api/html/custom_widgets.html
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/prop_bin.png" width="600" title="Properties Bin">
+<img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/nodes_palette.png" width="600" title="Node Palette">
```

#### html2text {}

```diff
@@ -1,18 +1,24 @@
  # NodeGraphQt
   [https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
                                    logo.png]
 ``NodeGraphQt`` is a node graph UI framework for `PySide2` that can be
 implemented and re-purposed into applications. [https://
 raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
-screenshot.png] ## Documentation https://jchanvfx.github.io/NodeGraphQt See the
-[basic_example.py](/examples/basic_example.py) python script from this repo.
-More examples can be found in the API documentation:
+screenshot.png] ## Install NodeGraphQt is avaliable on The Python Package Index
+(PyPI) here https://pypi.org/project/NodeGraphQt so it can be installed with:
+``` pip install NodeGraphQt ``` or you can download previous versions from the
+[releases](https://github.com/jchanvfx/NodeGraphQt/releases) page. ##
+Documentation https://jchanvfx.github.io/NodeGraphQt See the [basic_example.py]
+(/examples/basic_example.py) python script from this repo. More examples can be
+found in the API documentation:
 https://jchanvfx.github.io/NodeGraphQt/api/html/examples/
 ex_overview.html#simple-example ## Vertical Layout https://jchanvfx.github.io/
 NodeGraphQt/api/html/examples/ex_pipe.html#layout-direction [https://
 raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
 vertical_layout.png] ## Pipe Layout https://jchanvfx.github.io/NodeGraphQt/api/
 html/examples/ex_pipe.html#layout-styles [https://raw.githubusercontent.com/
 jchanvfx/NodeGraphQt/main/docs/_images/pipe_layout_types.gif] ## Custom Widgets
 https://jchanvfx.github.io/NodeGraphQt/api/html/custom_widgets.html [https://
 raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/prop_bin.png]
+[https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
+nodes_palette.png]
```

### Comparing `NodeGraphQt-0.5.7/examples/hotkeys/hotkey_functions.py` & `NodeGraphQt-0.5.8/examples/hotkeys/hotkey_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,14 +128,32 @@
 def delete_nodes(graph):
     """
     Delete selected node.
     """
     graph.delete_nodes(graph.selected_nodes())
 
 
+def extract_nodes(graph):
+    """
+    Extract selected nodes.
+    """
+    graph.extract_nodes(graph.selected_nodes())
+
+
+def clear_node_connections(graph):
+    """
+    Clear port connection on selected nodes.
+    """
+    graph.undo_stack().beginMacro('clear selected node connections')
+    for node in graph.selected_nodes():
+        for port in node.input_ports() + node.output_ports():
+            port.clear_connections()
+    graph.undo_stack().endMacro()
+
+
 def select_all_nodes(graph):
     """
     Select all nodes.
     """
     graph.select_all()
```

### Comparing `NodeGraphQt-0.5.7/examples/nodes/basic_nodes.py` & `NodeGraphQt-0.5.8/examples/nodes/basic_nodes.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/examples/nodes/custom_ports_node.py` & `NodeGraphQt-0.5.8/examples/nodes/custom_ports_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/examples/nodes/widget_nodes.py` & `NodeGraphQt-0.5.8/examples/nodes/widget_nodes.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.7/setup.cfg` & `NodeGraphQt-0.5.8/setup.cfg`

 * *Files identical despite different names*

