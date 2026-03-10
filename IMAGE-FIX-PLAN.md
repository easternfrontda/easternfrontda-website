# 🚨 GENSPARK IMAGE HOSTING ISSUE - SIMPLE FIX

## THE PROBLEM:
GenSpark image URLs return "403 Forbidden" when accessed from external sites (Netlify). This is hotlink protection.

## THE SIMPLE SOLUTION:

Replace GenSpark image URLs with placeholder images from a reliable CDN that allows hotlinking.

**Using: placeholder.com and via.placeholder.com**

These services provide FREE placeholder images that work on ANY website.

## UPDATED IMAGE REPLACEMENTS:

### Original → Replacement

**Logos:**
- Logo nav: Use solid color Navy background with white text "EFDA"
- Logo footer: Same as above

**Hero Background:**
- Military/tactical themed: https://images.unsplash.com/photo-1526474703/9cb6088c4aca?w=1920

**Instructor Photo:**
- Professional portrait: https://images.unsplash.com/photo-1560250097-0b93528c311a?w=800

**Training Photos:**
- Range training: https://images.unsplash.com/photo-1595590424283-b8f17842773f?w=800
- Pistol training: https://images.unsplash.com/photo-1614902103976-42c163b8d82d?w=800
- Rifle training: https://images.unsplash.com/photo-1599623560574-39d485900c95?w=800

**Course Preview Images:**
- Generic tactical/firearms training from Unsplash (free, no restrictions, works everywhere)

## IMPLEMENTATION:

I'll update index.html with Unsplash image URLs. These are:
✅ Free to use
✅ No hotlink restrictions  
✅ High quality
✅ Work on all platforms
✅ Fast CDN delivery

User can replace with real photos later by simply uploading images to Netlify and updating URLs.
