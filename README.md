Liste des variables smarty utilisées avec prestashop
$category
$category->name
$category->description
$category->id_image
$category->link_rewrite
$category->id
$category->id_parent
$category->active
$category->position
$category->level_depth
$category->nleft
$category->nright
$category->link_rewrite
$category->meta_title
$category->meta_keywords
$category->meta_description
$category->date_add
$category->date_upd
$subcategory
$subcategory.name
$subcategory.description
$subcategory.link_rewrite
$subcategory.id_category
$product
$product->category
$product->reduction_to
$product->reduction_from
$product.category
$product.name
$product.description
$product.description_short
$product.link_rewrite
$product.id_product_attribute
$product.id_product
$product.available_for_order
$product.price
$product.price_tax_exc
$product.reduction_percent
$product.price_without_reduction
$conf
$conf.PS_SHOP_ADDR1
$conf.PS_SHOP_ADDR2
$conf.PS_SHOP_CITY
$conf.PS_SHOP_CODE
$conf.PS_SHOP_COUNTRY
$conf.PS_SHOP_DETAILS
$conf.PS_SHOP_NAME
Globals
$base_dir (root folder of your shop)
$base_dir_ssl (root folder of your shop using HTTPS protocol)
$content_dir (root folder of your shop depending on the SSL settings)
$img_ps_dir (root folder containing images “/img/”)
$img_dir (images folder in your current theme directory)
$css_dir (css folder inside the current theme folder)
$js_dir (JavaScript inside the theme folder)
$tpl_dir (theme root folder)
$modules_dir (modules root folder)
$mail_dir (mail templates root folder)
$lang_iso (current language ISO code)
$come_from (previous page address [absolute])
$shop_name (your specified shop name)
$cart_qties (total number of products in the cart)
$cart (shopping cart contents)
$currencies (pulls available currencies)
$id_currency_cookie (selected currency id [cookie dependent])
$currency (active currency)
$cookie (active cookie)
$languages (grabs available languages)
$logged (checks whether users is logged in)
$page_name (current page’s name)
$customerName (customer name [session dependent])
$priceDisplay (current price display settings [currency dependent])


Ci dessous les variables Smarty (trouvées sur Variables Smarty)


{$base_dir}

Url de votre site web, racine du site. Utile et indispensable lorsque vous insérez des liens, je déconseille fortement de mettre des liens en dur directement dans votre code mais plutôt d’utilisez cette variable et toute les autres qui suivent, car le jour où vous migrez d’hébergement ou de nom de domaine, cela pourrait vous causer beaucoup de problèmes.

{$base_dir_ssl}

Idem via le protocol https.

{$content_dir}

Url vers votre dossier racine du site, peut changer en fonction des paramètres SSL. A ne pas confondre avec {$basedir}, cette variable vous donne l’Url complète jusqu’au dossier racine.

{$img_ps_dir}

Url vers le dossier img situé à la racine de votre boutique.

{$img_dir}

Url vers le dossier img de votre thème.

{$css_dir}

Url vers le dossier css de votre thème.

{$js_dir}

Url vers le dossier js situé à la racine de votre boutique.

{$tpl_dir}

Url vers votre dossier thème.

{$modules_dir}

Url vers le dossier modules. Utilisée principalement dans le code des modules.

{$mail_dir}

Url vers le dossier mail.

{$lang_iso}

Code ISO du language courant.

{$come_from}

Url absolue de la page précédente.

{$shop_name}

Nom de votre boutique.

{$cart_qties}

Nombre total de produits dans votre panier.

{$cart}

Contenu de votre panier sous forme de tableau.

{$currencies}

Liste des devises disponibles sous forme de tableau, retrouvez la liste via ce code {foreach from=$currencies item=c}{$c.name}{/foreach}

{$id_currency_cookie}

Identifiant de la devise actuelle.

{$languages}

Liste des langages disponibles dans la boutique sous forme de tableau, retrouvez la liste via ce code : {foreach from=$languages item=c}{$c.name}{/foreach}

{$logged}

Permet de vérifier si le client est connecté, utile pour afficher des éléments uniquement aux visiteurs enregistrés. (ex : {if $logged}Vous êtes connecté{/if}

{$page_name}

Nom de la page actuelle (ex: index)

{$customerName}

Nom et prénom du client actuellement connecté.

{$priceDisplay}

Paramètre actuel de l’affichage des prix (identifiant)
