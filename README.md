<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Stranger Things | Netflix Clone</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        .movie-hero {
            background: linear-gradient(to top, #141414 0%, transparent 100%);
        }
        .play-btn:hover {
            background-color: rgba(255,255,255,0.9);
        }
        .modal {
            transition: opacity 0.3s ease;
        }
        .video-player {
            width: 100%;
            height: 100%;
            background: black;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
        }
    </style>
</head>
<body class="bg-[#141414] text-white">
    <!-- Header -->
    <header class="fixed w-full z-50 bg-gradient-to-b from-black to-transparent">
        <div class="flex items-center justify-between px-12 py-4">
            <div class="flex items-center">
                <a href="index.html" class="text-red-600 font-bold text-4xl mr-8">NETFLIX</a>
                <nav class="hidden md:flex space-x-6">
                    <a href="#" class="hover:text-gray-300">TV Shows</a>
                    <a href="#" class="hover:text-gray-300">Movies</a>
                    <a href="#" class="hover:text-gray-300">My List</a>
                </nav>
            </div>
            <div class="flex items-center space-x-4">
                <i class="fas fa-search text-xl cursor-pointer"></i>
                <i class="fas fa-bell text-xl cursor-pointer"></i>
                <div class="w-8 h-8 bg-red-600 rounded cursor-pointer"></div>
            </div>
        </div>
    </header>

    <!-- Movie Hero Section -->
    <section class="relative pt-20">
        <div class="absolute inset-0 movie-hero"></div>
        <img src="https://images.pexels.com/photos/3495061/pexels-photo-3495061.jpeg" 
             alt="Stranger Things" 
             class="w-full h-screen object-cover">
        
        <div class="absolute bottom-0 left-0 right-0 px-12 pb-12">
            <h1 class="text-5xl font-bold mb-4">Stranger Things</h1>
            <div class="flex items-center space-x-4 mb-6">
                <span class="text-green-500 font-semibold">97% Match</span>
                <span>2016</span>
                <span class="border border-gray-400 px-1 text-xs">TV-14</span>
                <span>3 Seasons</span>
            </div>
            <div class="flex space-x-4">
                <button id="playBtn" class="bg-white text-black px-8 py-2 rounded flex items-center play-btn">
                    <i class="fas fa-play mr-2"></i> Play
                </button>
                <button class="bg-gray-600 bg-opacity-70 px-8 py-2 rounded flex items-center">
                    <i class="fas fa-plus mr-2"></i> My List
                </button>
            </div>
            <p class="max-w-2xl mt-4">When a young boy vanishes, a small town uncovers a mystery involving secret experiments, terrifying supernatural forces and one strange little girl.</p>
        </div>
    </section>

    <!-- Movie Details -->
    <section class="px-12 py-8">
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-8">
            <div class="lg:col-span-2">
                <h2 class="text-2xl font-bold mb-4">About Stranger Things</h2>
                <div class="grid grid-cols-2 gap-4 mb-6">
                    <div>
                        <p class="text-gray-400">Cast:</p>
                        <p>Millie Bobby Brown, Finn Wolfhard, Winona Ryder, David Harbour</p>
                    </div>
                    <div>
                        <p class="text-gray-400">Genres:</p>
                        <p>Sci-Fi TV, TV Thrillers, Teen TV Shows</p>
                    </div>
                    <div>
                        <p class="text-gray-400">This show is:</p>
                        <p>Ominous, Nostalgic, Exciting</p>
                    </div>
                    <div>
                        <p class="text-gray-400">Maturity Rating:</p>
                        <p>TV-14 • Fear, Language, Violence</p>
                    </div>
                </div>
                <p class="mb-6">In 1980s Indiana, a group of young friends witness supernatural forces and secret government exploits. As they search for answers, the children unravel a series of extraordinary mysteries.</p>
                
                <h3 class="text-xl font-bold mb-4">Episodes</h3>
                <div class="space-y-4">
                    <div class="flex items-start space-x-4 p-2 hover:bg-gray-800 rounded cursor-pointer">
                        <span class="text-gray-400">1</span>
                        <div>
                            <h4 class="font-semibold">Chapter One: The Vanishing of Will Byers</h4>
                            <p class="text-sm text-gray-400">After a boy disappears, his mother, a police chief and his friends must confront terrifying supernatural forces to get him back.</p>
                        </div>
                    </div>
                    <div class="flex items-start space-x-4 p-2 hover:bg-gray-800 rounded cursor-pointer">
                        <span class="text-gray-400">2</span>
                        <div>
                            <h4 class="font-semibold">Chapter Two: The Weirdo on Maple Street</h4>
                            <p class="text-sm text-gray-400">As they search for Will, the boys encounter a mysterious girl with supernatural abilities.</p>
                        </div>
                    </div>
                    <div class="flex items-start space-x-4 p-2 hover:bg-gray-800 rounded cursor-pointer">
                        <span class="text-gray-400">3</span>
                        <div>
                            <h4 class="font-semibold">Chapter Three: Holly, Jolly</h4>
                            <p class="text-sm text-gray-400">The search for Will intensifies, and the boys face new challenges.</p>
                        </div>
                    </div>
                    <div class="flex items-start space-x-4 p-2 hover:bg-gray-800 rounded cursor-pointer">
                        <span class="text-gray-400">4</span>
                        <div>
                            <h4 class="font-semibold">Chapter Four: The Body</h4>
                            <p class="text-sm text-gray-400">The boys discover a shocking truth about Will's disappearance.</p>
                        </div>
                    </div>
                    <div class="flex items-start space-x-4 p-2 hover:bg-gray-800 rounded cursor-pointer">
                        <span class="text-gray-400">5</span>
                        <div>
                            <h4 class="font-semibold">Chapter Five: The Flea and the Acrobat</h4>
                            <p class="text-sm text-gray-400">The group devises a plan to confront the supernatural forces at play.</p>
                        </div>
                    </div>
                </div>
            </div>
            
            <div>
                <h3 class="text-xl font-bold mb-4">More Like This</h3>
                <div class="grid grid-cols-3 gap-2">
                    <div class="cursor-pointer">
                        <img src="https://images.pexels.com/photos/33129/popcorn-movie-party-entertainment.jpg" 
                             alt="Related 1" 
                             class="w-full h-24 object-cover rounded">
                    </div>
                    <div class="cursor-pointer">
                        <img src="https://images.pexels.com/photos/1231234/pexels-photo-1231234.jpeg" 
                             alt="Related 2" 
                             class="w-full h-24 object-cover rounded">
                    </div>
                    <div class="cursor-pointer">
                        <img src="https://images.pexels.com/photos/1231235/pexels-photo-1231235.jpeg" 
                             alt="Related 3" 
                             class="w-full h-24 object-cover rounded">
                    </div>
                    <div class="cursor-pointer">
                        <img src="https://images.pexels.com/photos/1231236/pexels-photo-1231236.jpeg" 
                             alt="Related 4" 
                             class="w-full h-24 object-cover rounded">
                    </div>
                    <div class="cursor-pointer">
                        <img src="https://images.pexels.com/photos/1231237/pexels-photo-1231237.jpeg" 
                             alt="Related 5" 
                             class="w-full h-24 object-cover rounded">
                    </div>
                    <div class="cursor-pointer">
                        <img src="https://images.pexels.com/photos/1231238/pexels-photo-1231238.jpeg" 
                             alt="Related 6" 
                             class="w-full h-24 object-cover rounded">
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Trailer Modal -->
    <div id="trailerModal" class="fixed inset-0 bg-black bg-opacity-90 z-50 flex items-center justify-center hidden modal">
        <div class="relative w-full max-w-4xl">
            <button id="closeModal" class="absolute -top-12 right-0 text-white text-2xl">
                <i class="fas fa-times"></i>
            </button>
            <div class="aspect-w-16 aspect-h-9 video-player">
                <video controls class="w-full h-full">
                    <source src="path_to_your_trailer.mp4" type="video/mp4">
                    Your browser does not support the video tag.
                </video>
            </div>
        </div>
    </div>

    <script>
        // Trailer Modal functionality
        const playBtn = document.getElementById('playBtn');
        const trailerModal = document.getElementById('trailer
