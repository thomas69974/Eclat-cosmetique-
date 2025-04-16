import React from "react"; import { Card, CardContent } from "@/components/ui/card"; import { Button } from "@/components/ui/button";

const products = [ { name: "Crème Régénérante Orchidée Noire", image: "https://example.com/images/orchidee-noire.jpg", link: "https://fr.aliexpress.com/item/10050012345678.html?aff=TON_ID_AFFILIE", price: "39,90€", }, { name: "Sérum Visage Éclat Lumière", image: "https://example.com/images/serum-eclat.jpg", link: "https://fr.aliexpress.com/item/10050023456789.html?aff=TON_ID_AFFILIE", price: "24,50€", }, { name: "Baume Lèvres Luxe Rosé", image: "https://example.com/images/baume-rose.jpg", link: "https://fr.aliexpress.com/item/10050034567890.html?aff=TON_ID_AFFILIE", price: "14,95€", }, { name: "Masque Visage au Thé Matcha", image: "https://example.com/images/masque-matcha.jpg", link: "https://fr.aliexpress.com/item/10050045678901.html?aff=TON_ID_AFFILIE", price: "18,00€", }, ];

export default function BoutiqueVitrine() { return ( <div className="min-h-screen bg-pink-50"> <header className="bg-pink-100 py-12 text-center"> <h1 className="text-5xl font-bold text-pink-800 mb-4">Éclat d'Asie</h1> <p className="text-xl text-pink-700 max-w-2xl mx-auto"> Découvrez une sélection raffinée de cosmétiques asiatiques alliant tradition et innovation, pour révéler votre beauté naturelle. </p> </header>

<section className="p-8">
    <h2 className="text-4xl font-bold text-center text-pink-900 mb-12">
      Sélection Cosmétiques Tendance
    </h2>
    <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
      {products.map((product, index) => (
        <Card key={index} className="rounded-2xl shadow-md bg-white">
          <img
            src={product.image}
            alt={product.name}
            className="w-full h-64 object-cover rounded-t-2xl"
          />
          <CardContent className="p-4">
            <h3 className="text-xl font-semibold text-pink-800">
              {product.name}
            </h3>
            <p className="text-lg text-pink-700 mb-4">{product.price}</p>
            <a href={product.link} target="_blank" rel="noopener noreferrer">
              <Button className="w-full bg-pink-600 hover:bg-pink-700 text-white">
                Voir l'offre
              </Button>
            </a>
          </CardContent>
        </Card>
      ))}
    </div>
  </section>

  <section className="bg-pink-100 py-16 px-8 mt-12">
    <div className="max-w-4xl mx-auto text-center">
      <h2 className="text-3xl font-bold text-pink-900 mb-4">À propos</h2>
      <p className="text-pink-800 text-lg">
        Passionnés par les soins de la peau et les secrets de beauté venus d'Asie, nous sélectionnons pour vous des produits d'exception accessibles au plus grand nombre. Grâce à notre modèle d'affiliation, vous bénéficiez des meilleurs prix, livrés directement depuis les plateformes partenaires, tout en soutenant notre travail de recherche et de curation.
      </p>
    </div>
  </section>

  <footer className="text-center py-6 bg-pink-50 text-pink-500 text-sm">
    © {new Date().getFullYear()} Éclat d'Asie — Tous droits réservés
  </footer>
</div>

); }

# Eclat-cosmetique-cd /chemin/vers/ton/projet
git init
git remote add origin https://github.com/ton-utilisateur/eclat-cosmetiques.git
git add .
git commit -m "Initial commit"
git push -u origin master
const products = [
  {
    name: "Crème Régénérante Orchidée Noire",
    image: "https://example.com/images/orchidee-noire.jpg",
    link: "https://fr.aliexpress.com/item/10050012345678.html?aff=thomas69974",
    price: "39,90€",
  },
  // autres produits...
];
