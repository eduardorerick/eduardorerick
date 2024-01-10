<a href="https://www.linkedin.com/in/eduardo-rerick-4799191a0/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/socials/linkedin.svg" width="32" height="32" /></a>

```rust
//main.rs

mod profile;
use profile::print_profile;
use profile::SoftwareEngineer;

fn main() {
    let eduardo_rerick = SoftwareEngineer {
        name: "Eduardo Rerick",
        experience: 4,
        current_position: "Senior Software Engineer",
        current_company: "Caju",
        education: Education {
            degree: "Bachelor's in Chemistry",
            post_graduation: "Postgraduate in Software Engineering",
        },
        skills: vec![
            "JavaScript", "Python", "HTML", "CSS", "Typescript", "Rust",
            "React", "Next", "Node", "Express", "Nest", "Databricks",
            "Azure", "MongoDB", "SQL", "NoSQL", "Grafana", "Jaeger",
            "Open Telemetry", "Docker", "Prometheus"
        ],
        social_media_links: vec![
            "https://www.linkedin.com/in/eduardo-rerick/", "https://medium.com/@eduardorerick"
        ],
    };
}

//src/profile.rs

struct SoftwareEngineer {
    name: &'static str,
    experience: u32,
    current_position: &'static str,
    current_company: &'static str,
    education: Education,
    skills: Vec<&'static str>,
    social_media_links: Vec<&'static str>,
}

struct Education {
    degree: &'static str,
    post_graduation: &'static str,
}

```
