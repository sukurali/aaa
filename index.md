

## Mathjax

Math equations can be rendered using [Mathjax](https://www.mathjax.org) syntax with AMS symbol support.

Optionally enable this on a per-page basis by adding `mathjax: true` to your frontmatter.

Then, use `$$ ... $$` on a line by itself to render a block equation:

$$ | Pr_{x \leftarrow P_{1}} [A(x) = 1] - Pr_{x \leftarrow P_{2}} [A(x) = 1] | < \text{negligible} $$

The raw version is:

```
$$ | Pr_{x \leftarrow P_{1}} [A(x) = 1] - Pr_{x \leftarrow P_{2}} [A(x) = 1] | < \text{negligible} $$
```


Write in-line equations with `\\( ... \\)` , like \\( x^n / y \\) . It's easy!

```
Write in-line equations with `\\( ... \\)` , like \\( x^n / y \\) . It's easy!
```
## X Simple Shortcode
```
{{</* x user="GoHugoIO" id="1315233626070503424" */>}}
```
<br>
{{< x user="GoHugoIO" id="1315233626070503424" >}}
<br>



## Vimeo Simple Shortcode
```
{{</* vimeo 146022717 */>}}
```
<br>
{{< vimeo 146022717 >}}
<br>



## Youtube Simple Shortcode
```
{{</* youtube w7Ft2ymGmfc */>}}
```
<br>
{{< youtube w7Ft2ymGmfc >}}
<br>

## Theme Custom Shortcodes

These shortcodes are not Hugo built-ins, but are provided by the theme.

### Responsive Images with Cloudinary

You can learn more about this [here](https://cloudinary.com/documentation/responsive_images).

Set the `cloudinary_cloud_name` parameter in your site config to use this shortcode.

```
{{</* dynamic-img src="/my/image/on/cloudinary" title="A title for the image" */>}}
```

Note that you do not include the file extension (e.g. `.png`) in the `src` parameter, as the shortcode will automatically determine the best quality and format for the user's device.

Optionally, you can customize the general CSS styles for the image:

```
{{</* dynamic-img src="/my/image/on/cloudinary" title="A title for the image" style="max-width:60%" */>}}
```

