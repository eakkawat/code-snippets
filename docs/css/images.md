# Images

## How to fit an image inside a div container

If you have an image that is larger than its container, you can use the following CSS to make the image fit inside the container while maintaining its aspect ratio:

```CSS
img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
```

### Explanation

- `width: 100%;` and `height: 100%;` make the image take up the full width and height of its container.
- `object-fit: cover;` ensures that the image scales while maintaining its aspect ratio, and that the entire container is covered by the image. This means that if the image is larger than the container, some of the image may be cropped to fit.
