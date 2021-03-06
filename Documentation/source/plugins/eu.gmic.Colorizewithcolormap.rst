.. _eu.gmic.Colorizewithcolormap:

G’MIC Colorize with colormap node
=================================

*This documentation is for version 0.3 of G’MIC Colorize with colormap.*

Description
-----------

User-defined gradient :

Author: David Tschumperle. Latest update: 2010/29/12.

Wrapper for the G’MIC framework (http://gmic.eu) written by Tobias Fleischer (http://www.reduxfx.com).

Inputs
------

+-------+-------------+----------+
| Input | Description | Optional |
+=======+=============+==========+
| Input |             | No       |
+-------+-------------+----------+

Controls
--------

.. tabularcolumns:: |>{\raggedright}p{0.2\columnwidth}|>{\raggedright}p{0.06\columnwidth}|>{\raggedright}p{0.07\columnwidth}|p{0.63\columnwidth}|

.. cssclass:: longtable

+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
| Parameter / script name                                       | Type    | Default                              | Function                  |
+===============================================================+=========+======================================+===========================+
| Brightness (%) / ``Brightness_``                              | Double  | 0                                    |                           |
+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
| Contrast (%) / ``Contrast_``                                  | Double  | 0                                    |                           |
+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
| Gamma (%) / ``Gamma_``                                        | Double  | 0                                    |                           |
+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
| Normalize input / ``Normalize_input``                         | Boolean | Off                                  |                           |
+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
| Gradient preset / ``Gradient_preset``                         | Choice  | User-defined                         | |                         |
|                                                               |         |                                      | | **User-defined**        |
|                                                               |         |                                      | | **Black to white**      |
|                                                               |         |                                      | | **White to black**      |
|                                                               |         |                                      | | **Sepia**               |
|                                                               |         |                                      | | **Solarize**            |
+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
| Interpolation type / ``Interpolation_type``                   | Choice  | Linear                               | |                         |
|                                                               |         |                                      | | **Nearest**             |
|                                                               |         |                                      | | **Linear**              |
|                                                               |         |                                      | | **Cubic**               |
|                                                               |         |                                      | | **Lanczos**             |
+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
| Preserve initial brightness / ``Preserve_initial_brightness`` | Boolean | Off                                  |                           |
+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
| Number of tones / ``Number_of_tones``                         | Integer | 5                                    |                           |
+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
| 1st tone / ``p1st_tone``                                      | Color   | r: 0 g: 0 b: 0                       |                           |
+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
| 2nd tone / ``p2nd_tone``                                      | Color   | r: 0.168627 g: 0.0980392 b: 0.215686 |                           |
+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
| 3rd tone / ``p3rd_tone``                                      | Color   | r: 0.619608 g: 0.537255 b: 0.741176  |                           |
+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
| 4th tone / ``p4th_tone``                                      | Color   | r: 0.878431 g: 0.74902 b: 0.894118   |                           |
+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
| 5th tone / ``p5th_tone``                                      | Color   | r: 1 g: 1 b: 1                       |                           |
+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
| 6th tone / ``p6th_tone``                                      | Color   | r: 1 g: 1 b: 1                       |                           |
+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
| 7th tone / ``p7th_tone``                                      | Color   | r: 1 g: 1 b: 1                       |                           |
+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
| 8th tone / ``p8th_tone``                                      | Color   | r: 1 g: 1 b: 1                       |                           |
+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
| Preview type / ``Preview_type``                               | Choice  | Full                                 | |                         |
|                                                               |         |                                      | | **Full**                |
|                                                               |         |                                      | | **Forward horizontal**  |
|                                                               |         |                                      | | **Forward vertical**    |
|                                                               |         |                                      | | **Backward horizontal** |
|                                                               |         |                                      | | **Backward vertical**   |
|                                                               |         |                                      | | **Duplicate top**       |
|                                                               |         |                                      | | **Duplicate left**      |
|                                                               |         |                                      | | **Duplicate bottom**    |
|                                                               |         |                                      | | **Duplicate right**     |
+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
| Output Layer / ``Output_Layer``                               | Choice  | Layer 0                              | |                         |
|                                                               |         |                                      | | **Merged**              |
|                                                               |         |                                      | | **Layer 0**             |
|                                                               |         |                                      | | **Layer 1**             |
|                                                               |         |                                      | | **Layer 2**             |
|                                                               |         |                                      | | **Layer 3**             |
|                                                               |         |                                      | | **Layer 4**             |
|                                                               |         |                                      | | **Layer 5**             |
|                                                               |         |                                      | | **Layer 6**             |
|                                                               |         |                                      | | **Layer 7**             |
|                                                               |         |                                      | | **Layer 8**             |
|                                                               |         |                                      | | **Layer 9**             |
+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
| Resize Mode / ``Resize_Mode``                                 | Choice  | Dynamic                              | |                         |
|                                                               |         |                                      | | **Fixed (Inplace)**     |
|                                                               |         |                                      | | **Dynamic**             |
|                                                               |         |                                      | | **Downsample 1/2**      |
|                                                               |         |                                      | | **Downsample 1/4**      |
|                                                               |         |                                      | | **Downsample 1/8**      |
|                                                               |         |                                      | | **Downsample 1/16**     |
+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
| Ignore Alpha / ``Ignore_Alpha``                               | Boolean | Off                                  |                           |
+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
| Preview/Draft Mode / ``PreviewDraft_Mode``                    | Boolean | Off                                  |                           |
+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
| Log Verbosity / ``Log_Verbosity``                             | Choice  | Off                                  | |                         |
|                                                               |         |                                      | | **Off**                 |
|                                                               |         |                                      | | **Level 1**             |
|                                                               |         |                                      | | **Level 2**             |
|                                                               |         |                                      | | **Level 3**             |
+---------------------------------------------------------------+---------+--------------------------------------+---------------------------+
