# Art Gallery Setup Instructions

## How to add new artwork

1. **Add your PNG file** to the `/home/images/` folder
   - Name your file something descriptive (e.g., `sunset-painting.png`, `ceramic-vase.png`)

2. **Update the metadata** in `/home/artworks.json`:
   ```json
   {
     "filename": "your-image.png",
     "title": "Title of Your Artwork",
     "description": "Write about where you got this piece and what it means to you. You can include links using markdown syntax like [artist name](https://artist-website.com)."
   }
   ```

3. **That's it!** The gallery will automatically display your new artwork.

## File structure
```
/home/
  ├── index.html          # Main gallery page
  ├── artwork.html        # Template for individual artwork pages
  ├── style.css          # Styling for all pages
  ├── artworks.json      # Metadata for all artworks
  └── images/            # Folder for all PNG files
      ├── example1.png
      ├── example2.png
      └── your-art.png
```

## Notes
- The gallery dynamically loads all artworks from `artworks.json`
- Each artwork gets its own detail page automatically
- The order in `artworks.json` determines the display order in the grid
- For best results, use PNG files with consistent aspect ratios