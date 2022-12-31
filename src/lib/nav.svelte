
<script>



  const links = [
    {
      href: "/a",
      label: "Home"
    },
    {
      href: "/b",
      label: "About"
    },
    {
      href: "/c",
      label: "Portfolio"
    },
    {
      href: "/d",
      label: "Experience"
    },
    {
      href: "/e",
      label: "Contact"
    },
  ];
  </script>
  
  
  
    <nav class="flex justify-between items-center w-full h-20 px-4 bg-gray-800  text-white">
      <div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8">
        <a href="/">
          <!-- adding <a href="/" will compose the image to function as a home link -->
          <img src="" class="nav-logo" alt="" />
          <!-- image on top of nav -->
        </a>
      </div>
    
      <ul class= "flex">
        {#each links as { href, label}}
        <li class="px-4 cursor-pointer font-medium text-gray-500 hover:scale-105 duration-200">
          <a {href}>{label}</a>{/each}
      </ul>
    </nav>