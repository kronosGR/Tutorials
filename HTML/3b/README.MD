### Chapter 3 - Basic Media
#### 3b. Video  (`<video>`): For embedding video files.
##### 1. What is the `<video>` Element?
The `<video>` element is an HTML5 semantic element used to embed video content directly into web pages without requiring third-party plugins like Flash. It provides a standardized way to display videos that works across all modern browsers.

* Basic Syntax and Structure
  
```html
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  Your browser does not support the video tag.
</video>
```

##### 2. Video Common Attributes
###### Essential Attributes
* src
Specifies the URL of the video file to embed.
```html
<video src="example.mp4"></video>
```

* controls
Displays video controls (play, pause, volume, etc.) for the user.
```html
<video src="movie.mp4" controls></video>
```

* width and height
Sets the dimensions of the video player.
```html
<video src="movie.mp4" width="640" height="480"></video>
```

###### Media Control Attributes
* autoplay
Specifies that the video should start playing as soon as it is ready.
```html
<video src="movie.mp4" autoplay></video>
```

* loop
Specifies that the video should loop when it reaches the end.
```html
<video src="movie.mp4" loop></video>
```

* muted
Specifies that the audio output of the video should be muted.
```html
<video src="movie.mp4" muted></video>
```

* preload
Specifies if and how the author thinks the video should be loaded when the page loads.

Values:
	- auto: Load the entire video
	- metadata: Load only metadata (like duration, dimensions)
	- none: Do not load the video
```html	
<video src="movie.mp4" preload="metadata"></video>
```

###### Advanced Attributes
* poster
Specifies an image to be shown while the video is downloading, or until the user hits the play button.
```html
<video src="movie.mp4" poster="thumbnail.jpg"></video>
```

* playsinline
For iOS Safari, this attribute allows videos to play inline instead of fullscreen.
```html
<video src="movie.mp4" playsinline></video>
```

##### 3.  Multiple Video Sources
The `<video>` element supports multiple `<source>` elements to provide different video formats for compatibility:

```html
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  <source src="movie.webm" type="video/webm">
  Your browser does not support the video tag.
</video>
```

##### 4. Video Format Support
Common Video Formats:
1. MP4 - Most widely supported, especially with H.264 codec
2. WebM - Open format, good for Chrome and Firefox
3. Ogg - Open format, supported by Firefox and Opera
4. MOV - Apple's format, less common

* Browser Support Matrix
  
```
Format	Chrome	Firefox	Safari	Edge
MP4		✓		✓		✓		✓
WebM	✓		✓		✗		✓
Ogg		✗		✓		✗		✗
```

##### 5. Video Element Events
The `<video>` element supports various JavaScript events for interactive control:
- loadstart: When loading of the video starts
- canplay: When enough data is available to start playing
- playing: When video starts playing
- pause: When video is paused
- ended: When video reaches the end
- error: When an error occurs

##### 6. Accessibility Considerations
Provide captions: Use `<track>` element for subtitles
Descriptive text: Include alternative content for screen readers
Keyboard navigation: Ensure controls are accessible via keyboard
```html
<video controls>
  <source src="movie.mp4" type="video/mp4">
  <track kind="captions" src="captions.vtt" srclang="en" label="English">
  Your browser does not support the video tag.
</video>
```

##### 7. SEO Benefits
1. Structured data: Use schema.org markup for videos
2. Descriptive metadata: Include relevant keywords in video titles and descriptions
3. Fast loading: Properly optimized videos improve page speed scores

##### 8. Performance Optimization Tips
1. Choose appropriate formats: MP4 for broad compatibility, WebM for modern browsers
2. Compress videos: Reduce file sizes without sacrificing quality
3. Use responsive design: Make videos adapt to different screen sizes
4. Implement lazy loading: Load videos only when needed
5. Provide multiple resolutions: Offer different quality versions

##### 9. Common Use Cases
1. Product demonstrations: Show products in action
2. Tutorials and how-tos: Educational content
3. Marketing videos: Promotional material for businesses
4. Live streaming: Real-time video content
5. Background videos: Decorative video backgrounds (use carefully)

##### 10. Browser Compatibility
The `<video>` element is supported in all modern browsers:

- Chrome 4+
- Firefox 3.5+
- Safari 4+
- Internet Explorer 9+
- Edge 12+

##### 11. Troubleshooting Common Issues
1. Video not playing: Check file paths and formats
2. Autoplay blocked: Most browsers block autoplay with sound
3. Mobile compatibility: Use playsinline for iOS devices
4. Cross-origin issues: Handle CORS properly for external videos
5. Performance problems: Optimize video files and use appropriate preload settings

##### 12. Project additions for the chapter
To include a video in your project, you'll need to create a new video file and update the my-first-post.html file.

```html
 <video width="640" height="360" controls>
        <source src="video1" type="video/mp4" />
        Your browser does not support the video tag.
      </video>
```
File Changed: The my-first-post.html file is updated to include the `<video>` element, which embeds the video into the blog post. This tag uses the src attribute to specify the video file's location. The controls attribute is added to provide a play/pause button, volume control, and other standard video player functions.

##### 13. Questions
1. What are the main advantages of using the HTML5 `<video>` element over older Flash-based video embedding methods?
2. How does the preload attribute affect website performance, and when would you choose each preload value?
3. Explain how to provide multiple video formats for maximum browser compatibility and what the `<source>` element's role is in this process.
4. What are the differences between using autoplay, loop, and muted attributes together, and why is the muted attribute often required for autoplay to work?
5. How can you ensure that videos load efficiently while maintaining good user experience, considering both performance and accessibility?
6. What is the purpose of the poster attribute, and how does it improve the user experience when loading videos?
7. Describe the differences between MP4, WebM, and Ogg video formats in terms of browser support and use cases.
8. How can you make videos accessible to users with disabilities, including those who rely on screen readers or have hearing impairments?
9. What are some best practices for optimizing video files for web delivery, including compression techniques and file size considerations?
10. How do modern browsers handle autoplay policies, and what strategies can developers use to work within these restrictions while still providing engaging video content?


