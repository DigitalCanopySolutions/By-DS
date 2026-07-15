Contenu à ajouter dans le Google Doc source de Canopy-Beta-Setup-Guide.pdf
(pas de source éditable trouvée dans le dossier, juste le PDF final — à
coller là où tu maintiens réellement le document, puis réexporter).

=====================================================================
1. Petit ajout ponctuel, à la fin de l'étape 1C (juste après l'install
   de G-Connector, avant l'étape 2)
=====================================================================

Just installed it? If you see a red error banner right away, don't
worry — just reload the page once (Cmd+R or F5). Fresh installs
almost always need one reload before they work.

=====================================================================
2. Nouvelle section "Troubleshooting", à ajouter juste avant la
   dernière page ("This is an early, hand-run beta...")
=====================================================================

TROUBLESHOOTING — quick fixes before you reach out

Most hiccups here have a one-click fix. Try these first:

Red error message right after installing G-Connector (something like
"PERMISSION_DENIED")
→ Reload the page once. Fresh installs need it, it's normal.

A screen saying "Google hasn't verified this app"
→ That's expected — it's just Google being cautious about a small
add-on. Click "Advanced", then "Go to G-Connector (unsafe)". You're
only authorizing your own copy with your own Zoho account, nothing
leaves your Google account.

The "☁️ Canopy" menu doesn't show up next to Help
→ Reload the page. This menu only loads when the Sheet opens, so if
you were already on the page when it got added, a refresh brings it
in.

You clicked "Build / Rebuild" but the Leads/Dashboard/Alerts pages
look empty or unchanged
→ Make sure Step 3 (Get Module Data) actually pulled your Zoho leads
into Sheet1 first — Canopy builds its report from that data, so if
Sheet1 is still empty, there's nothing yet to build from.

Still stuck after trying the above? That's genuinely useful for us to
know — reply to the email that sent you this guide, or write to
contact@digitalsubstrate.io. Screenshots help a lot if you can grab
one.

=====================================================================
Pourquoi ces 4 cas précisément
=====================================================================
- Le 1er, c'est très exactement le bug qu'on vient de croiser en test
  (erreur PERMISSION_DENIED juste après l'install, réglée par un
  rechargement).
- Le 2ème couvre l'écran "app non vérifiée" que Google affiche souvent
  pour des Add-ons peu connus, surtout sur un compte Gmail perso — un
  testeur qui tombe dessus sans explication risque de cliquer "Retour
  en sécurité" et de rester bloqué sans même comprendre pourquoi.
- Le 3ème couvre le cas où le menu ☁️ Canopy semble "ne jamais
  apparaître" alors qu'il suffit de recharger (le menu ne se
  reconstruit qu'à l'ouverture de la feuille, pas en direct).
- Le 4ème couvre l'erreur d'ordre la plus probable : cliquer Build
  avant d'avoir importé les données Zoho.
