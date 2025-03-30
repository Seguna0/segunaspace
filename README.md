import React from 'react';
import { Card, CardContent } from '@/components/ui/card';
import { Button } from '@/components/ui/button';
import { FaTwitter, FaInstagram, FaLinkedin, FaFilePdf } from 'react-icons/fa';
import { motion } from 'framer-motion';

const Portfolio = () => {
  return (
    <div className="min-h-screen bg-gradient-to-b from-gray-900 to-black text-white">
      {/* Header */}
      <header className="text-center py-12">
        <h1 className="text-4xl font-bold">こばりょ | ポートフォリオ & 資料</h1>
        <p className="text-lg mt-4">挑戦と成長を続ける未来志向のビジネスパーソン</p>
      </header>
      
      {/* Profile Section */}
      <section className="p-8 max-w-4xl mx-auto">
        <Card className="bg-gray-800 rounded-2xl shadow-lg">
          <CardContent className="p-6">
            <h2 className="text-2xl font-semibold">プロフィール</h2>
            <p className="mt-4">株式会社Piety創業者 / 株式会社OH! My family CCO / 宇宙教育事業を副業で展開中。</p>
            <p className="mt-2">Photosynthでの営業・事業開発に従事しながら、SNS運用や登壇活動を行う。</p>
          </CardContent>
        </Card>
      </section>

      {/* Works Section */}
      <section className="p-8 max-w-4xl mx-auto">
        <h2 className="text-3xl font-bold mb-6">実績</h2>
        <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
          <Card className="bg-gray-800 rounded-2xl shadow-lg">
            <CardContent className="p-6">
              <h3 className="text-xl font-semibold">鳥取竹イベント登壇</h3>
              <p className="mt-2">地域活性化のための登壇、竹の活用事例を紹介。</p>
            </CardContent>
          </Card>

          <Card className="bg-gray-800 rounded-2xl shadow-lg">
            <CardContent className="p-6">
              <h3 className="text-xl font-semibold">宇宙無線給電コンテスト出場</h3>
              <p className="mt-2">宇宙エネルギー活用に関するアイデアを発表。</p>
            </CardContent>
          </Card>
        </div>
      </section>

      {/* PDF Section */}
      <section className="p-8 max-w-4xl mx-auto">
        <h2 className="text-3xl font-bold mb-6">資料</h2>
        <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
          <Card className="bg-gray-800 rounded-2xl shadow-lg">
            <CardContent className="p-6">
              <FaFilePdf size={40} className="text-red-500 mb-4" />
              <h3 className="text-xl font-semibold">講義資料1</h3>
              <a href="/pdfs/lecture1.pdf" target="_blank" rel="noopener noreferrer">
                <Button variant="outline" className="mt-4">PDFを表示</Button>
              </a>
            </CardContent>
          </Card>
          
          <Card className="bg-gray-800 rounded-2xl shadow-lg">
            <CardContent className="p-6">
              <FaFilePdf size={40} className="text-red-500 mb-4" />
              <h3 className="text-xl font-semibold">講義資料2</h3>
              <a href="/pdfs/lecture2.pdf" target="_blank" rel="noopener noreferrer">
                <Button variant="outline" className="mt-4">PDFを表示</Button>
              </a>
            </CardContent>
          </Card>
          
          <Card className="bg-gray-800 rounded-2xl shadow-lg">
            <CardContent className="p-6">
              <FaFilePdf size={40} className="text-red-500 mb-4" />
              <h3 className="text-xl font-semibold">就活資料</h3>
              <a href="/pdfs/job_hunting.pdf" target="_blank" rel="noopener noreferrer">
                <Button variant="outline" className="mt-4">PDFを表示</Button>
              </a>
            </CardContent>
          </Card>
        </div>
      </section>
      
      {/* Gourmet, Travel, Movies, Books Section */}
      <section className="p-8 max-w-4xl mx-auto">
        <h2 className="text-3xl font-bold mb-6">特集ページ</h2>
        <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
          <Card className="bg-gray-800 rounded-2xl shadow-lg">
            <CardContent className="p-6">
              <h3 className="text-xl font-semibold">グルメ特集</h3>
              <p className="mt-2">おすすめのレストランや料理を紹介。</p>
            </CardContent>
          </Card>

          <Card className="bg-gray-800 rounded-2xl shadow-lg">
            <CardContent className="p-6">
              <h3 className="text-xl font-semibold">旅行特集</h3>
              <p className="mt-2">訪れた国やおすすめスポットを紹介。</p>
            </CardContent>
          </Card>

          <Card className="bg-gray-800 rounded-2xl shadow-lg">
            <CardContent className="p-6">
              <h3 className="text-xl font-semibold">映画紹介</h3>
              <p className="mt-2">お気に入りの映画やレビューを掲載。</p>
            </CardContent>
          </Card>

          <Card className="bg-gray-800 rounded-2xl shadow-lg">
            <CardContent className="p-6">
              <h3 className="text-xl font-semibold">本の紹介</h3>
              <p className="mt-2">おすすめの本や感想を共有。</p>
            </CardContent>
          </Card>
        </div>
      </section>
      
      {/* Contact Section */}
      <section className="p-8 max-w-4xl mx-auto text-center">
        <h2 className="text-3xl font-bold">お問い合わせ</h2>
        <p className="mt-4">SNSからお気軽にご連絡ください。</p>
        <div className="flex justify-center space-x-6 mt-6">
          <Button variant="ghost">
            <FaTwitter size={32} />
          </Button>
          <Button variant="ghost">
            <FaInstagram size={32} />
          </Button>
          <Button variant="ghost">
            <FaLinkedin size={32} />
          </Button>
        </div>
      </section>
      
      <footer className="text-center py-4 text-gray-400">
        © 2025 こばりょ. All rights reserved.
      </footer>
    </div>
  );
};

export default Portfolio;
