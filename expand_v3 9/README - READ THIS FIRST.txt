═══════════════════════════════════════════════════════════════
  EXPAND ASSESSMENT SUITE — DEPLOYMENT & EMAIL SETUP GUIDE
═══════════════════════════════════════════════════════════════

STEP 1 — DEPLOY TO VERCEL (Update your live site)
───────────────────────────────────────────────────

1. Open your web browser and go to:  https://vercel.com
2. Click "Log In" and sign into your account
3. Once logged in, look at the TOP RIGHT corner
4. Click the button that says "Add New..." then click "Project"
5. You will see a page with a big section at the top that says
   "Import Git Repository" — IGNORE that section entirely
6. SCROLL DOWN the page until you see a box that says
   "Or deploy from your computer"  (it has a cloud icon)
7. Now open your File Explorer / Finder on your computer
8. Find the "expand_v3" folder you extracted from the zip
9. DRAG that folder and DROP it ONTO that specific upload box
   on the Vercel website page — NOT onto the browser tab bar
10. Vercel will show a progress bar and then say "Congratulations!"
11. Click "Visit" to see your updated live site

⚠️  IMPORTANT: You are dragging the FOLDER onto the upload BOX
    on the Vercel page — not onto the browser bar at the top.
    If the folder opens in the browser, you missed the box.


STEP 2 — SET UP EMAIL (One template in EmailJS)
────────────────────────────────────────────────

You need to create ONE template in EmailJS. This takes 5 minutes.

1. Go to:  https://www.emailjs.com
2. Log into your account
3. In the LEFT MENU click "Email Templates"
4. Click the blue button "Create New Template"
5. You will see a template editor appear
6. At the TOP of the editor, find the field called "Subject"
   → Delete whatever is there and type exactly:  {{subject}}
7. Find the field called "To Email"
   → Delete whatever is there and type exactly:  {{to_email}}
8. In the big message body area in the middle:
   → Click inside it
   → Press CTRL+A (select all) to select everything
   → DELETE it all
   → Look for a button that says "Code Editor" or "<>" or "HTML"
     and click it to switch to code/HTML view
   → Now type exactly this (and nothing else):  {{{html_body}}}
9. Click the SAVE button at the top right
10. After saving, look at the URL in your browser bar
    It will look like: emailjs.com/templates/template_xxxxxxx
    The part that says "template_xxxxxxx" is your Template ID
    COPY that ID (example: template_abc12345)
11. Send that Template ID to Christo (or your developer)
    so it can be added to the live site


WHAT HAPPENS AFTER SETUP:
──────────────────────────
→ Every time someone completes an assessment, TWO emails fire:
  1. A branded results report goes to the person who completed it
  2. A lead notification with all their details goes to
     info@christopretorius.com

═══════════════════════════════════════════════════════════════
  www.christopretorius.com
═══════════════════════════════════════════════════════════════
