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
        current_company: "Yssy",
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
        education_background: Education {
            degree: "Bachelor's in Chemistry",
            post_graduation: "Postgraduate in Software Engineering",
        },
        social_media_links: vec![
            "LinkedIn", "Twitter", "Personal Blog"
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
    highlighted_projects: Vec<Project>,
    education_background: Education,
    social_media_links: Vec<&'static str>,
    open_source_contributions: Vec<Contribution>,
}

struct Education {
    degree: &'static str,
    post_graduation: &'static str,
}

```
