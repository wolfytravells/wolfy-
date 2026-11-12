WOLFY TRAVELLER BUS WEBSITE

Files:
- index.html: public bus rental website, booking enquiry form, owner photo upload and public gallery
- admin.html: owner-only login, customer enquiry list, status update
- supabase_setup.sql: database and storage policies

SETUP
1. Create a free project at https://supabase.com/
2. In Project Settings > API, copy Project URL and anon/public key.
3. In BOTH index.html and admin.html replace:
   PASTE_YOUR_SUPABASE_PROJECT_URL
   PASTE_YOUR_SUPABASE_ANON_PUBLIC_KEY
   with your project's values.
4. In supabase_setup.sql replace owner@example.com with the owner's Supabase Auth email.
5. Run the whole SQL file in Supabase > SQL Editor.
6. In Supabase > Authentication > Users, create/invite the owner user using that same email and a strong password.
7. Publish index.html and admin.html to a GitHub repository. In Settings > Pages choose Deploy from a branch, main, /(root).
8. Public website URL will be https://YOUR-USERNAME.github.io/REPOSITORY/
   Owner dashboard: https://YOUR-USERNAME.github.io/REPOSITORY/admin.html

OWNER PHOTO UPLOAD
Sign in at admin.html first in the same browser, then open the public website and upload photos in the owner upload section. Public visitors can see photos but cannot upload through this template.

BOOKINGS
Visitors submit trip enquiries. Owner sees customer name, phone, travel date, days, pickup, destination, passengers and message. Owner can set Pending, Confirmed or Cancelled. This does not automatically check vehicle availability, calculate fares, or take payments; owner must contact customer and confirm manually.

IMPORTANT
- Never put the Supabase service_role key in website code. Use only anon/public key.
- Keep admin password private. The owner-only policies restrict booking access and photo uploads by owner email.
- Before public launch, test as a visitor and as owner. Add real vehicle photos, actual seating capacity, amenities, contact/WhatsApp details, service area, fare policy, cancellation policy and privacy notice.
- The template restricts image types and file size but is not a full image moderation system. Owner should review gallery content.
- Do not publish private customer details in the gallery or public pages.
