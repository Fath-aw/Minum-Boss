  <script> 
    // Mobile menu toggle 
    const menuBtn = document.getElementById('menu-btn'); 
    const navLinks = document.querySelector('nav ul'); 
    menuBtn.addEventListener('click', () => { 
      navLinks.classList.toggle('hidden'); 
    }); 

    // Close mobile menu when a link is clicked
    const navItems = document.querySelectorAll('nav ul li a');
    navItems.forEach(item => {
      item.addEventListener('click', () => {
        if (!navLinks.classList.contains('hidden')) {
          navLinks.classList.add('hidden');
        }
      });
    });
  </script> 
</body> 
</html>
