# Mihraza
import React from "react"; import Link from "next/link";

export default function Home() { const categories = [ { name: "Tunik & Gömlek", href: "/kategori/tunik-gomlek", }, { name: "İkili Takım", href: "/kategori/ikili-takim", }, { name: "Şal & Eşarp", href: "/kategori/sal-esarp", }, { name: "Çorap", href: "/kategori/corap", }, { name: "Parfüm", href: "/kategori/parfum", }, ];

return ( <main className="min-h-screen bg-white text-gray-800 p-4"> <h1 className="text-3xl font-bold text-center mb-8">Mihraza – Zarafetin Adı</h1> <p className="text-center text-sm mb-10 text-gray-600">Tesettür modasının en zarif parçalarını keşfedin</p> <div className="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-4"> {categories.map((cat) => ( <Link
key={cat.name}
href={cat.href}
className="border rounded-2xl shadow p-6 hover:shadow-lg transition text-center"


