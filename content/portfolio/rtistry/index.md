---
title: "Rtistry"
subtitle: ""
excerpt: "Generative art is the practice of creating artwork using code. When the programming language of choice is R, it's often termed *Rtistry* or *aRt*."
date: 2022-01-01
weight: 2
author: "Nicola Rennie"
draft: false
categories:
  - Rtistry
layout: single
image: featured.jpeg
links:
- icon: github
  icon_pack: fab
  name: code
  url: https://github.com/nrennie/aRt
---

### Overview

Generative art is the practice of creating artwork using code. When the programming language of choice is R, it's often termed *Rtistry* or *aRt*. The generative artwork below can be reproduced using my {aRt} package on [GitHub](https://github.com/nrennie/aRt), which you can install in R using: 

```r
remotes::install_github("nrennie/aRt")
library(aRt)
```
You can also view my generative artwork on [Instagram](https://www.instagram.com/nrennie_art/). 

### Examples

#### attraction

The `attraction()` function produces generative art based on strange attractors.

``` r
attraction(n=50000, a=-3, b=1, c=0.5, d=-1, main_col="black", bg_col="white")
attraction(n=50000, a=-6, b=1, c=0.5, d=-2, main_col="black", bg_col="white")
attraction(n=50000, a=-3, b=-2, c=1, d=-1, main_col=rcartocolor::carto_pal(n = 7, "SunsetDark"), bg_col="white")
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/attraction1.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/attraction2.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/attraction3.jpeg?raw=true" width="30%">
</p>

#### blending

The `blending()` function produces generative art of many boxes.

``` r
blending(n = 100, down = "white", up = "black", s = 1234)
blending(n = 500, down = "white", up = "black", s = 1234)
blending(n = 100, down = "#ba1141", up = "#003366", s = 1234)

```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/blending1.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/blending2.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/blending3.jpeg?raw=true" width="30%">
</p>

#### boxes

The `boxes()` function produces generative art of many boxes.

``` r
boxes(n=100, perc=0.1, col_palette=rcartocolor::carto_pal(n = 7, "DarkMint"), bg_col="black", s=1234)
boxes(n=20, perc=0.1, col_palette=rcartocolor::carto_pal(n = 7, "DarkMint"), bg_col="black", s=1234)
boxes(n=100, perc=0.5, col_palette=rcartocolor::carto_pal(n = 7, "Magenta"), bg_col="black", s=1234)
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/boxes_n100_p1.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/boxes_n20_p1.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/boxes_n100_p5.jpeg?raw=true" width="30%">
</p>

#### bricks

The `bricks()` function draws multiple rectangular polygons in rows.

``` r
bricks(n_y=20, colours=c("#9B1D20", "#3D2B3D", "#CBEFB6", "#635D5C"), bg_col="gray97")
bricks(n_y=200, colours=c("#9B1D20", "#3D2B3D", "#CBEFB6", "#635D5C"), bg_col="gray97")
bricks(n_y=20, colours=rcartocolor::carto_pal(7, "Burg"), bg_col="gray97")

```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/bricks1.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/bricks2.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/bricks3.jpeg?raw=true" width="30%">
</p>


#### bubbles

The `bubbles()` function produces generative art using layered polar bar charts.

``` r
bubbles(num_circles = 20, main_col = "black", col_palette = rcartocolor::carto_pal(n = 12, "Bold"), bg_col = "white", s = 1234)
bubbles(num_circles = 20, main_col = "lightgrey", col_palette = rcartocolor::carto_pal(n = 12, "Bold"), bg_col = "white", s = 123)
bubbles(num_circles = 10, main_col = "white", col_palette = rcartocolor::carto_pal(n = 12, "Prism"), bg_col = "black", s = 2022)
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/bubbles1.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/bubbles2.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/bubbles3.jpeg?raw=true" width="30%">
</p>


#### bullseye

The `bullseye()` function produces generative art using layered polar bar charts.

``` r
bullseye(main_col="black", bg_col="white", s=1234)
bullseye(main_col="white", bg_col="black", s=1234)
bullseye(main_col="black", bg_col="white", s=2021)
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/bullseye_1234.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/bullseye_1234n.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/bullseye_2021.jpeg?raw=true" width="30%">
</p>

#### circles

The `circles()` function produces generative art using dendograms and circular graphs.

``` r
circles(n=100, smoothness=100, col_palette=rcartocolor::carto_pal(n = 12, "Bold"), line_col=NA, bg_col="black", s=1234)
circles(n=10, smoothness=100, col_palette=rcartocolor::carto_pal(n = 12, "Bold"), line_col=NA, bg_col="#e73f74", s=1234)
circles(n=2, smoothness=3, col_palette=rcartocolor::carto_pal(n = 12, "Bold"), line_col="black", bg_col="black", s=1234)
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/circles1.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/circles2.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/circles3.jpeg?raw=true" width="30%">
</p>

#### circular

The `circular()` function produces circular generative art produced by many random paths from the centre of the circle.

``` r
circular(n=2, main_col="black", bg_col="white", s=56)
circular(n=10, main_col="black", bg_col="white", s=56)
circular(n=100, main_col="black", bg_col="white", s=56)
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/circular_n2.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/circular_n10.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/circular_n100.jpeg?raw=true" width="30%">
</p>

#### connected

The `connected()` function produces generative art by connected points on a circle.

``` r
connected(n=100, n_geom=10, random=F, col_palette=RColorBrewer::brewer.pal(n = 9,"RdPu"), bg_col="#ae217e", s=1234)
connected(n=100, n_geom=10, random=T, col_palette=RColorBrewer::brewer.pal(n = 9,"RdPu"), bg_col="#ae217e", s=1234)
connected(n=250, n_geom=2, random=F, col_palette=RColorBrewer::brewer.pal(n = 5,"RdPu"), bg_col="#ae217e", s=1234)
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/connected_100_10F.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/connected_100_10T.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/connected_250_2F.jpeg?raw=true" width="30%">
</p>

#### crawling

The `crawling()` function produces generative art using dendograms and tree graphs.

``` r
crawling(n=50, edge_colour="black", node_size=1, node_colour="black", bg_col="white", s=1234)
crawling(n=250, edge_colour="black", node_size=1, node_colour="black", bg_col="white", s=1234)
crawling(n=1000, edge_colour="black", node_size=1, node_colour="black", bg_col="white", s=1234)
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/crawling50.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/crawling250.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/crawling1000.jpeg?raw=true" width="30%">
</p>

#### dots

The `dots()` function produces generative art using jittered points.

``` r
dots(n_x=50, n_y=100, jitter_size_width=0.5, jitter_size_height=0.5, col_palette = rcartocolor::carto_pal(n = 7, "Purp"), bg_col="#63589f", s=1234)
dots(n_x=500, n_y=100, jitter_size_width=0.5, jitter_size_height=5, col_palette = rcartocolor::carto_pal(n = 7, "Purp"), bg_col="#63589f", s=1234)
dots(n_x=50, n_y=100, jitter_size_width=0.05, jitter_size_height=50, col_palette = rcartocolor::carto_pal(n = 7, "Purp"), bg_col="#63589f", s=1234)
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/dots1.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/dots2.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/dots3.jpeg?raw=true" width="30%">
</p>

#### fading

The `fading()` function produces generative art using voronoi tiles.

``` r
fading(n_layers=6, n_points=10, col_palette=rcartocolor::carto_pal(n = 7, "SunsetDark"), s=1234)
fading(n_layers=6, n_points=1, col_palette=rcartocolor::carto_pal(n = 7, "Sunset"), s=1234)
fading(n_layers=10, n_points=10, col_palette=rcartocolor::carto_pal(n = 7, "SunsetDark"), s=1234)
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/fading_6_10.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/fading_6_1.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/fading_10_10.jpeg?raw=true" width="30%">
</p>

#### flow fields

The `flow_fields()` function produces generative art using particle traces. These functions are inspired by a blog post by [Will Chase](https://www.williamrchase.com/post/flow-fields-12-months-of-art-september/). 

``` r
flow_fields(n = 10000, granualarity = 1000, x_freq = 1, y_freq = 1, alpha = 1, line_col = c("#edf8fb","#bfd3e6","#9ebcda","#8c96c6","#8c6bb1","#88419d","#6e016b"), bg_col = "lightgrey", s = 1234)
flow_fields(n = 10000, granualarity = 1000, x_freq = 1, y_freq = 1, alpha = 0.3, line_col = "black", bg_col = "white", s = 1234)
flow_fields(n = 10000, granualarity = 1000, x_freq = 3, y_freq = 0.2, alpha = 1, line_col = c("#edf8fb","#bfd3e6","#9ebcda","#8c96c6","#8c6bb1","#88419d","#6e016b"), bg_col = "lightgrey", s = 1234)
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/flow_fields1.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/flow_fields2.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/flow_fields3.jpeg?raw=true" width="30%">
</p>

### fractals

The `fractals()` function produces generative art based on fractal patterns. These functions are inspired by a blog post on [R-bloggers](https://www.r-bloggers.com/2010/08/fractals-in-r/).

``` r
fractals(N = 25, col_palette = MetBrewer::met.brewer("Demuth", n = 25),
         shift = 0, left = -1, right = 1,
         y_param = 3, resolution = 0.005, dist_max = 4)
fractals(N = 25, col_palette = rev(MetBrewer::met.brewer("Benedictus", n = 25)),
         shift = 0, left = -3, right = 3,
         y_param = 2, resolution = 0.005, dist_max = 4)
fractals(N = 20, col_palette = grey.colors(30),
         shift = -1, left = -1, right = 1,
         y_param = 2, resolution = 0.005, dist_max = 3)
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/fractals1.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/fractals2.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/fractals3.jpeg?raw=true" width="30%">
</p>


#### heart

The `heart()` function draws a heart from many overlapping lines.

``` r
heart(n=25, col_scheme="mono", bg_col="black", s=1234)
heart(n=100, col_scheme="mono", bg_col="black", s=1234)
heart(n=25, col_scheme="rainbow", bg_col="black", s=1234)
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/heart_n25_m.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/heart_n100_m.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/heart_n25_r.jpeg?raw=true" width="30%">
</p>


#### infinity

The `infinity()` function draws an infinity symbol from many overlapping lines.

``` r
infinity(n=25, col_scheme="mono", bg_col="black", s=1234)
infinity(n=100, col_scheme="mono", bg_col="black", s=1234)
infinity(n=25, col_scheme="rainbow", bg_col="black", s=1234)
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/infinity_n25_m.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/infinity_n100_m.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/infinity_n25_r.jpeg?raw=true" width="30%">
</p>


#### polygons

The `polygons()` function draws multiple polygons.

``` r
polygons(n_x=12, n_y=18, gap_size=0.5, deg_jitter=0.1, colours=c("#9B1D20", "#3D2B3D", "#CBEFB6", "#635D5C"), rand = FALSE, bg_col="gray97")
polygons(n_x=6, n_y=9, gap_size=0.2, deg_jitter=0.1, colours=c("#9B1D20", "#3D2B3D", "#CBEFB6", "#635D5C"), rand = FALSE, bg_col="gray97")
polygons(n_x=12, n_y=18, gap_size=0.5, deg_jitter=0.5, colours=rcartocolor::carto_pal(7, "Burg"), rand = FALSE, bg_col="gray97")

```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/polygons1.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/polygons2.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/polygons3.jpeg?raw=true" width="30%">
</p>


#### rectangles

The `rectangles()` function draws multiple rectangles.

``` r
rectangles(n = 100, max_height = 7, max_width = 5, size = 2, main_col = "lightgrey", col_palette = rcartocolor::carto_pal(n = 12, "Bold"), bg_col = "white", s = 123)
rectangles(n = 10, max_height = 15, max_width = 15, size = 4, main_col = "lightgrey", col_palette = rcartocolor::carto_pal(n = 12, "Bold"), bg_col = "white", s = 123)
rectangles(n = 100, max_height = 4, max_width = 6, size = 1, main_col = ggplot2::alpha("white", 0.5), col_palette = rcartocolor::carto_pal(n = 12, "Prism"), bg_col = "black", s = 123)

```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/rectangles1.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/rectangles2.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/rectangles3.jpeg?raw=true" width="30%">
</p>

#### shell

The `shells()` function produces generative art using sine and cosine waves.

``` r
shells(n = 4, alpha = 1, main_col = "black", bg_col = "white")
shells(n = 10, alpha = 1, main_col = "black", bg_col = "white")
shells(n = 6, alpha = 0.5, main_col = "#CC338B", bg_col = alpha("#CC338B", 0.2))
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/shell1.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/shell2.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/shell3.jpeg?raw=true" width="30%">
</p>

#### spirals

The `spirals()` function produces generative art consisting of dots arranged in a spiral.

``` r
spirals(perc=0.2, s=1234)
spirals(perc=0.5, s=1234)
spirals(perc=0.8, s=1234)
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/spirals_p2.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/spirals_p5.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/spirals_p8.jpeg?raw=true" width="30%">
</p>

#### static

The `static()` function produces generative art reminiscent of the noise displayed on analog televisions when no transmission signal is received.

``` r
static(perc=0.01, n=500, s=1234)
static(perc=0.1, n=500, s=1234)
static(perc=0.3, n=500, s=1234)
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/static_p01_n500.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/static_p10_n500.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/static_p30_n500.jpeg?raw=true" width="30%">
</p>

#### streams

The `streams()` function produces generative art consisting of stream charts.

``` r
streams(bg_col = "white", 
        line_col = "white",
        fill_col = c("#5F4690", "#1D6996", "#38A6A5", "#0F8554",
                     "#73AF48", "#EDAD08", "#E17C05", "#CC503E", 
                     "#94346E", "#6F4070"),
        type = "right",
        s = 1234)
streams(bg_col = "black",
        line_col = NA,
        fill_col = grey.colors(n = 25),
        type = "up",
        s = 450)
streams(bg_col = "white",
        line_col = NA,
        fill_col = rep("purple", 8),
        type = "left",
        s = 13)
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/streams1.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/streams2.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/streams3.jpeg?raw=true" width="30%">
</p>

#### stripes

The `stripes()` function produces generative art consisting of rows of vertical stripes.


``` r
stripes(perc=0, n=3, col_palette = rcartocolor::carto_pal(n = 7, "TealGrn"), alpha = 1, s=1234)
stripes(perc=0.5, n=3, col_palette = rcartocolor::carto_pal(n = 7, "TealGrn"), alpha = 1, s=1234)
stripes(perc=1, n=3, col_palette = rcartocolor::carto_pal(n = 7, "TealGrn"), alpha = 1, s=1234)
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/stripes_p00_n3.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/stripes_p50_n3.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/stripes_p100_n3.jpeg?raw=true" width="30%">
</p>

#### sunbursts

The `sunbursts()` function produces generative art consisting of two-dimesional density plots.

``` r
sunbursts(n = 100, x_means = c(0, 10, 5), y_means = c(0, 7, 8), xy_var = 5, low = "#074050", high = "#d3f2a3", s = 1234)
sunbursts(n = 5, x_means = c(0, 1, 15), y_means = c(0, 2, 16), xy_var = 10, low = "#4e0550", high = "#facdfc", s = 1234)
sunbursts(n = 250, x_means = c(1, 2, 9, 50), y_means = c(3, 6, 8, -3), xy_var = 100, low = "white", high = "black", s = 1234)
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/sunbursts1.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/sunbursts2.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/sunbursts3.jpeg?raw=true" width="30%">
</p>

#### tiles

The `tiles()` function produces generative art using square polygons.

``` r
tiles(n_x=12, n_y=12, col_palette=MetBrewer::met.brewer("Veronese", 5), s=1234)
tiles(n_x=50, n_y=50, col_palette=MetBrewer::met.brewer("Veronese", 6), s=1234)
tiles(n_x=12, n_y=12, col_palette=MetBrewer::met.brewer("Pissaro", 5), s=1234)
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/tiles_veronese1.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/tiles_veronese2.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/tiles_pissaro1.jpeg?raw=true" width="30%">
</p>


#### vortex

The `vortex()` function produces circular vortex generative art produced by a line plot and polar coordinates.

``` r
vortex(n=25, start_val=90, col_scheme="mono", bg_col="black", s=1234)
vortex(n=100, start_val=90, col_scheme="mono", bg_col="black", s=1234)
vortex(n=25, start_val=90, col_scheme="rainbow", bg_col="black", s=1234)
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/vortex_n25_m.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/vortex_n100_m.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/vortex_n25_r.jpeg?raw=true" width="30%">
</p>


#### waves

The `waves()` function produces generative art using sine and cosine waves.

``` r
waves(a=23, b=6, main_col="white", bg_col="black", s=2021)
waves(a=23, b=6, main_col=rcartocolor::carto_pal(n = 7, "Prism"), bg_col="#edad08", s=2021)
waves(a=6, b=23, main_col="black", bg_col="white", s=2021)
```
<p align="center">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/waves23_6_bw.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/waves23_6_col.jpeg?raw=true" width="30%">
<img src="https://github.com/nrennie/aRt/blob/main/man/figures/waves6_23_bw.jpeg?raw=true" width="30%">
</p>
