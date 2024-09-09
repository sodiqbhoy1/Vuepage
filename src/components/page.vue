<template>
    <div>
      <!-- Hero Section -->
      <section class="bg-blue-600 text-white py-20 rounded">
        <div class="container mx-auto text-center">
          <h1 class="text-4xl font-bold mb-4">Welcome to MyApp</h1>
          <p class="text-xl mb-6">Your solution for awesome web experiences</p>
          <a href="#" class="bg-white text-blue-600 py-3 px-6 rounded-full font-semibold hover:bg-gray-100">Get Started</a>
        </div>
      </section>
  
      <!-- Features Section -->
      <section class="py-16">
        <div class="container mx-auto px-4">
          <h2 class="text-3xl font-bold text-center mb-12">Features</h2>
          <div class="grid md:grid-cols-3 gap-8">
            <div class="p-6 bg-white shadow-md rounded-lg text-center">
              <h3 class="text-xl font-bold mb-2">Feature One</h3>
              <p class="text-gray-600">Learn more about how Feature One can help you achieve your goals!</p>
            </div>
            <div class="p-6 bg-white shadow-md rounded-lg text-center">
              <h3 class="text-xl font-bold mb-2">Feature Two</h3>
              <p class="text-gray-600">Feature Two brings incredible power and flexibility to your project.</p>
            </div>
            <div class="p-6 bg-white shadow-md rounded-lg text-center">
              <h3 class="text-xl font-bold mb-2">Feature Three</h3>
              <p class="text-gray-600">Maximize your efficiency with the amazing Feature Three!</p>
            </div>
          </div>
        </div>
      </section>
  
      <!-- Call to Action Section -->
      <section class="bg-gray-100 py-16">
        <div class="container mx-auto text-center">
          <h2 class="text-3xl font-bold mb-6">Ready to get started?</h2>
          <a href="#" class="bg-blue-600 text-white py-3 px-6 rounded-full font-semibold hover:bg-blue-700">Join Now</a>
        </div>
      </section>
  
      <!-- Footer Section -->
      <footer class="bg-gray-800 text-white py-8 rounded">
        <div class="container mx-auto text-center">
          <p>&copy; 2024 MyApp. All rights reserved.</p>
        </div>
      </footer>
    </div>
  </template>
  
  <script>
  export default {
    name: "LandingPage",
  };
  </script>
  
  