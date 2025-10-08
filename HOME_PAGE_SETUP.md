# Home Page Setup - Import Instructions

## Files Created

### 1. CSS Stylesheet
- **Location**: `src/MyProject/wwwroot/css/site.css`
- **Description**: Modern "Digital Intelligence" theme with gradients and responsive design

### 2. Document Type (uSync)
- **Location**: `src/MyProject/uSync/v16/ContentTypes/home.config`
- **Properties**:
  - `pageTitle` (Textstring) - Required
  - `welcomeMessage` (Textarea)
  - `featuredImage` (Media Picker 3)

### 3. Template (uSync)
- **Location**: `src/MyProject/uSync/v16/Templates/home.config`
- **View File**: `src/MyProject/Views/home.cshtml`
- **Features**: 
  - Responsive hero section
  - Blog grid placeholder
  - About section
  - Footer with social links

### 4. Home Page Content (uSync)
- **Location**: `src/MyProject/uSync/v16/Content/home.config`
- **Pre-filled with**: Welcome message about the AI agent

## Import Instructions

### Option 1: Automatic Import (Recommended)

1. Navigate to the Umbraco backoffice: `http://localhost:14737/umbraco`
2. Go to **Settings** → **uSync** → **Dashboard**
3. Click **"Import"** button
4. uSync will automatically detect and import:
   - Home Document Type
   - Home Template
   - Home Content

### Option 2: Manual Import via Settings

1. Go to **Settings** → **Document Types**
2. The "Home" document type should appear automatically after uSync import
3. Go to **Settings** → **Templates**
4. The "Home" template should be available
5. Go to **Content**
6. The "Home" page should be in the content tree

### Option 3: Restart Application

If the files don't appear immediately:
1. Stop the application
2. Restart with: `dotnet run --project src/MyProject/MyProject.csproj`
3. uSync should auto-import on startup

## Verification Steps

1. **Check Document Type**: Settings → Document Types → "Home" should exist
2. **Check Template**: Settings → Templates → "Home" should exist  
3. **Check Content**: Content → "Home" page should be at root level
4. **View Site**: Navigate to `http://localhost:14737/` to see the home page

## Expected Result

The home page should display:
- Header with navigation (gradient background)
- Hero section with title and welcome message
- Placeholder for blog posts
- About section
- Footer

## Theme Colors

- Primary: Indigo (#6366f1)
- Secondary: Purple (#8b5cf6)
- Accent: Cyan (#06b6d4)

## Next Steps

After importing:
1. Add a featured image via Media → Upload
2. Assign the image to the home page
3. Create Blog List and Blog document types
4. Start creating blog posts

---

**Created**: October 8, 2025  
**For**: Umbraco US Festival 2025 - Chicago  
**By**: AI Agent
