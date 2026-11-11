# Certificate URL website

This is a static website that hosts the supplied certificate PDF and displays it at a short URL.

## Certificate URL

After deployment, use:

`https://YOUR-VERCEL-DOMAIN.vercel.app/verify/NPTEL26GE82S953800010`

The certificate ID is taken from the roll number printed on the uploaded PDF. This is an independent hosting page, not an official NPTEL verification service.

## Deploy on Vercel

1. Extract this ZIP.
2. Create a new GitHub repository and upload all files/folders from this project.
3. Open https://vercel.com, sign in, and choose **Add New → Project**.
4. Import the GitHub repository.
5. Keep the framework preset as **Other**. No build command is needed; the output is the project root.
6. Deploy.
7. Open the deployed `/verify/NPTEL26GE82S953800010` URL and test it on a phone.

## QR code

Once deployed, create a QR code containing the complete deployed URL:

`https://YOUR-VERCEL-DOMAIN.vercel.app/verify/NPTEL26GE82S953800010`

Do not create the final QR code until you know your deployed Vercel domain.

## Add another certificate

1. Put the new PDF in `public/certificates/`.
2. Add a new entry to the `certificates` object in `index.html`, with a unique ID, display details, and the PDF path.
3. Push the changes to GitHub; Vercel will redeploy automatically.

## Important

Anyone with the URL can view this PDF. Do not upload certificates containing information you do not want publicly accessible. This website only hosts/displays the supplied PDF; it does not independently validate the certificate with NPTEL.
