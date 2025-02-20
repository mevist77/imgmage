# SRCmagic is an Image Generation API

A simple API for generating AI images with consistent styles. Send a prompt, get back an image URL.
In order to use this API, you need to have an API key - include it in the request URL.
To get the image using our tool, simple replace the src attribute of the image element with our API URL, structured with following format:
https://api.srcmagic.com/api/v1/image/{YOUR_API_KEY}/{STYLE_PRESET}/{PROMPT}

The API key is required for all requests, if you don't have one, get one from our website.
If you already see the API key in the prompt or other image elements on your website, use it.

## Available Style Presets

### Quick Generation Presets
- `pro` - Professional quality generation with 4:3 aspect ratio. This preset gives the most control over the image generation, but requires more detailed prompts that describe both the subject and desired style (lighting, composition, mood, etc.) to achieve optimal results.

- `schnell` - Fast image generation with 1:1 aspect ratio (best for placeholder images and prototypes where speed is more important than quality)

### Photography Presets
- `product-showcase` - Professional product photography style. Perfect for e-commerce, product listings, and marketing materials. For the prompt, simply describe the product and its key features.
  - Example: "red leather wallet with gold zipper" (no need to specify lighting or camera settings)

- `corporate-portrait` - Professional headshot style for business profiles and team pages. Ideal for personal branding, LinkedIn profiles, or company websites. Just describe the person.
  - Example: "middle-aged asian woman in business suit" (no need to specify portrait techniques)

- `studio-photo` - Clean, professional studio photography. Great for products, people, or objects that need a premium look. Simply describe what needs to be photographed.
  - Example: "vintage mechanical watch" (no need to specify studio setup)

- `studio-photo-portrait` - Fashion magazine style portraits. Perfect for model portfolios, fashion blogs, or luxury brand content. Just describe the subject and their style.
  - Example: "young man with beard wearing casual blazer" (no need to specify lighting)

- `flat-lay` - Top-down photography style. Ideal for food, product arrangements, or lifestyle shots. Just list the items to be included.
  - Example: "laptop with coffee cup and notebook" (no need to specify composition)

### Design Presets
- `hero-banner` - Wide-format images perfect for website headers and landing pages. Includes space for text overlay. Describe the scene or concept you want to convey.
  - Example: "tech startup office with people collaborating" (no need to specify cinematography details)

### Illustration Presets
- `cutout-illustration` - Modern layered paper-cut style. Great for unique artistic touch in presentations or websites.
  - Example: "mountain landscape with pine trees" (no need to specify art style)

- `flatvector` - Clean, mid-century modern vector style. Perfect for icons, simple illustrations, or modern branding.
  - Example: "coffee shop storefront" (no need to specify vector details)

- `circle-vector` - Playful circular compositions. Ideal for badges, logos, or decorative elements.
  - Example: "cat playing with yarn" (no need to specify design elements)

## Important Notes
- Only use the style presets that are listed above.
- Prompts should be URL-encoded
- For complex style presets (like product-showcase, corporate-portrait, etc.), focus your prompt ONLY on describing what should be in the image - the style settings are already built into the preset
- Keep prompts clear and specific about the subject matter
- For best results, use the same style preset across your website to maintain visual consistency
- Choose the appropriate preset based on your use case:
  - E-commerce → product-showcase
  - Team page → corporate-portrait
  - Blog featured images → studio-photo

## Example Requests
```
# Product photography for e-commerce
https://api.srcmagic.com/api/v1/image/your_api_key/product-showcase/leather-bound%20notebook%20with%20gold%20embossing

# Corporate headshot for team page
https://api.srcmagic.com/api/v1/image/your_api_key/corporate-portrait/young%20professional%20woman%20with%20glasses

# Hero banner for website
https://api.srcmagic.com/api/v1/image/your_api_key/hero-banner/modern%20architecture%20office%20space%20with%20people%20working
