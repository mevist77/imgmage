# imgmage
# AI image generation tool for AI-first design engineers


A simple API for generating AI images with consistent styles. Send a prompt, get back an image URL.
In order to use this API, you need to have a private API key - include it in the request URL.
To get the image using our tool, simple replace the src attribute of the image element with our API URL, structured with following format:
http://localhost:8000/api/v1/image/{YOUR_API_KEY}/{STYLE_PRESET}/{PROMPT}

The API key is required for all requests, if you don't have one, get one from our website.
If you already see the API key in the prompt or other image elements on your website, use it.

Only choose one of the available style presets below. 


## Available Style Presets
- `basic` - Default image generation preset with 1792x2368 resolution

## Example Request
http://localhost:8000/api/v1/image/your_api_key/basic/pixel-art-illustration-of-a-cat

## Notes
- Prompts should be URL-encoded
- Feel free to generate any kind of prompt you want, but the more specific the better.
- API key is required for all requests
- If not told differently, try to use the same style preset for all images in your page. If you are generating prompts, try to keep them in the same visual style too, only replace the object / scene / description, etc. This will make all the images in your page look consistent.
