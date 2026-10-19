# PTCU Hydro Research Teams

Static website for students to self-register into one of six Hydrotherapy research teams. Uses the existing Supabase project and existing admin account.

## Publish on GitHub Pages

1. Create a new GitHub repository (or open the repository where you want this site).
2. Upload **the contents of this folder** to the repository root. Make sure `index.html` is at the root, not nested inside another folder.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Choose branch `main` and folder `/(root)`, then Save.
6. Wait for GitHub Pages to publish and open the URL shown in Settings → Pages.

## Included behavior

- Six teams: the first three have capacity 6; the last three have capacity 5.
- Uses the existing roster of 34 students in Supabase.
- Each student can join one team only; each team has fixed numbered slots.
- Team membership and remaining places are displayed publicly.
- Admin login uses the existing Supabase Auth user; authorized admins can remove registrations.

## Supabase

Project: https://supabase.com/dashboard/project/wauycitelklrfxyebdgf

The browser code contains only the Supabase publishable key. **Never add a `service_role` or secret key, or an admin password, to this repository.**

Note: team capacity is 33 seats for 34 listed students, so one student will be left without a place if all teams fill. Public registration is based on selecting a name from the roster; it does not verify the student's real identity.
