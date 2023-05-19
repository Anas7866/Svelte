<script>
  import { onMount } from "svelte";
  import { Loader } from "@googlemaps/js-api-loader";

  let autocomplete;
  let address;

  const options = {
    componentRestrictions: { country: "au" },
    strictBounds: false,
  };

  onMount(() => {
    const loader = new Loader({
      apiKey: "AIzaSyDKDVVNL5FeC6oEKMdVMascV7WDuglvu8c",
      version: "weekly",
      libraries: ["places"],
    });

    loader.loadCallback((e) => {
      if (e) {
        console.log(e);
      } else {
        autocomplete = new google.maps.places.Autocomplete(
          document.getElementById("autocomplete"),
          options
        );

        autocomplete.addListener("place_changed", onPlaceChanged);
      }
    });

    function onPlaceChanged() {
      address = autocomplete.getPlace();

      console.log(address.formatted_address);
    }
  });
</script>

<main>
  <div class="input-group mb-3">
    <input
      type="text"
      class="form-control input_form_style"
      placeholder="Search..."
      aria-label="Search..."
      name="autocomplete"
      id="autocomplete"
      autocomplete="off"
      aria-describedby="basic-addon2"
    />
    <span class="input-group-text bg_search_button" id="basic-addon2"
      ><i class="fas fa-search" /></span
    >
  </div>
</main>

<style>
  .input_form_style:focus {
    box-shadow: none;
    outline: none;
    border: 1px solid #86b941;
  }
  .bg_search_button {
    background-color: #1f5a3f;
    color: white;
  }
</style>
